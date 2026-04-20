<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Recife store| loja Discord</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css"/>
    <link rel="icon" href="https://cdn.discordapp.com/attachments/1360065809858298080/1495700622736101518/Logo_Recife.png">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;700;900&display=swap');
        
        body {
            background-color: #050505;
            color: #ffffff;
            font-family: 'Inter', sans-serif;
            overflow-x: hidden;
        }

        .glass-card {
            background: rgba(255, 255, 255, 0.03);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.05);
            transition: all 0.3s ease;
        }

        .glass-card:hover {
            border-color: rgba(255, 255, 255, 0.2);
            transform: translateY(-5px);
        }

        .btn-primary {
            background: #ffffff;
            color: #000000;
            font-weight: bold;
            transition: all 0.3s ease;
        }

        .btn-primary:hover {
            background: #e0e0e0;
            box-shadow: 0 0 20px rgba(255,255,255,0.2);
        }

        .nav-link {
            position: relative;
            opacity: 0.7;
            transition: 0.3s;
        }

        .nav-link:hover, .nav-link.active {
            opacity: 1;
        }

        .nav-link.active::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 100%;
            height: 2px;
            background: white;
        }

        .notification {
            position: fixed;
            bottom: 20px;
            right: 20px;
            padding: 15px 25px;
            border-radius: 8px;
            background: #111;
            border-left: 4px solid #fff;
            z-index: 1000;
            animation: slideInRight 0.5s ease forwards;
        }

        @keyframes slideInRight {
            from { transform: translateX(100%); }
            to { transform: translateX(0); }
        }
    </style>
</head>
<body>

    <nav class="fixed w-full z-50 py-6 px-8 flex justify-between items-center bg-black/50 backdrop-blur-md border-b border-white/5">
        <div class="flex items-center gap-3">
            <img src="https://cdn.discordapp.com/attachments/1486475883047944354/1486736756521828522/9701372e88ed9a9793c004dc0c4435a4.png" class="w-10 h-10 rounded-full border border-white/20">
            <span class="font-black text-xl tracking-tighter">RECIFE ROLEPLAY</span>
        </div>
        <div class="hidden md:flex gap-8 text-sm font-medium">
            <button onclick="showPage('inicio')" class="nav-link active" id="btn-inicio">🏠 Início</button>
            <button onclick="showPage('galeria')" class="nav-link" id="btn-galeria">🛒 Produtos</button>
            <button onclick="showPage('avaliar')" class="nav-link" id="btn-avaliar">⭐ Avaliar</button>
            <button onclick="showPage('creditos')" class="nav-link" id="btn-creditos">🛡️ Suporte</button>
        </div>
        <button id="discordLoginBtn" class="glass-card px-5 py-2 rounded-full text-xs font-bold border border-white/10 hover:bg-white hover:text-black transition">
            🔌 ENTRAR COM DISCORD
        </button>
    </nav>

    <main class="pt-32 px-6 max-w-6xl mx-auto pb-20">

        <section id="page-inicio" class="animate__animated animate__fadeIn">
            <div class="relative w-full h-64 md:h-80 rounded-3xl overflow-hidden mb-12 glass-card">
                <img src="https://media.discordapp.net/attachments/1486475883047944354/1486736755750338570/dark_bot.png" class="w-full h-full object-cover opacity-40">
                <div class="absolute inset-0 bg-gradient-to-t from-black to-transparent"></div>
                <div class="absolute bottom-10 left-10">
                    <h1 class="text-5xl md:text-7xl font-black mb-2 tracking-tighter">Recife Store</h1>
                    <p class="text-gray-400 max-w-md">Premium Discord Services. Qualidade, rapidez e o melhor preço do mercado.</p>
                </div>
            </div>

            <div class="grid md:grid-cols-2 gap-8 items-center mb-16">
                <div class="glass-card p-10 rounded-3xl">
                    <h2 class="text-3xl font-bold mb-4">Sobre Nós 🌴</h2>
                    <p class="text-gray-400 leading-relaxed mb-6">
                        Recife Store é uma fornecedora do Discord criado por Gui, focado em preços acessíveis, confiança e entrega rápida. Elevamos o nível do seu servidor com produtos selecionados e suporte dedicado.
                    </p>
                    <div class="flex gap-4">
                        <a href="https://discord.gg/kQa2DWhKwB" target="_blank" class="btn-primary px-8 py-3 rounded-xl flex items-center gap-2">
                           💬 Discord
                        </a>
                        <button onclick="showPage('avaliar')" class="glass-card px-8 py-3 rounded-xl">
                           ⭐ Avaliações
                        </button>
                    </div>
                </div>
             
