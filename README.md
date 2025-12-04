<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rifa iPhone 16 Pro - 2000 números a R$15</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f5f7fa;
            color: #333;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        header {
            background: linear-gradient(135deg, #1a2a6c, #2a3a8c);
            color: white;
            padding: 30px 20px;
            text-align: center;
            border-radius: 0 0 20px 20px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            margin-bottom: 30px;
        }
        
        .logo {
            font-size: 2.8rem;
            margin-bottom: 10px;
            color: #4fc3f7;
        }
        
        h1 {
            font-size: 2.2rem;
            margin-bottom: 10px;
        }
        
        .subtitle {
            font-size: 1.2rem;
            opacity: 0.9;
            max-width: 800px;
            margin: 0 auto;
        }
        
        .highlight {
            color: #ffeb3b;
            font-weight: bold;
        }
        
        .main-content {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            margin-bottom: 40px;
        }
        
        .product-section {
            flex: 1;
            min-width: 300px;
            background: white;
            border-radius: 15px;
            padding: 25px;
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.08);
        }
        
        .product-image {
            width: 100%;
            height: 300px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 20px;
            position: relative;
            overflow: hidden;
        }
        
        .product-image img {
            max-width: 80%;
            filter: drop-shadow(0 10px 15px rgba(0, 0, 0, 0.3));
            transition: transform 0.5s;
        }
        
        .product-image:hover img {
            transform: scale(1.05);
        }
        
        .product-info h2 {
            color: #1a2a6c;
            margin-bottom: 15px;
            font-size: 1.8rem;
        }
        
        .product-specs {
            list-style-type: none;
            margin-bottom: 20px;
        }
        
        .product-specs li {
            padding: 8px 0;
            border-bottom: 1px dashed #eee;
        }
        
        .product-specs li:last-child {
            border-bottom: none;
        }
        
        .product-specs i {
            color: #4fc3f7;
            margin-right: 10px;
            width: 20px;
        }
        
        .rifa-section {
            flex: 1;
            min-width: 300px;
            background: white;
            border-radius: 15px;
            padding: 25px;
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.08);
        }
        
        .rifa-info {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 10px;
            margin-bottom: 25px;
            border-left: 5px solid #4fc3f7;
        }
        
        .rifa-details {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            margin-bottom: 20px;
        }
        
        .detail-item {
            text-align: center;
            padding: 15px;
            flex: 1;
            min-width: 150px;
        }
        
        .detail-item .number {
            font-size: 2.5rem;
            font-weight: bold;
            color: #1a2a6c;
        }
        
        .detail-item .label {
            font-size: 0.9rem;
            color: #666;
        }
        
        .numbers-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(50px, 1fr));
            gap: 8px;
            max-height: 300px;
            overflow-y: auto;
            padding: 10px;
            border: 1px solid #eee;
            border-radius: 8px;
            margin-bottom: 25px;
        }
        
        .number-box {
            height: 45px;
            display: flex;
            align-items: center;
            justify-content: center;
            background: #f0f4ff;
            border-radius: 5px;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.2s;
            border: 2px solid transparent;
        }
        
        .number-box:hover {
            background: #e1e8ff;
        }
        
        .number-box.selected {
            background: #4fc3f7;
            color: white;
            border-color: #1a2a6c;
        }
        
        .number-box.sold {
            background: #ffcdd2;
            color: #c62828;
            cursor: not-allowed;
        }
        
        .selected-numbers {
            margin-bottom: 20px;
            min-height: 60px;
            padding: 15px;
            background: #f8f9fa;
            border-radius: 10px;
        }
        
        .selected-numbers h3 {
            margin-bottom: 10px;
            color: #1a2a6c;
        }
        
        #selected-list {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }
        
        .selected-number {
            background: #4fc3f7;
            color: white;
            padding: 5px 10px;
            border-radius: 20px;
            font-weight: bold;
            display: flex;
            align-items: center;
        }
        
        .selected-number i {
            margin-left: 5px;
            cursor: pointer;
        }
        
        .total-price {
            font-size: 1.5rem;
            font-weight: bold;
            color: #1a2a6c;
            margin-bottom: 20px;
            text-align: center;
        }
        
        .buttons {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
        }
        
        button {
            flex: 1;
            padding: 16px;
            border: none;
            border-radius: 8px;
            font-size: 1.1rem;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s;
            min-width: 200px;
        }
        
        .buy-btn {
            background: linear-gradient(to right, #4fc3f7, #2196f3);
            color: white;
        }
        
        .buy-btn:hover {
            background: linear-gradient(to right, #2196f3, #1976d2);
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(33, 150, 243, 0.4);
        }
        
        .clear-btn {
            background: #f5f5f5;
            color: #666;
        }
        
        .clear-btn:hover {
            background: #e0e0e0;
        }
        
        footer {
            text-align: center;
            padding: 30px 20px;
            background: #1a2a6c;
            color: white;
            border-radius: 20px 20px 0 0;
            margin-top: 40px;
        }
        
        .contact-info {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 30px;
            margin-top: 20px;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .rules {
            background: white;
            border-radius: 15px;
            padding: 25px;
            margin-top: 30px;
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.08);
        }
        
        .rules h2 {
            color: #1a2a6c;
            margin-bottom: 15px;
        }
        
        .rules ul {
            padding-left: 20px;
        }
        
        .rules li {
            margin-bottom: 10px;
        }
        
        @media (max-width: 768px) {
            .main-content {
                flex-direction: column;
            }
            
            h1 {
                font-size: 1.8rem;
            }
            
            .detail-item {
                min-width: 120px;
            }
            
            button {
                min-width: 100%;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="logo">
                <i class="fas fa-ticket-alt"></i>
            </div>
            <h1>RIFA iPhone 16 Pro</h1>
            <p class="subtitle">Participe da rifa e concorra a um <span class="highlight">iPhone 16 Pro</span> novinho! São <span class="highlight">2000 números</span> disponíveis a apenas <span class="highlight">R$ 15,00 cada</span>.</p>
        </div>
    </header>
    
    <div class="container">
        <div class="main-content">
            <section class="product-section">
                <div class="product-image">
                    <!-- Imagem ilustrativa do iPhone 16 Pro -->
                    <i class="fas fa-mobile-alt" style="font-size: 12rem; color: white;"></i>
                </div>
                
                <div class="product-info">
                    <h2>iPhone 16 Pro - Prêmio Principal</h2>
                    <p>O mais novo lançamento da Apple com tecnologia de ponta e design inovador.</p>
                    
                    <ul class="product-specs">
                        <li><i class="fas fa-microchip"></i> Chip A18 Pro com Neural Engine</li>
                        <li><i class="fas fa-camera"></i> Sistema de câmera profissional de 48MP</li>
                        <li><i class="fas fa-expand-alt"></i> Tela Super Retina XDR de 6,7 polegadas</li>
                        <li><i class="fas fa-battery-full"></i> Bateria para até 28 horas de reprodução de vídeo</li>
                        <li><i class="fas fa-shield-alt"></i> Ceramic Shield e resistência à água IP68</li>
                        <li><i class="fas fa-palette"></i> Cores: Preto, Branco, Dourado e Azul</li>
                    </ul>
                    
                    <div class="rifa-info">
                        <p><i class="fas fa-info-circle"></i> <strong>Informações da Rifa:</strong> Serão sorteados 2000 números ao preço de R$ 15,00 cada. O sorteio será realizado quando todos os números forem vendidos.</p>
                    </div>
                </div>
            </section>
            
            <section class="rifa-section">
                <h2>Escolha seus números</h2>
                <p>Selecione os números que deseja comprar (R$ 15,00 cada).</p>
                
                <div class="rifa-details">
                    <div class="detail-item">
                        <div class="number">2000</div>
                        <div class="label">Números Totais</div>
                    </div>
                    <div class="detail-item">
                        <div class="number" id="available-count">1874</div>
                        <div class="label">Disponíveis</div>
                    </div>
                    <div class="detail-item">
                        <div class="number" id="sold-count">126</div>
                        <div class="label">Vendidos</div>
                    </div>
                </div>
                
                <div class="numbers-grid" id="numbers-grid">
                    <!-- Os números serão gerados via JavaScript -->
                </div>
                
                <div class="selected-numbers">
                    <h3>Seus números selecionados:</h3>
                    <div id="selected-list">
                        <!-- Números selecionados aparecerão aqui -->
                    </div>
                    <p id="no-selection" style="color: #999; font-style: italic;">Nenhum número selecionado ainda.</p>
                </div>
                
                <div class="total-price">
                    Total: R$ <span id="total-price">0</span>,00
                </div>
                
                <div class="buttons">
                    <button class="buy-btn" id="buy-btn">
                        <i class="fas fa-shopping-cart"></i> Comprar Números Selecionados
                    </button>
                    <button class="clear-btn" id="clear-btn">
                        <i class="fas fa-times"></i> Limpar Seleção
                    </button>
                </div>
            </section>
        </div>
        
        <div class="rules">
            <h2>Regras da Rifa</h2>
            <ul>
                <li>A rifa possui 2000 números no total, cada um ao valor de R$ 15,00.</li>
                <li>O sorteio será realizado mediante a venda de todos os números.</li>
                <li>O resultado será divulgado em nossas redes sociais e por e-mail para os participantes.</li>
                <li>O prêmio será entregue ao ganhador em até 30 dias após a confirmação do sorteio.</li>
                <li>O pagamento deve ser realizado via PIX, cartão de crédito ou boleto bancário.</li>
                <li>Em caso de dúvidas, entre em contato conosco pelos canais informados abaixo.</li>
            </ul>
        </div>
    </div>
    
    <footer>
        <div class="container">
            <h3>Entre em contato para mais informações</h3>
            <div class="contact-info">
                <div class="contact-item">
                    <i class="fab fa-whatsapp"></i>
                    <span>(11) 99999-9999</span>
                </div>
                <div class="contact-item">
                    <i class="fas fa-envelope"></i>
                    <span>contato@rifaiphone16.com</span>
                </div>
                <div class="contact-item">
                    <i class="fab fa-instagram"></i>
                    <span>@rifa_iphone16pro</span>
                </div>
            </div>
            <p style="margin-top: 20px; font-size: 0.9rem; opacity: 0.8;">© 2023 Rifa iPhone 16 Pro. Este site é apenas para fins ilustrativos.</p>
        </div>
    </footer>

    <script>
        // Gerar os 2000 números da rifa
        const totalNumbers = 2000;
        let selectedNumbers = [];
        let soldNumbers = [];
        
        // Inicializar alguns números como vendidos (apenas para demonstração)
        for (let i = 0; i < 126; i++) {
            soldNumbers.push(Math.floor(Math.random() * totalNumbers) + 1);
        }
        
        // Remover duplicatas
        soldNumbers = [...new Set(soldNumbers)];
        
        // Atualizar contagem de vendidos
        document.getElementById('sold-count').textContent = soldNumbers.length;
        document.getElementById('available-count').textContent = totalNumbers - soldNumbers.length;
        
        // Gerar a grade de números
        const numbersGrid = document.getElementById('numbers-grid');
        
        for (let i = 1; i <= totalNumbers; i++) {
            const numberBox = document.createElement('div');
            numberBox.className = 'number-box';
            numberBox.textContent = i;
            numberBox.dataset.number = i;
            
            // Verificar se o número já foi vendido
            if (soldNumbers.includes(i)) {
                numberBox.classList.add('sold');
                numberBox.title = 'Número já vendido';
            } else {
                numberBox.addEventListener('click', toggleNumberSelection);
            }
            
            numbersGrid.appendChild(numberBox);
        }
        
        // Função para selecionar/deselecionar números
        function toggleNumberSelection(event) {
            const numberBox = event.currentTarget;
            const number = parseInt(numberBox.dataset.number);
            
            // Verificar se o número já está selecionado
            const index = selectedNumbers.indexOf(number);
            
            if (index === -1) {
                // Adicionar à seleção
                selectedNumbers.push(number);
                numberBox.classList.add('selected');
            } else {
                // Remover da seleção
                selectedNumbers.splice(index, 1);
                numberBox.classList.remove('selected');
            }
            
            updateSelectionDisplay();
            updateTotalPrice();
        }
        
        // Atualizar a exibição dos números selecionados
        function updateSelectionDisplay() {
            const selectedList = document.getElementById('selected-list');
            const noSelection = document.getElementById('no-selection');
            
            // Limpar a lista atual
            selectedList.innerHTML = '';
            
            if (selectedNumbers.length === 0) {
                noSelection.style.display = 'block';
                return;
            }
            
            noSelection.style.display = 'none';
            
            // Ordenar números em ordem crescente
            selectedNumbers.sort((a, b) => a - b);
            
            // Adicionar cada número selecionado à lista
            selectedNumbers.forEach(number => {
                const numberElement = document.createElement('div');
                numberElement.className = 'selected-number';
                numberElement.innerHTML = `${number} <i class="fas fa-times" data-number="${number}"></i>`;
                selectedList.appendChild(numberElement);
                
                // Adicionar evento para remover número ao clicar no X
                numberElement.querySelector('i').addEventListener('click', function(e) {
                    e.stopPropagation();
                    removeSelectedNumber(number);
                });
            });
        }
        
        // Remover número da seleção
        function removeSelectedNumber(number) {
            const index = selectedNumbers.indexOf(number);
            if (index !== -1) {
                selectedNumbers.splice(index, 1);
                
                // Remover a classe 'selected' do número na grade
                const numberBox = document.querySelector(`.number-box[data-number="${number}"]`);
                if (numberBox) {
                    numberBox.classList.remove('selected');
                }
                
                updateSelectionDisplay();
                updateTotalPrice();
            }
        }
        
        // Calcular e atualizar o preço total
        function updateTotalPrice() {
            const pricePerNumber = 15;
            const totalPrice = selectedNumbers.length * pricePerNumber;
            document.getElementById('total-price').textContent = totalPrice;
        }
        
        // Limpar seleção
        document.getElementById('clear-btn').addEventListener('click', function() {
            // Remover a classe 'selected' de todos os números
            document.querySelectorAll('.number-box.selected').forEach(box => {
                box.classList.remove('selected');
            });
            
            // Limpar array de números selecionados
            selectedNumbers = [];
            
            updateSelectionDisplay();
            updateTotalPrice();
        });
        
        // Simular compra
        document.getElementById('buy-btn').addEventListener('click', function() {
            if (selectedNumbers.length === 0) {
                alert('Por favor, selecione pelo menos um número para comprar.');
                return;
            }
            
            const totalPrice = selectedNumbers.length * 15;
            const numbersList = selectedNumbers.join(', ');
            
            alert(`Você está comprando ${selectedNumbers.length} número(s): ${numbersList}\nValor total: R$ ${totalPrice},00\n\nEm um site real, você seria redirecionado para a página de pagamento.`);
            
            // Marcar números como vendidos (apenas para demonstração)
            selectedNumbers.forEach(number => {
                if (!soldNumbers.includes(number)) {
                    soldNumbers.push(number);
                    
                    // Atualizar a aparência do número na grade
                    const numberBox = document.querySelector(`.number-box[data-number="${number}"]`);
                    if (numberBox) {
                        numberBox.classList.remove('selected');
                        numberBox.classList.add('sold');
                        numberBox.title = 'Número já vendido';
                        numberBox.removeEventListener('click', toggleNumberSelection);
                    }
                }
            });
            
            // Atualizar contagem
            document.getElementById('sold-count').textContent = soldNumbers.length;
            document.getElementById('available-count').textContent = totalNumbers - soldNumbers.length;
            
            // Limpar seleção
            selectedNumbers = [];
            updateSelectionDisplay();
            updateTotalPrice();
        });
        
        // Inicializar exibição
        updateSelectionDisplay();
    </script>
</body>
</html>
