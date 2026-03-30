<!DOCTYPE html>
<html lang="pt-br" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MestreEBD | Apoio ao Professor PECC</title>
    <!-- Tailwind CSS para Design -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- FontAwesome para Ícones -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
    
    <style>
        body { font-family: 'Inter', sans-serif; }
        .animate-fadeIn { animation: fadeIn 0.5s ease-in-out; }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .trimestre-content.hidden { display: none; }
    </style>
</head>
<body class="bg-slate-50 text-slate-800">

    <!-- NAVEGAÇÃO -->
    <nav class="bg-slate-900 text-white shadow-xl sticky top-0 z-50 border-b border-sky-500/30">
        <div class="container mx-auto px-4 py-4 flex justify-between items-center">
            <h1 class="text-2xl font-bold tracking-tight">Mestre<span class="text-sky-400">EBD</span></h1>
            <ul class="hidden md:flex space-x-8 font-medium text-sm uppercase tracking-wider">
                <li><a href="#" class="hover:text-sky-400 transition">Início</a></li>
                <li><a href="#downloads" class="hover:text-sky-400 transition">Downloads</a></li>
                <li><a href="#dinamicas" class="hover:text-sky-400 transition">Dinâmicas</a></li>
                <li><a href="#sobre" class="hover:text-sky-400 transition">Sobre</a></li>
                <li><a href="#contato" class="hover:text-sky-400 transition">Contato</a></li>
            </ul>
            <a href="#downloads" class="bg-sky-600 hover:bg-sky-700 px-5 py-2 rounded-full text-xs font-bold transition uppercase tracking-tighter">BAIXAR PDF/PPT</a>
        </div>
    </nav>

    <!-- HERO SECTION (INÍCIO) -->
    <header class="relative bg-slate-900 text-white py-24 overflow-hidden">
        <div class="absolute inset-0 opacity-20">
            <img src="https://images.unsplash.com/photo-1504052434139-44b53d63bc3d?auto=format&fit=crop&w=1920&q=80" alt="Bíblia fundo" class="w-full h-full object-cover">
        </div>
        <div class="container mx-auto px-4 relative z-10 text-center text-balance">
            <span class="bg-sky-500/20 text-sky-400 px-4 py-1 rounded-full text-xs font-bold uppercase tracking-widest mb-6 inline-block border border-sky-500/30">Recursos para a EBD</span>
            <h2 class="text-4xl md:text-6xl font-extrabold mb-6 leading-tight">Facilitando o ensino das<br><span class="text-sky-400">Lições PECC</span></h2>
            <p class="text-xl mb-10 text-slate-300 max-w-2xl mx-auto font-light leading-relaxed">
                Slides, resumos e dinâmicas organizadas para que você foque no ministério e na vida dos seus alunos.
            </p>
            <div class="flex flex-col sm:flex-row justify-center gap-4">
                <a href="#downloads" class="bg-sky-600 hover:bg-sky-700 text-white px-10 py-4 rounded-2xl font-bold shadow-2xl transition transform hover:-translate-y-1">Acessar Downloads</a>
                <a href="#dinamicas" class="bg-white/10 hover:bg-white/20 backdrop-blur-md text-white px-10 py-4 rounded-2xl font-bold transition border border-white/20">Ver Dinâmicas</a>
            </div>
        </div>
    </header>

    <!-- DOWNLOADS (POR TRIMESTRE) -->
    <section id="downloads" class="bg-slate-900 py-20 text-white">
        <div class="container mx-auto px-4 text-center">
            <h3 class="text-3xl font-bold mb-2 text-sky-400">Materiais PECC 2026</h3>
            <p class="mb-10 text-slate-400 font-light">Selecione o trimestre para acessar os arquivos.</p>

            <!-- Menu de Abas -->
            <div class="flex flex-wrap justify-center gap-2 mb-12">
                <button onclick="abrirTrimestre(event, 't1')" class="tab-link active bg-sky-600 px-6 py-2 rounded-full font-bold transition duration-300">1º Trimestre</button>
                <button onclick="abrirTrimestre(event, 't2')" class="tab-link bg-[#1e293b] hover:bg-slate-700 px-6 py-2 rounded-full font-bold transition duration-300 border border-slate-700 text-slate-400">2º Trimestre</button>
                <button onclick="abrirTrimestre(event, 't3')" class="tab-link bg-[#1e293b] hover:bg-slate-700 px-6 py-2 rounded-full font-bold transition duration-300 border border-slate-700 text-slate-400">3º Trimestre</button>
                <button onclick="abrirTrimestre(event, 't4')" class="tab-link bg-[#1e293b] hover:bg-slate-700 px-6 py-2 rounded-full font-bold transition duration-300 border border-slate-700 text-slate-400">4º Trimestre</button>
            </div>

            <!-- Conteúdo do 1º Trimestre -->
            <div id="t1" class="trimestre-content block animate-fadeIn">
                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4 max-w-6xl mx-auto mb-6">
                    
                    <!-- Lição 01 - PDF (COM SEU LINK DO MEGA) -->
                    <a href="https://mega.nz/file/YlRUXRRT#LilmblwTls6NUMGPOdn2kvpvB-OEfGJPHvoyzUHVoEo" target="_blank" class="bg-[#1e293b] border border-slate-700 p-4 rounded-xl hover:border-sky-500 transition flex items-center justify-center gap-3 shadow-lg">
                        <i class="fas fa-file-pdf text-red-500 text-xl"></i> 
                        <span class="font-semibold">Lição 01 (PDF)</span>
                    </a>

                    <!-- Lição 01 - PPT -->
                    <a href="#" target="_blank" class="bg-[#1e293b] border border-slate-700 p-4 rounded-xl hover:border-sky-500 transition flex items-center justify-center gap-3 shadow-lg">
                        <i class="fas fa-file-powerpoint text-orange-500 text-xl"></i> 
                        <span class="font-semibold">Lição 01 (PPT)</span>
                    </a>

                    <!-- Lição 02 - PDF -->
                    <a href="#" target="_blank" class="bg-[#1e293b] border border-slate-700 p-4 rounded-xl hover:border-sky-500 transition flex items-center justify-center gap-3 shadow-lg">
                        <i class="fas fa-file-pdf text-red-500 text-xl"></i> 
                        <span class="font-semibold text-slate-500 italic">Lição 02 (PDF)</span>
                    </a>

                    <!-- Lição 02 - PPT -->
                    <a href="#" target="_blank" class="bg-[#1e293b] border border-slate-700 p-4 rounded-xl hover:border-sky-500 transition flex items-center justify-center gap-3 shadow-lg">
                        <i class="fas fa-file-powerpoint text-orange-500 text-xl"></i> 
                        <span class="font-semibold text-slate-500 italic">Lição 02 (PPT)</span>
                    </a>
                </div>

                <!-- Grid Extra (Escondido) -->
                <div id="maisLicoes" class="hidden grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4 max-w-6xl mx-auto animate-fadeIn">
                    <p class="col-span-full py-10 text-slate-500 italic">Novas lições serão adicionadas semanalmente.</p>
                </div>

                <button onclick="toggleLicoes()" id="btnVerMais" class="mt-10 bg-transparent border-2 border-sky-600 text-sky-400 hover:bg-sky-600 hover:text-white px-8 py-3 rounded-full font-bold transition flex items-center gap-2 mx-auto">
                    <span id="txtBotao">Ver Lições Anteriores</span>
                    <i id="iconeBotao" class="fas fa-chevron-down text-xs"></i>
                </button>
            </div>

            <!-- Conteúdos Futuros -->
            <div id="t2" class="trimestre-content hidden animate-fadeIn py-10">
                <p class="text-slate-500 italic">Materiais sendo preparados para Abril.</p>
            </div>
            <div id="t3" class="trimestre-content hidden animate-fadeIn py-10">
                <p class="text-slate-500 italic">Disponível em breve.</p>
            </div>
            <div id="t4" class="trimestre-content hidden animate-fadeIn py-10">
                <p class="text-slate-500 italic">Disponível em breve.</p>
            </div>
        </div>
    </section>

    <!-- DINÂMICAS -->
    <section id="dinamicas" class="bg-white py-24">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16">
                <h3 class="text-3xl font-bold text-slate-900">Dinâmicas Criativas</h3>
                <div class="w-16 h-1 bg-sky-500 mx-auto mt-4 rounded-full"></div>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 max-w-6xl mx-auto">
                <!-- Card Dinâmica 01 -->
                <div class="bg-slate-50 rounded-3xl p-8 border border-slate-200 shadow-sm hover:shadow-xl transition-all duration-300">
                    <span class="bg-amber-100 text-amber-700 text-xs font-bold px-3 py-1 rounded-full uppercase mb-4 inline-block">Quebra-gelo</span>
                    <h4 class="text-2xl font-bold text-slate-800 mb-4">O Presente Misterioso</h4>
                    <p class="text-slate-600 mb-6 text-sm leading-relaxed">Uma atividade para introduzir o tema da lição e despertar a curiosidade dos alunos.</p>
                    <button onclick="verDetalhes('din01')" class="w-full bg-sky-600 text-white py-3 rounded-xl font-bold hover:bg-sky-700 transition">Ver Passo a Passo</button>
                    <div id="din01" class="hidden mt-6 p-4 bg-sky-50 rounded-xl border-l-4 border-sky-500 text-sm text-slate-700 animate-fadeIn">
                        <strong>Instruções:</strong> Coloque um espelho dentro da caixa. Diga aos alunos que dentro está "A obra-prima de Deus". Deixe cada um olhar. No fim, leia Gênesis 1:27.
                    </div>
                </div>

                <!-- Card Dinâmica 02 -->
                <div class="bg-slate-50 rounded-3xl p-8 border border-slate-200 shadow-sm hover:shadow-xl transition-all duration-300">
                    <span class="bg-emerald-100 text-emerald-700 text-xs font-bold px-3 py-1 rounded-full uppercase mb-4 inline-block">Fixação</span>
                    <h4 class="text-2xl font-bold text-slate-800 mb-4">Mapa do Tesouro</h4>
                    <p class="text-slate-600 mb-6 text-sm leading-relaxed">Perfeito para revisar o conteúdo estudado e memorizar versículos chave no final da aula.</p>
                    <button onclick="verDetalhes('din02')" class="w-full bg-sky-600 text-white py-3 rounded-xl font-bold hover:bg-sky-700 transition">Ver Passo a Passo</button>
                    <div id="din02" class="hidden mt-6 p-4 bg-sky-50 rounded-xl border-l-4 border-sky-500 text-sm text-slate-700 animate-fadeIn">
                        <strong>Instruções:</strong> Esconda versículos pela sala. Divida em grupos e dê pistas bíblicas. O grupo que encontrar primeiro, ganha um brinde.
                    </div>
                </div>

                <!-- Em breve -->
                <div class="bg-slate-100 rounded-3xl p-8 border border-dashed border-slate-300 flex flex-col items-center justify-center text-center opacity-60">
                    <i class="fas fa-plus-circle text-slate-400 text-4xl mb-4"></i>
                    <p class="text-slate-500 font-bold uppercase tracking-widest text-xs italic">Mais em breve!</p>
                </div>
            </div>
        </div>
    </section>

    <!-- SOBRE -->
    <section id="sobre" class="bg-slate-50 py-24 border-t border-slate-200">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row items-center gap-16 max-w-6xl mx-auto text-balance text-center md:text-left">
                <div class="md:w-1/2 relative">
                    <div class="absolute -top-4 -left-4 w-64 h-64 bg-sky-100 rounded-3xl -z-10"></div>
                    <img src="https://images.unsplash.com/photo-1519791883288-dc8bd696e667?auto=format&fit=crop&w=800&q=80" alt="Sobre o Mestre" class="rounded-3xl shadow-2xl w-full max-w-md mx-auto">
                </div>
                <div class="md:w-1/2">
                    <h3 class="text-sky-600 font-bold uppercase tracking-widest text-sm mb-4 italic">Nossa Missão</h3>
                    <h3 class="text-4xl font-bold text-slate-900 mb-6">Equipando Vocacionados</h3>
                    <p class="text-slate-600 text-lg mb-6 leading-relaxed">
                        Este site nasceu do desejo de servir à igreja local. Nosso objetivo é simplificar seu preparo para que você foque no ensino da Verdade através das **Lições PECC**.
                    </p>
                    <div class="bg-white p-6 rounded-2xl border-l-8 border-sky-500 shadow-sm italic text-slate-800 text-lg">
                        "Ensinando-os a guardar todas as coisas que eu vos tenho mandado..." <span class="block mt-2 font-bold text-sky-600 text-sm not-italic">— Mateus 28:20</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CONTATO -->
    <section id="contato" class="bg-sky-50 py-24">
        <div class="container mx-auto px-4 max-w-3xl">
            <div class="bg-white p-10 rounded-3xl shadow-2xl border border-sky-100">
                <h3 class="text-3xl font-bold text-center mb-8 text-slate-900 leading-tight">Sugestões ou Dúvidas? <br><span class="text-sky-600 text-xl font-normal tracking-wide italic">Mande uma mensagem</span></h3>
                <form class="space-y-6">
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-6 text-sm">
                        <input type="text" placeholder="Seu Nome" class="w-full p-4 rounded-xl bg-slate-50 border border-slate-200 focus:ring-2 focus:ring-sky-500 transition outline-none">
                        <input type="email" placeholder="Seu E-mail" class="w-full p-4 rounded-xl bg-slate-50 border border-slate-200 focus:ring-2 focus:ring-sky-500 transition outline-none">
                    </div>
                    <textarea placeholder="Como posso te ajudar?" class="w-full p-4 rounded-xl bg-slate-50 border border-slate-200 h-32 focus:ring-2 focus:ring-sky-500 transition outline-none text-sm"></textarea>
                    <button class="w-full bg-sky-600 hover:bg-sky-700 text-white py-4 rounded-xl font-bold text-lg shadow-xl shadow-sky-200 transition duration-300">Enviar para o Portal</button>
                </form>
            </div>
        </div>
    </section>

    <!-- RODAPÉ -->
    <footer class="bg-slate-950 text-slate-400 py-16 border-t-4 border-sky-600">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-12 max-w-6xl mx-auto">
                <div>
                    <h4 class="text-2xl font-bold text-white mb-4 italic tracking-tighter">Mestre<span class="text-sky-400 font-bold">EBD</span></h4>
                    <p class="text-sm leading-relaxed mb-6">Equipando professores da Escola Bíblica com materiais práticos fundamentados na Palavra de Deus.</p>
                    <div class="flex gap-4">
                        <a href="#" class="w-10 h-10 bg-slate-800 rounded-full flex items-center justify-center hover:bg-sky-600 hover:text-white transition"><i class="fab fa-instagram"></i></a>
                        <a href="#" class="w-10 h-10 bg-slate-800 rounded-full flex items-center justify-center hover:bg-emerald-600 hover:text-white transition"><i class="fab fa-whatsapp"></i></a>
                    </div>
                </div>
                <div>
                    <h5 class="text-white font-bold uppercase tracking-widest text-xs mb-6 underline decoration-sky-500 decoration-2 underline-offset-8">Navegação</h5>
                    <ul class="space-y-3 text-sm">
                        <li><a href="#" class="hover:text-sky-400 transition">Início</a></li>
                        <li><a href="#downloads" class="hover:text-sky-400 transition">Downloads</a></li>
                        <li><a href="#dinamicas" class="hover:text-sky-400 transition">Dinâmicas</a></li>
                        <li><a href="#sobre" class="hover:text-sky-400 transition">Sobre</a></li>
                    </ul>
                </div>
                <div>
                    <h5 class="text-white font-bold uppercase tracking-widest text-xs mb-6 underline decoration-sky-500 decoration-2 underline-offset-8">Direitos Autorais</h5>
                    <p class="text-xs leading-relaxed italic">Este site oferece subsídios de apoio. Não substituímos as revistas originais da Editora Cristã Evangélica (PECC). Sempre adquira o material oficial.</p>
                </div>
                <div class="bg-slate-900 p-6 rounded-2xl border border-slate-800">
                    <p class="text-slate-300 italic text-sm mb-4">"Ide, portanto, fazei discípulos de todas as nações..."</p>
                    <span class="text-xs font-bold text-sky-400 uppercase tracking-widest">— Mateus 28:19</span>
                </div>
            </div>
            <div class="mt-16 pt-8 border-t border-slate-900 text-center">
                <p class="text-xs uppercase tracking-widest font-medium">© 2026 Portal MestreEBD. Feito para a glória de Deus.</p>
            </div>
        </div>
    </footer>

    <!-- SCRIPTS JAVASCRIPT -->
    <script>
        function abrirTrimestre(evt, trimestreId) {
            var i, tabcontent, tablinks;
            tabcontent = document.getElementsByClassName("trimestre-content");
            for (i = 0; i < tabcontent.length; i++) {
                tabcontent[i].classList.add("hidden");
                tabcontent[i].classList.remove("block");
            }
            tablinks = document.getElementsByClassName("tab-link");
            for (i = 0; i < tablinks.length; i++) {
                tablinks[i].classList.remove("bg-sky-600", "active");
                tablinks[i].classList.add("bg-[#1e293b]");
                tablinks[i].classList.add("text-slate-400");
            }
            document.getElementById(trimestreId).classList.remove("hidden");
            document.getElementById(trimestreId).classList.add("block");
            evt.currentTarget.classList.add("bg-sky-600", "active");
            evt.currentTarget.classList.remove("bg-[#1e293b]");
            evt.currentTarget.classList.remove("text-slate-400");
        }

        function toggleLicoes() {
            var listaExtra = document.getElementById("maisLicoes");
            var txtBotao = document.getElementById("txtBotao");
            var icone = document.getElementById("iconeBotao");
            if (listaExtra.classList.contains("hidden")) {
                listaExtra.classList.remove("hidden");
                txtBotao.innerText = "Recolher Lições";
                icone.classList.replace("fa-chevron-down", "fa-chevron-up");
            } else {
                listaExtra.classList.add("hidden");
                txtBotao.innerText = "Ver Lições Anteriores";
                icone.classList.replace("fa-chevron-up", "fa-chevron-down");
            }
        }

        function verDetalhes(id) {
            var dinamica = document.getElementById(id);
            dinamica.classList.toggle("hidden");
        }
    </script>

</body>
</html>
