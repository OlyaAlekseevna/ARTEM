<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Телегин Артём Андреевич - Геолог нефти и газа</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=Montserrat:wght@500;600;700;800&display=swap" rel="stylesheet">
    
    <style>
        :root {
            --primary: #0ea5e9;
            --primary-dark: #0284c7;
            --secondary: #7c3aed;
            --accent: #f59e0b;
            --earth: #8b5a2b;
            --rock: #64748b;
            --success: #10b981;
            --dark: #1e293b;
            --light: #f8fafc;
            --gray: #64748b;
            --light-gray: #e2e8f0;
            --gradient: linear-gradient(135deg, #0ea5e9 0%, #7c3aed 100%);
            --gradient-earth: linear-gradient(135deg, #8b5a2b 0%, #0ea5e9 100%);
            --gradient-light: linear-gradient(135deg, rgba(14, 165, 233, 0.1) 0%, rgba(124, 58, 237, 0.1) 100%);
            --card-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.08);
            --transition: all 0.3s ease;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Inter', sans-serif;
            line-height: 1.6;
            color: var(--dark);
            background-color: var(--light);
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Заголовок с градиентом и прозрачностью */
        .hero {
            padding: 80px 0 60px;
            background: var(--gradient-light);
            margin-bottom: 60px;
            position: relative;
            overflow: hidden;
        }
        
        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: var(--gradient);
            opacity: 0.05;
            z-index: -1;
        }
        
        .hero-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: center;
        }
        
        @media (max-width: 992px) {
            .hero-content {
                grid-template-columns: 1fr;
                gap: 30px;
            }
        }
        
        .hero-text h1 {
            font-family: 'Montserrat', sans-serif;
            font-size: 3.2rem;
            font-weight: 800;
            margin-bottom: 10px;
            background: var(--gradient-earth);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            letter-spacing: -0.5px;
            line-height: 1.2;
        }
        
        .hero-subtitle {
            font-size: 1.8rem;
            color: var(--dark);
            margin-bottom: 20px;
            font-weight: 600;
        }
        
        .hero-highlight {
            background: var(--gradient-light);
            padding: 15px 20px;
            border-radius: 12px;
            margin-top: 20px;
            border-left: 4px solid var(--earth);
        }
        
        .hero-info {
            background: white;
            border-radius: 16px;
            padding: 30px;
            box-shadow: var(--card-shadow);
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
            padding-bottom: 20px;
            border-bottom: 1px solid var(--light-gray);
        }
        
        .contact-item:last-child {
            margin-bottom: 0;
            padding-bottom: 0;
            border-bottom: none;
        }
        
        .contact-icon {
            width: 50px;
            height: 50px;
            background: var(--gradient);
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 1.2rem;
            margin-right: 20px;
            flex-shrink: 0;
        }
        
        .contact-text strong {
            display: block;
            margin-bottom: 5px;
            color: var(--dark);
        }
        
        .contact-text span {
            color: var(--gray);
        }
        
        /* Основная информация */
        .main-info {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            margin-bottom: 60px;
        }
        
        @media (max-width: 768px) {
            .main-info {
                grid-template-columns: 1fr;
            }
        }
        
        .card {
            background: white;
            border-radius: 16px;
            padding: 30px;
            box-shadow: var(--card-shadow);
            border: 1px solid rgba(226, 232, 240, 0.8);
        }
        
        .card-title {
            font-family: 'Montserrat', sans-serif;
            font-size: 1.5rem;
            font-weight: 700;
            margin-bottom: 25px;
            color: var(--dark);
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .card-title i {
            color: var(--primary);
        }
        
        .highlight {
            background: var(--gradient-light);
            padding: 8px 15px;
            border-radius: 8px;
            font-weight: 600;
            color: var(--primary-dark);
            border-left: 3px solid var(--primary);
            display: inline-block;
            margin-bottom: 10px;
        }
        
        .badge {
            display: inline-block;
            background: var(--gradient);
            color: white;
            padding: 6px 12px;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 600;
            margin-right: 8px;
            margin-bottom: 8px;
        }
        
        /* Карточки навыков с анимацией */
        .skills-section {
            margin-bottom: 60px;
        }
        
        .section-title {
            font-family: 'Montserrat', sans-serif;
            font-size: 2.2rem;
            font-weight: 700;
            margin-bottom: 40px;
            color: var(--dark);
            text-align: center;
            position: relative;
        }
        
        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: var(--gradient);
            border-radius: 2px;
        }
        
        .skills-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 25px;
        }
        
        @media (max-width: 576px) {
            .skills-container {
                grid-template-columns: 1fr;
            }
        }
        
        .skill-card {
            background: white;
            border-radius: 16px;
            padding: 25px;
            box-shadow: var(--card-shadow);
            transition: var(--transition);
            border: 1px solid rgba(226, 232, 240, 0.8);
            position: relative;
            overflow: hidden;
        }
        
        .skill-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 5px;
            background: var(--gradient);
        }
        
        .skill-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px -10px rgba(0, 0, 0, 0.15);
        }
        
        .skill-card h3 {
            font-size: 1.3rem;
            margin-bottom: 15px;
            color: var(--dark);
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .skill-card h3 i {
            color: var(--primary);
        }
        
        /* Сетка инструментов в виде тегов */
        .tools-section {
            margin-bottom: 60px;
        }
        
        .tools-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
            margin-top: 25px;
        }
        
        .tool-tag {
            background: var(--gradient-light);
            color: var(--primary-dark);
            padding: 10px 18px;
            border-radius: 50px;
            font-size: 0.95rem;
            font-weight: 500;
            border: 1px solid rgba(14, 165, 233, 0.2);
            transition: var(--transition);
            display: flex;
            align-items: center;
            gap: 8px;
        }
        
        .tool-tag:hover {
            background: var(--primary);
            color: white;
            transform: translateY(-3px);
        }
        
        .tool-tag i {
            font-size: 0.9rem;
        }
        
        /* Примеры кейсов в выделенных блоках */
        .cases-section {
            margin-bottom: 60px;
        }
        
        .cases-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
            gap: 30px;
        }
        
        @media (max-width: 768px) {
            .cases-container {
                grid-template-columns: 1fr;
            }
        }
        
        .case-card {
            background: white;
            border-radius: 16px;
            overflow: hidden;
            box-shadow: var(--card-shadow);
            transition: var(--transition);
            border: 1px solid rgba(226, 232, 240, 0.8);
        }
        
        .case-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 20px 40px -10px rgba(0, 0, 0, 0.15);
        }
        
        .case-header {
            background: var(--gradient);
            color: white;
            padding: 25px;
            position: relative;
        }
        
        .case-header h3 {
            font-size: 1.3rem;
            font-weight: 700;
            margin-bottom: 5px;
        }
        
        .case-company {
            font-size: 0.9rem;
            opacity: 0.9;
        }
        
        .case-content {
            padding: 25px;
        }
        
        .case-content p {
            margin-bottom: 15px;
            color: var(--gray);
        }
        
        .case-highlight {
            background: var(--gradient-light);
            padding: 15px;
            border-radius: 10px;
            margin-top: 15px;
            border-left: 4px solid var(--primary);
        }
        
        .case-highlight strong {
            color: var(--primary-dark);
        }
        
        /* Опыт работы */
        .experience-section {
            margin-bottom: 60px;
        }
        
        .experience-card {
            background: white;
            border-radius: 16px;
            padding: 30px;
            box-shadow: var(--card-shadow);
            margin-bottom: 30px;
            border-left: 5px solid var(--primary);
        }
        
        .experience-header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-bottom: 20px;
            flex-wrap: wrap;
            gap: 15px;
        }
        
        .experience-title {
            font-size: 1.4rem;
            color: var(--dark);
            font-weight: 700;
        }
        
        .experience-period {
            background: var(--gradient-light);
            padding: 8px 15px;
            border-radius: 20px;
            font-weight: 600;
            color: var(--primary-dark);
        }
        
        .experience-subtitle {
            color: var(--primary);
            font-weight: 600;
            margin-bottom: 15px;
            font-size: 1.1rem;
        }
        
        .experience-details {
            color: var(--gray);
            margin-bottom: 20px;
        }
        
        .responsibilities {
            margin-top: 20px;
            padding-left: 20px;
        }
        
        .responsibilities li {
            margin-bottom: 10px;
            color: var(--gray);
        }
        
        /* Дополнительная информация */
        .additional-info {
            background: white;
            border-radius: 16px;
            padding: 30px;
            margin-bottom: 60px;
            box-shadow: var(--card-shadow);
            border-left: 5px solid var(--earth);
        }
        
        .additional-info h2 {
            font-family: 'Montserrat', sans-serif;
            font-size: 1.8rem;
            margin-bottom: 20px;
            color: var(--dark);
        }
        
        .additional-info p {
            margin-bottom: 15px;
            color: var(--gray);
        }
        
        .hobby-item {
            display: flex;
            align-items: center;
            margin-bottom: 15px;
            padding: 15px;
            background: var(--gradient-light);
            border-radius: 10px;
        }
        
        .hobby-icon {
            width: 40px;
            height: 40px;
            background: var(--earth);
            color: white;
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 15px;
            font-size: 1.2rem;
        }
        
        /* Языки */
        .languages {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 20px;
        }
        
        .language-item {
            flex: 1;
            min-width: 200px;
            background: white;
            border-radius: 12px;
            padding: 20px;
            box-shadow: var(--card-shadow);
            border: 1px solid var(--light-gray);
        }
        
        .language-name {
            font-weight: 700;
            margin-bottom: 10px;
            color: var(--dark);
        }
        
        .language-level {
            color: var(--primary);
            font-weight: 600;
            margin-bottom: 15px;
        }
        
        .language-bar {
            height: 8px;
            background: var(--light-gray);
            border-radius: 4px;
            overflow: hidden;
        }
        
        .language-progress {
            height: 100%;
            background: var(--gradient);
            border-radius: 4px;
        }
        
        /* Адаптивность для мобильных устройств */
        @media (max-width: 768px) {
            .hero {
                padding: 50px 0 40px;
            }
            
            .hero-text h1 {
                font-size: 2.2rem;
            }
            
            .hero-subtitle {
                font-size: 1.4rem;
            }
            
            .section-title {
                font-size: 1.8rem;
            }
            
            .hero-info {
                padding: 20px;
            }
            
            .contact-item {
                flex-direction: column;
                align-items: flex-start;
                gap: 10px;
            }
            
            .contact-icon {
                margin-right: 0;
                margin-bottom: 10px;
            }
            
            .card {
                padding: 20px;
            }
            
            .experience-header {
                flex-direction: column;
                align-items: flex-start;
            }
            
            .language-item {
                min-width: 100%;
            }
        }
        
        @media (max-width: 480px) {
            .hero-text h1 {
                font-size: 1.8rem;
            }
            
            .hero-subtitle {
                font-size: 1.2rem;
            }
            
            .section-title {
                font-size: 1.6rem;
            }
            
            .tool-tag {
                padding: 8px 14px;
                font-size: 0.85rem;
            }
            
            .badge {
                font-size: 0.8rem;
                padding: 5px 10px;
            }
        }
        
        /* Анимации */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .fade-in {
            opacity: 0;
            animation: fadeIn 0.8s ease forwards;
        }
        
        .delay-1 { animation-delay: 0.1s; }
        .delay-2 { animation-delay: 0.2s; }
        .delay-3 { animation-delay: 0.3s; }
        .delay-4 { animation-delay: 0.4s; }
        
        /* Кнопка для печати/скачивания */
        .print-btn {
            position: fixed;
            bottom: 30px;
            right: 30px;
            width: 60px;
            height: 60px;
            background: var(--gradient);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            box-shadow: 0 5px 15px rgba(14, 165, 233, 0.3);
            cursor: pointer;
            z-index: 100;
            transition: var(--transition);
        }
        
        .print-btn:hover {
            transform: scale(1.1);
        }
        
        @media (max-width: 768px) {
            .print-btn {
                bottom: 20px;
                right: 20px;
                width: 50px;
                height: 50px;
                font-size: 1.2rem;
            }
        }
        
        /* Футер */
        .footer {
            text-align: center;
            padding: 30px 0;
            margin-top: 40px;
            border-top: 1px solid var(--light-gray);
            color: var(--gray);
            font-size: 0.9rem;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Заголовок с градиентом -->
        <section class="hero fade-in">
            <div class="hero-content">
                <div class="hero-text">
                    <h1>Телегин Артём Андреевич</h1>
                    <div class="hero-subtitle">Геолог нефти и газа</div>
                    <p style="color: var(--gray); margin-top: 20px;">Студент 3 курса Тюменского индустриального университета по специальности "Геолог нефти и газа". Увлечённый геологией, стремлюсь развиваться в области нефтегазовой геологии и применять свои знания на практике.</p>
                    <div class="hero-highlight">
                        <strong>Цель:</strong> Стать экспертом в области геологии и работать в престижной нефтегазовой компании.
                    </div>
                </div>
                
                <div class="hero-info fade-in delay-1">
                    <div class="contact-item">
                        <div class="contact-icon">
                            <i class="fas fa-phone"></i>
                        </div>
                        <div class="contact-text">
                            <strong>+7 (922) 0447111</strong>
                            <span>Предпочитаемый способ связи</span>
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <div class="contact-icon">
                            <i class="fas fa-envelope"></i>
                        </div>
                        <div class="contact-text">
                            <strong>atelegin36@gmail.com</strong>
                            <span>Электронная почта</span>
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <div class="contact-icon">
                            <i class="fas fa-map-marker-alt"></i>
                        </div>
                        <div class="contact-text">
                            <strong>Тюмень</strong>
                            <span>Проживает, не готов к переезду, готов к командировкам</span>
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <div class="contact-icon">
                            <i class="fas fa-passport"></i>
                        </div>
                        <div class="contact-text">
                            <strong>Россия</strong>
                            <span>Гражданство, есть разрешение на работу</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- Основная информация -->
        <section class="main-info">
            <div class="card fade-in delay-1">
                <h2 class="card-title"><i class="fas fa-bullseye"></i> Карьерные цели</h2>
                <p><span class="highlight">Геолог нефти и газа</span></p>
                <p><strong>Специализации:</strong> Геолог</p>
                <p><strong>Тип занятости:</strong> Полная занятость, частичная занятость, проектная работа, стажировка</p>
                <p><strong>График работы:</strong> Полный день, сменный график, гибкий график, удаленная работа</p>
                <p><strong>Желательное время в пути до работы:</strong> Не имеет значения</p>
                <p><strong>Опыт работы:</strong> 2 месяца</p>
            </div>
            
            <div class="card fade-in delay-2">
                <h2 class="card-title"><i class="fas fa-user-graduate"></i> Образование</h2>
                <p><strong>Уровень:</strong> Неоконченное высшее</p>
                <p><strong>Год окончания:</strong> 2027 (ожидаемый)</p>
                <p><strong>ВУЗ:</strong> Тюменский индустриальный университет</p>
                <p><strong>Институт:</strong> Институт геологии и нефтегазодобычи</p>
                <p><strong>Специальность:</strong> Геология нефти и газа</p>
                <div style="margin-top: 20px;">
                    <span class="badge">Студент 3 курса</span>
                    <span class="badge">Очная форма</span>
                </div>
            </div>
        </section>
        
        <!-- Языки -->
        <section class="skills-section">
            <h2 class="section-title fade-in">Знание языков</h2>
            <div class="languages">
                <div class="language-item fade-in delay-1">
                    <div class="language-name">Русский</div>
                    <div class="language-level">Родной</div>
                    <div class="language-bar">
                        <div class="language-progress" style="width: 100%"></div>
                    </div>
                </div>
                
                <div class="language-item fade-in delay-2">
                    <div class="language-name">Английский</div>
                    <div class="language-level">C1 — Продвинутый</div>
                    <div class="language-bar">
                        <div class="language-progress" style="width: 90%"></div>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- Ключевые навыки в карточках -->
        <section class="skills-section">
            <h2 class="section-title fade-in">Ключевые навыки</h2>
            <div class="skills-container">
                <div class="skill-card fade-in delay-1">
                    <h3><i class="fas fa-mountain"></i> Геологические навыки</h3>
                    <p>Ведение геологических маршрутов, сбор образцов горных пород, построение геологических карт, определение рельефа местности.</p>
                </div>
                
                <div class="skill-card fade-in delay-2">
                    <h3><i class="fas fa-users"></i> Лидерские качества</h3>
                    <p>Опыт руководства группой из 24 человек, организация работы команды, распределение задач, контроль выполнения.</p>
                </div>
                
                <div class="skill-card fade-in delay-3">
                    <h3><i class="fas fa-book"></i> Научно-исследовательская деятельность</h3>
                    <p>Ведение журналов образцов, анализ геологических данных, работа с научной документацией, участие в полевых исследованиях.</p>
                </div>
            </div>
        </section>
        
        <!-- Инструменты и технологии -->
        <section class="tools-section">
            <h2 class="section-title fade-in">Инструменты и технологии</h2>
            <div class="card fade-in delay-1">
                <div class="tools-grid">
                    <span class="tool-tag"><i class="fas fa-map"></i> Isoline</span>
                    <span class="tool-tag"><i class="fas fa-chart-line"></i> Plotlog</span>
                    <span class="tool-tag"><i class="fas fa-drafting-compass"></i> AutoCAD</span>
                    <span class="tool-tag"><i class="fas fa-cube"></i> nanoCAD</span>
                    <span class="tool-tag"><i class="fas fa-map-marked-alt"></i> ГИС</span>
                    <span class="tool-tag"><i class="fas fa-file-excel"></i> MS Excel</span>
                    <span class="tool-tag"><i class="fas fa-file-powerpoint"></i> MS PowerPoint</span>
                    <span class="tool-tag"><i class="fas fa-file-word"></i> MS Word</span>
                    <span class="tool-tag"><i class="fas fa-desktop"></i> MS Office</span>
                    <span class="tool-tag"><i class="fas fa-code"></i> Java</span>
                    <span class="tool-tag"><i class="fas fa-paint-brush"></i> CorelDraw</span>
                    <span class="tool-tag"><i class="fas fa-phone-alt"></i> Телефонные переговоры</span>
                </div>
            </div>
        </section>
        
        <!-- Опыт работы -->
        <section class="experience-section">
            <h2 class="section-title fade-in">Опыт работы</h2>
            <div class="experience-card fade-in delay-1">
                <div class="experience-header">
                    <div>
                        <h3 class="experience-title">Тюменский Индустриальный Университет</h3>
                        <div class="experience-subtitle">Бригадир (учебная практика)</div>
                    </div>
                    <div class="experience-period">Июнь 2024 — Июль 2024 (2 месяца)</div>
                </div>
                
                <div class="experience-details">
                    <p>Проходил учебную практику в городе Сухой Лог в 2024 году, где занимал должность бригадира, руководил группой студентов из 24 человек.</p>
                </div>
                
                <div>
                    <h4 style="color: var(--dark); margin-bottom: 10px;">Обязанности:</h4>
                    <ul class="responsibilities">
                        <li>Организация группы студентов и ведение по геологическим маршрутам</li>
                        <li>Сбор образцов горных пород</li>
                        <li>Проведение разведок и активное участие в построении карт геологических маршрутов</li>
                        <li>Ведение журнала образцов горных пород, собранных в маршрутах</li>
                    </ul>
                </div>
                
                <div class="case-highlight" style="margin-top: 20px;">
                    <strong>Цель практики:</strong> Научиться вести геологические маршруты, определять рельеф и строить карту местности.
                </div>
            </div>
        </section>
        
        <!-- Дополнительная информация -->
        <section class="additional-info fade-in delay-2">
            <h2><i class="fas fa-user"></i> Обо мне</h2>
            <p>Прохожу третий курс обучения по специальности "Геолог нефти и газа" в Тюменском индустриальном университете. Я очень люблю геологию, меня всегда интересовало, как и почему природа вокруг нас сформировалась такой, какая она есть. Увлекаюсь минералами и горным породам, собираю свою коллекцию.</p>
            
            <h3 style="margin: 25px 0 15px; color: var(--dark);">Увлечения и хобби:</h3>
            
            <div class="hobby-item">
                <div class="hobby-icon">
                    <i class="fas fa-volleyball-ball"></i>
                </div>
                <div>
                    <strong>Волейбол</strong>
                    <p>Играю за сборную университета по волейболу в 3 лиге. Занял 3 место во 2 Спартакиаде профессиональных образовательных организаций высшего образования Тюменской области на 2023-2024 учебный год по волейболу среди мужских команд до 19 лет.</p>
                </div>
            </div>
            
            <div class="hobby-item">
                <div class="hobby-icon">
                    <i class="fas fa-book-open"></i>
                </div>
                <div>
                    <strong>Чтение</strong>
                    <p>В свободное время предпочитаю читать книги. Моей любимой книгой является роман "Метро 2033" за авторством Дмитрия Глуховского. Эта книга научила меня тому, что человек - удивительное существо, способное адаптироваться даже к самым сложным условиям жизни, оставаясь самим собой.</p>
                </div>
            </div>
            
            <div class="hobby-item">
                <div class="hobby-icon">
                    <i class="fas fa-gem"></i>
                </div>
                <div>
                    <strong>Коллекционирование минералов</strong>
                    <p>Собираю свою коллекцию минералов и горных пород, увлекаюсь их изучением и классификацией.</p>
                </div>
            </div>
        </section>
        
        <!-- Футер -->
        <footer class="footer fade-in delay-3">
            <p><strong>Телегин Артём Андреевич</strong> | Геолог нефти и газа</p>
            <p>Резюме обновлено 24 марта 2025 в 09:38</p>
            <p style="margin-top: 10px; font-size: 0.8rem;">Готов к новым вызовам и профессиональному развитию в области геологии нефти и газа</p>
        </footer>
    </div>
    
    <!-- Кнопка для печати -->
    <div class="print-btn" onclick="window.print()">
        <i class="fas fa-print"></i>
    </div>

    <script>
        // Анимация элементов при прокрутке
        document.addEventListener('DOMContentLoaded', function() {
            const fadeElements = document.querySelectorAll('.fade-in');
            
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = 1;
                        entry.target.style.transform = 'translateY(0)';
                    }
                });
            }, { threshold: 0.1 });
            
            fadeElements.forEach(el => {
                el.style.opacity = 0;
                el.style.transform = 'translateY(20px)';
                el.style.transition = 'opacity 0.8s ease, transform 0.8s ease';
                observer.observe(el);
            });
            
            // Анимация карточек навыков при наведении
            const skillCards = document.querySelectorAll('.skill-card');
            skillCards.forEach(card => {
                card.addEventListener('mouseenter', function() {
                    this.style.transform = 'translateY(-10px)';
                });
                
                card.addEventListener('mouseleave', function() {
                    this.style.transform = 'translateY(0)';
                });
            });
            
            // Анимация тегов инструментов
            const toolTags = document.querySelectorAll('.tool-tag');
            toolTags.forEach(tag => {
                tag.addEventListener('mouseenter', function() {
                    this.style.transform = 'translateY(-3px)';
                });
                
                tag.addEventListener('mouseleave', function() {
                    this.style.transform = 'translateY(0)';
                });
            });
            
            // Анимация карточек кейсов
            const caseCards = document.querySelectorAll('.case-card');
            caseCards.forEach(card => {
                card.addEventListener('mouseenter', function() {
                    this.style.transform = 'translateY(-8px)';
                });
                
                card.addEventListener('mouseleave', function() {
                    this.style.transform = 'translateY(0)';
                });
            });
            
            // Анимация прогресс-баров языков
            const progressBars = document.querySelectorAll('.language-progress');
            progressBars.forEach(bar => {
                const width = bar.style.width;
                bar.style.width = '0%';
                setTimeout(() => {
                    bar.style.width = width;
                    bar.style.transition = 'width 1.5s ease';
                }, 300);
            });
        });
        
        // Адаптация для мобильных устройств
        function checkMobile() {
            if (window.innerWidth <= 768) {
                document.body.classList.add('mobile');
            } else {
                document.body.classList.remove('mobile');
            }
        }
        
        window.addEventListener('load', checkMobile);
        window.addEventListener('resize', checkMobile);
        
        // Печать резюме
        function printResume() {
            window.print();
        }
    </script>
</body>
</html>