<div class="grid grid-cols-2 gap-4">

    <div class="glass-card p-6 rounded-2xl text-center">
        <span class="block text-3xl mb-2">⚡</span>
        <h3 class="font-bold">VIP SUPREMO</h3>
        <p class="text-gray-400 text-sm">Acesso completo e vantagens exclusivas.</p>
    </div>

    <div class="glass-card p-6 rounded-2xl text-center">
        <span class="block text-3xl mb-2">💎</span>
        <h3 class="font-bold">VIP DIAMANTE</h3>
        <p class="text-gray-400 text-sm">Benefícios premium e destaque no servidor.</p>
    </div>

    <div class="glass-card p-6 rounded-2xl text-center">
        <span class="block text-3xl mb-2">🥈</span>
        <h3 class="font-bold">VIP PRATA</h3>
        <p class="text-gray-400 text-sm">Recursos básicos com vantagens especiais.</p>
    </div>

    <div class="glass-card p-6 rounded-2xl text-center">
        <span class="block text-3xl mb-2">🛡️</span>
        <h3 class="font-bold">VIP PROTEÇÃO</h3>
        <p class="text-gray-400 text-sm">Segurança extra e benefícios exclusivos.</p>
    </div>

    <div class="glass-card p-6 rounded-2xl text-center">
        <span class="block text-3xl mb-2">🔥</span>
        <h3 class="font-bold">VIP</h3>
        <p class="text-gray-400 text-sm">Melhoria no servidor e vantagens normais.</p>
    </div>

    <div class="glass-card p-6 rounded-2xl text-center">
        <span class="block text-3xl mb-2">🚗</span>
        <h3 class="font-bold">Skyline</h3>
        <p class="text-gray-400 text-sm">Experiência máxima dentro do servidor.</p>
    </div>

</div>
               
                </div>
            </div>
        </section>

<button onclick="showPage('pix')" class="nav-link" id="btn-pix">💳 Pix</button>

        <section id="page-galeria" class="hidden animate__animated animate__fadeIn">
    
    <h2 class="text-4xl font-black mb-10 text-center uppercase tracking-widest">
        🗃️ Produtos da cidade Recife
    </h2>

    <div class="grid grid-cols-2 md:grid-cols-3 gap-4">

        <!-- PRODUTO 1 -->
        <div class="glass-card p-6 rounded-2xl text-center">
            <span class="block text-3xl mb-2">🚙</span>
            <h3 class="font-bold">VIP NORMAL</h3>
            <p class="text-green-400 text-sm">R$ 10,00</p>
            <button onclick="showPage('pix')" class="btn-primary px-4 py-1 text-xs mt-2 rounded-lg">
                Comprar
            </button>
        </div>

        <!-- PRODUTO 2 -->
        <div class="glass-card p-6 rounded-2xl text-center">
            <span class="block text-3xl mb-2">🥈</span>
            <h3 class="font-bold">VIP PRATA</h3>
            <p class="text-green-400 text-sm">R$ 15,00</p>
            <button onclick="showPage('pix')" class="btn-primary px-4 py-1 text-xs mt-2 rounded-lg">
                Comprar
            </button>
        </div>

        <!-- PRODUTO 3 -->
        <div class="glass-card p-6 rounded-2xl text-center">
            <span class="block text-3xl mb-2">🚗</span>
            <h3 class="font-bold">skyline</h3>
            <p class="text-green-400 text-sm">R$ 15,00</p>
            <button onclick="showPage('pix')" class="btn-primary px-4 py-1 text-xs mt-2 rounded-lg">
                Comprar
            </button>
        </div>

        <!-- PRODUTO 4 -->
        <div class="glass-card p-6 rounded-2xl text-center">
            <span class="block text-3xl mb-2">💎</span>
            <h3 class="font-bold">VIP DIAMANTE </h3>
            <p class="text-green-400 text-sm">R$ 20,00</p>
            <button onclick="showPage('pix')" class="btn-primary px-4 py-1 text-xs mt-2 rounded-lg">
                Comprar
            </button>
        </div>

    </div>

</section>
                </div>
        </section>

