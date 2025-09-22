<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tutorial: Como Colocar seu Site Online</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Arial, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            padding: 20px;
            color: #333;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: white;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            overflow: hidden;
        }
        
        header {
            background: #2c3e50;
            color: white;
            padding: 30px;
            text-align: center;
        }
        
        h1 {
            margin-bottom: 10px;
            font-size: 2.5rem;
        }
        
        .subtitle {
            font-size: 1.3rem;
            opacity: 0.9;
        }
        
        .methods {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            padding: 30px;
        }
        
        .method-card {
            background: #f8f9fa;
            border-radius: 10px;
            padding: 25px;
            border: 2px solid #e9ecef;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .method-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .method-card.recommended {
            border-color: #27ae60;
            background: #f0fff4;
        }
        
        .method-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
        }
        
        .method-title {
            font-size: 1.4rem;
            color: #2c3e50;
            font-weight: bold;
        }
        
        .method-badge {
            background: #3498db;
            color: white;
            padding: 5px 10px;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: bold;
        }
        
        .recommended .method-badge {
            background: #27ae60;
        }
        
        .method-features {
            list-style: none;
            margin: 15px 0;
        }
        
        .method-features li {
            padding: 8px 0;
            border-bottom: 1px solid #eee;
            display: flex;
            align-items: center;
        }
        
        .method-features li:before {
            content: "✓";
            color: #27ae60;
            font-weight: bold;
            margin-right: 10px;
        }
        
        .method-steps {
            background: white;
            padding: 15px;
            border-radius: 8px;
            margin: 15px 0;
            border-left: 4px solid #3498db;
        }
        
        .step {
            margin-bottom: 10px;
            padding-left: 20px;
            position: relative;
        }
        
        .step:before {
            content: "•";
            color: #3498db;
            font-weight: bold;
            position: absolute;
            left: 0;
        }
        
        .method-link {
            display: block;
            text-align: center;
            background: #3498db;
            color: white;
            padding: 12px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            margin-top: 15px;
            transition: background 0.3s;
        }
        
        .method-link:hover {
            background: #2980b9;
        }
        
        .comparison {
            padding: 30px;
            background: #f8f9fa;
        }
        
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }
        
        th, td {
            padding: 15px;
            text-align: left;
            border-bottom: 1px solid #ddd;
        }
        
        th {
            background: #2c3e50;
            color: white;
        }
        
        tr:hover {
            background: #f1f1f1;
        }
        
        .price-free {
            color: #27ae60;
            font-weight: bold;
        }
        
        .price-paid {
            color: #e74c3c;
        }
        
        footer {
            text-align: center;
            padding: 20px;
            background: #2c3e50;
            color: white;
        }
        
        @media (max-width: 768px) {
            .methods {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>🌐 Como Colocar seu Site Online</h1>
            <div class="subtitle">4 Métodos Simples - Do Gratuito ao Profissional</div>
        </header>
        
        <div class="methods">
            <!-- Método 1 - GitHub Pages -->
            <div class="method-card recommended">
                <div class="method-header">
                    <div class="method-title">GitHub Pages</div>
                    <div class="method-badge">RECOMENDADO</div>
                </div>
                <p>Perfect para iniciantes - totalmente gratuito</p>
                
                <ul class="method-features">
                    <li>100% Gratuito</li>
                    <li>Fácil de usar</li>
                    <li>Domínio personalizado (opcional)</li>
                    <li>Ideal para portfólios e projetos</li>
                </ul>
                
                <div class="method-steps">
                    <div class="step">Crie conta no GitHub</div>
                    <div class="step">Repositório: usuario.github.io</div>
                    <div class="step">Upload do arquivo HTML</div>
                    <div class="step">Pronto! Site no ar</div>
                </div>
                
                <a href="https://github.com" class="method-link" target="_blank">Criar Conta GitHub</a>
            </div>
            
            <!-- Método 2 - Netlify -->
            <div class="method-card">
                <div class="method-header">
                    <div class="method-title">Netlify</div>
                    <div class="method-badge">FÁCIL</div>
                </div>
                <p>Deploy com arrastar e soltar</p>
                
                <ul class="method-features">
                    <li>Plano gratuito generoso</li>
                    <li>Deploy contínuo automático</li>
                    <li>SSL gratuito</li>
                    <li>Ótimo para projetos simples</li>
                </ul>
                
                <div class="method-steps">
                    <div class="step">Faça login no Netlify</div>
                    <div class="step">Arraste a pasta do site</div>
                    <div class="step">URL gerada automaticamente</div>
                    <div class="step">Personalize se quiser</div>
                </div>
                
                <a href="https://netlify.com" class="method-link" target="_blank">Acessar Netlify</a>
            </div>
            
            <!-- Método 3 - Vercel -->
            <div class="method-card">
                <div class="method-header">
                    <div class="method-title">Vercel</div>
                    <div class="method-badge">RÁPIDO</div>
                </div>
                <p>Especializado em projetos web</p>
                
                <ul class="method-features">
                    <li>Deploy instantâneo</li>
                    <li>Integração com GitHub</li>
                    <li>Performance otimizada</li>
                    <li>Ótimo para desenvolvedores</li>
                </ul>
                
                <div class="method-steps">
                    <div class="step">Conecte com GitHub</div>
                    <div class="step">Importe o repositório</div>
                    <div class="step">Deploy automático</div>
                    <div class="step">Site pronto em segundos</div>
                </div>
                
                <a href="https://vercel.com" class="method-link" target="_blank">Experimentar Vercel</a>
            </div>
        </div>
        
        <div class="comparison">
            <h2>📊 Comparação Detalhada</h2>
            <table>
                <thead>
                    <tr>
                        <th>Característica</th>
                        <th>GitHub Pages</th>
                        <th>Netlify</th>
                        <th>Vercel</th>
                        <th>Hospedagem Paga</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Custo</td>
                        <td class="price-free">Grátis</td>
                        <td class="price-free">Grátis</td>
                        <td class="price-free">Grátis</td>
                        <td class="price-paid">R$ 10-50/mês</td>
                    </tr>
                    <tr>
                        <td>Domínio Próprio</td>
                        <td>✓ (gratuito)</td>
                        <td>✓ (gratuito)</td>
                        <td>✓ (gratuito)</td>
                        <td>✓ (pago)</td>
                    </tr>
                    <tr>
                        <td>SSL/HTTPS</td>
                        <td>✓</td>
                        <td>✓</td>
                        <td>✓</td>
                        <td>✓</td>
                    </tr>
                    <tr>
                        <td>Fácil de Usar</td>
                        <td>⭐⭐⭐⭐⭐</td>
                        <td>⭐⭐⭐⭐⭐</td>
                        <td>⭐⭐⭐⭐</td>
                        <td>⭐⭐⭐</td>
                    </tr>
                    <tr>
                        <td>Indicado Para</td>
                        <td>Iniciantes</td>
                        <td>Projetos simples</td>
                        <td>Desenvolvedores</td>
                        <td>Negócios</td>
                    </tr>
                </tbody>
            </table>
        </div>
        
        <div style="padding: 30px; text-align: center;">
            <h2>🚀 Próximos Passos Recomendados</h2>
            <p style="margin: 20px 0; font-size: 1.2rem;">
                <strong>1. Comece com GitHub Pages</strong> - É o mais simples e atende perfeitamente suas necessidades<br>
                <strong>2. Depois evolua</strong> conforme seu projeto crescer
            </p>
            <a href="#github-tutorial" style="background: #27ae60; color: white; padding: 15px 30px; 
               text-decoration: none; border-radius: 5px; font-weight: bold; display: inline-block; 
               margin: 10px;">Ver Tutorial Passo a Passo do GitHub</a>
        </div>
        
        <footer>
            <p>💡 <strong>Dica:</strong> Recomendo começar com GitHub Pages - é grátis e suficiente para seu projeto!</p>
            <p style="margin-top: 10px; font-size: 0.9rem;">Se tiver dúvidas em algum passo, me avise que eu te ajudo!</p>
        </footer>
    </div>

    <script>
        // Simulação de interações
        document.querySelectorAll('.method-link').forEach(link => {
            link.addEventListener('click', function(e) {
                e.preventDefault();
                const service = this.closest('.method-card').querySelector('.method-title').textContent;
                alert(`Em um cenário real, você seria redirecionado para o site do ${service}`);
            });
        });
    </script>
</body>
</html>