<<section id="page-pix" class="hidden animate__animated animate__fadeIn text-center">
    <div class="glass-card p-10 rounded-3xl max-w-xl mx-auto">
        <h2 class="text-3xl font-black mb-6">💳 Pagamento via Pix</h2>    <p class="text-gray-400 mb-6">
        Clique no botão abaixo para ver a chave Pix e realizar o pagamento.
    </p>

    <button onclick="mostrarPix()" class="btn-primary px-8 py-4 rounded-xl font-bold">
        Ver pagamento
    </button>

    <div id="pixBox" class="mt-6 hidden animate__animated">

        <!-- QR -->
        <img src="90d290c1-843a-4001-b5bc-238b266533a0" class="mx-auto mb-4 rounded-xl" width="200">

        <p class="text-gray-300 mb-2">Ou copie a chave Pix:</p>

        <!-- CHAVE -->
        <p id="chavePix" class="bg-white/5 p-4 rounded-xl break-all">
            90d290c1-843a-4001-b5bc-238b266533a0
        </p>

        <!-- BOTÕES LADO A LADO -->
        <div class="flex justify-center gap-3 mt-4">

            <!-- COPIAR -->
            <button onclick="copiarPix()" 
                class="px-6 py-2 bg-green-500 rounded-lg font-bold">
                📋 Copiar
            </button>

            <!-- DISCORD -->
            <a href="https://discord.gg/kQa2DWhKwB" target="_blank"
               class="px-6 py-2 bg-blue-500 rounded-lg font-bold inline-block">
               💬 Discord
            </a>

        </div>

    </div>
</div>

</section><script>
function mostrarPix() {
    const box = document.getElementById("pixBox");
    box.classList.remove("hidden");
    box.classList.add("animate__fadeIn");
}

function copiarPix() {
    const chave = document.getElementById("chavePix").innerText;
    navigator.clipboard.writeText(chave);

    alert("Chave Pix copiada!");
}
</script>

<script>
function mostrarPix() {
    document.getElementById("pixBox").classList.remove("hidden");
}

function copiarPix() {
    const chave = document.getElementById("chavePix").innerText;
    navigator.clipboard.writeText(chave);
    alert("Chave Pix copiada!");
}
</script>
    </div>
</section>

        <section id="page-avaliar" class="hidden animate__animated animate__fadeIn">
            <div class="max-w-2xl mx-auto glass-card p-10 rounded-3xl">
                <h2 class="text-3xl font-black mb-6 flex items-center gap-3">📝 Deixe sua Avaliação</h2>
                <form id="feedbackForm" class="space-y-6">
                    <div>
                        <label class="block text-xs uppercase font-bold text-gray-500 mb-2">Seu Nome / Discord</label>
                        <input type="text" id="fb-name" required class="w-full bg-white/5 border border-white/10 rounded-xl p-4 focus:outline-none focus:border-white transition" placeholder="Ex: Noah#0001">
                    </div>
                    <div>
                        <label class="block text-xs uppercase font-bold text-gray-500 mb-2">Nota (1 a 5)</label>
                        <select id="fb-stars" class="w-full bg-white/5 border border-white/10 rounded-xl p-4 focus:outline-none focus:border-white transition appearance-none">
                            <option value="5" class="bg-black">⭐⭐⭐⭐⭐ - Excelente</option>
                            <option value="4" class="bg-black">⭐⭐⭐⭐ - Muito Bom</option>
                            <option value="3" class="bg-black">⭐⭐⭐ - Regular</option>
                            <option value="2" class="bg-black">⭐⭐ - Ruim</option>
                            <option value="1" class="bg-black">⭐ - Péssimo</option>
                        </select>
                    </div>
                    <div>
                        <label class="block text-xs uppercase font-bold text-gray-500 mb-2">Comentário</label>
                        <textarea id="fb-comment" required rows="4" class="w-full bg-white/5 border border-white/10 rounded-xl p-4 focus:outline-none focus:border-white transition" placeholder="Conte como foi sua experiência..."></textarea>
                    </div>
                    <button type="submit" class="btn-primary w-full py-4 rounded-xl font-black uppercase tracking-widest">Enviar Avaliação</button>
                </form>
            </div>
        </section>

        <section id="page-creditos" class="hidden animate__animated animate__fadeIn text-center">
            <div class="glass-card p-12 rounded-3xl inline-block">
                <img src="https://cdn.discordapp.com/attachments/1486475883047944354/1486736756521828522/9701372e88ed9a9793c004dc0c4435a4.png" class="w-24 h-24 rounded-full mx-auto mb-6 border-2 border-white">
                <h2 class="text-3xl font-black mb-2">PROJETO RECIFE</h2>
                <p class="text-gray-400 mb-8 uppercase tracking-widest text-sm">Desenvolvido por <span class="text-white font-bold">Gui</span></p>
                <div class="grid grid-cols-1 gap-4 max-w-xs mx-auto">
                    <a href="https://discord.gg/kQa2DWhKwB" class="glass-card py-3 rounded-lg hover:bg-white hover:text-black">🎫 Abrir Ticket</a>
                    <a href="#" class="glass-card py-3 rounded-lg hover:bg-white hover:text-black">🤝 Parceria</a>
                </div>
            </div>
        </section>

    </main>

    <script>
        // SISTEMA DE NAVEGAÇÃO
        function showPage(pageId) {
            document.querySelectorAll('section').forEach(s => s.classList.add('hidden'));
            document.querySelectorAll('.nav-link').forEach(l => l.classList.remove('active'));
            
            document.getElementById('page-' + pageId).classList.remove('hidden');
            document.getElementById('btn-' + pageId).classList.add('active');
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        // NOTIFICAÇÕES CUSTOMIZADAS
        function notify(msg) {
            const toast = document.createElement('div');
            toast.className = 'notification';
            toast.innerHTML = `🏁 ${msg}`;
            document.body.appendChild(toast);
            setTimeout(() => { toast.style.opacity = '0'; setTimeout(() => toast.remove(), 500); }, 3000);
        }

        // ANTI-SPAM & WEBHOOK
        const WEBHOOK_URL = "https://discord.com/api/webhooks/1495696976145154168/peJ-H5QrPIvOYGvn88hvTtMqRAuSVj_svPFfHeb2ngv9fv4S_tJTf2y-DDERAPC3w1G2";
        let lastSubmit = 0;

        document.getElementById('feedbackForm').addEventListener('submit', async (e) => {
            e.preventDefault();
            
            const now = Date.now();
            if (now - lastSubmit < 60000) {
                return notify("Aguarde 1 minuto para enviar outra avaliação.");
            }

            const data = {
                embeds: [{
                    title: "⭐ Nova Avaliação - Recife Store",
                    color: 0,
                    fields: [
                        { name: "👤 Cliente", value: document.getElementById('fb-name').value, inline: true },
                        { name: "⭐ Nota", value: document.getElementById('fb-stars').value + "/5", inline: true },
                        { name: "💬 Comentário", value: document.getElementById('fb-comment').value },
                        { name: "📅 Data", value: new Date().toLocaleString() }
                    ],
                    thumbnail: { url: "https://cdn.discordapp.com/attachments/1360065809858298080/1495700622736101518/Logo_Recife.png" }
                }]
            };

            try {
                const response = await fetch(WEBHOOK_URL, {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify(data)
                });

                if (response.ok) {
                    notify("Avaliação enviada com sucesso!");
                    lastSubmit = now;
                    document.getElementById('feedbackForm').reset();
                }
            } catch (err) {
                notify("Erro ao enviar avaliação.");
            }
        });

        // SIMULAÇÃO LOGIN DISCORD (SEGURANÇA EXTREMA)
        document.getElementById('discordLoginBtn').addEventListener('click', () => {
            // Em um ambiente real, você redirecionaria para a URL de OAuth2 do Discord.
            // Aqui simulamos a notificação de sucesso.
            notify("Login com Discord simulado!");
            
            // WEBHOOK ADMIN LOGIN
            const ADMIN_WEBHOOK = "https://discord.com/api/webhooks/1495696976145154168/peJ-H5QrPIvOYGvn88hvTtMqRAuSVj_svPFfHeb2ngv9fv4S_tJTf2y-DDERAPC3w1G2";
            fetch(ADMIN_WEBHOOK, {
                method: 'POST',
                headers: { 'Content-Type': 'application/json' },
                body: JSON.stringify({
                    content: "📢 **Novo Acesso ao Site:** usuário novo"
                })
            });
        });
    </script>

<!-- MODAL COMPRA -->
<div id="buyModal" class="fixed inset-0 bg-black/80 hidden items-center justify-center z-50">
    <div class="glass-card p-8 rounded-2xl max-w-md w-full text-center relative">
        
        <button onclick="closeModal()" class="absolute top-3 right-3 text-white text-xl">✖</button>

        <h2 class="text-2xl font-bold mb-4">Finalizar Compra 💳</h2>
        
        <p class="text-gray-400 mb-4">Produto selecionado:</p>
        <h3 id="productName" class="text-xl font-bold mb-6"></h3>

        <div class="bg-black/50 p-4 rounded-xl mb-4">
            <p class="text-sm text-gray-400 mb-2">Chave Pix:</p>
            <p id="pixKey" class="font-bold break-all">SUA_CHAVE_PIX_AQUI</p>
        </div>

function mostrarPix() {
    const box = document.getElementById('pixBox');
    box.classList.toggle('hidden');
}

        <button onclick="copyPix()" class="btn-primary w-full py-3 rounded-xl">
            📋 Copiar chave Pix
        </button>
    </div>
</div>
</body>
</html>
