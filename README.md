<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SUS+Vida - Tecnologia a serviço da saúde pública</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root {
            --sus-green: #36AA3E;
            --sus-blue: #1A7998;
            --sus-light: #F8F9FA;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            color: #333;
        }
        
        .navbar {
            background-color: var(--sus-green);
        }
        
        .navbar-brand {
            font-weight: 700;
            color: white !important;
        }
        
        .btn-sus {
            background-color: var(--sus-green);
            color: white;
        }
        
        .btn-sus:hover {
            background-color: #2d8d35;
            color: white;
        }
        
        .hero-section {
            background: linear-gradient(rgba(54, 170, 62, 0.9), rgba(54, 170, 62, 0.8)), 
                        url('https://placehold.co/1920x600?text=SUS+Vida+fazendo+a+saúde+pública+mais+acessível');
            background-size: cover;
            background-position: center;
            color: white;
            padding: 5rem 0;
            text-align: center;
        }
        
        .feature-card {
            border: none;
            border-radius: 10px;
            transition: transform 0.3s;
            height: 100%;
        }
        
        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }
        
        .feature-icon {
            font-size: 2.5rem;
            color: var(--sus-green);
            margin-bottom: 1rem;
        }
        
        .footer {
            background-color: var(--sus-blue);
            color: white;
            padding: 3rem 0;
        }
        
        .accessibility-tools {
            position: fixed;
            bottom: 20px;
            right: 20px;
            z-index: 1000;
        }
        
        .tab-content {
            padding: 2rem;
            background-color: white;
            border-radius: 0 0 10px 10px;
        }
        
        .nav-tabs .nav-link.active {
            background-color: var(--sus-green);
            color: white !important;
        }
        
        .nav-tabs .nav-link {
            color: var(--sus-green);
        }
        
        .symptoms-area {
            min-height: 150px;
        }
    </style>
</head>
<body>
    <!-- Barra de navegação -->
    <nav class="navbar navbar-expand-lg navbar-dark">
        <div class="container">
            <a class="navbar-brand" href="#">
                <i class="fas fa-heartbeat me-2"></i>SUS+Vida
            </a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item">
                        <a class="nav-link active" href="#"><i class="fas fa-home me-1"></i> Início</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#agendar"><i class="fas fa-calendar-check me-1"></i> Agendar</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#especialidades"><i class="fas fa-stethoscope me-1"></i> Especialidades</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#cirurgias"><i class="fas fa-procedures me-1"></i> Cirurgias</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#duvidas"><i class="fas fa-question-circle me-1"></i> Dúvidas</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#monitor"><i class="fas fa-watch me-1"></i> Monitor</a>
                    </li>
                </ul>
                <a href="#login" class="btn btn-outline-light ms-3"><i class="fas fa-user me-1"></i> Entrar</a>
            </div>
        </div>
    </nav>

    <!-- Seção Hero -->
    <section class="hero-section">
        <div class="container text-center">
            <h1 class="display-4 fw-bold mb-4">Tecnologia e saúde caminhando juntas</h1>
            <p class="lead mb-5">Facilitamos seu acesso aos serviços de saúde pública com praticidade e inovação</p>
            <div class="d-flex justify-content-center gap-3">
                <a href="#agendar" class="btn btn-light btn-lg px-4">Agendar Consulta</a>
                <a href="#saiba-mais" class="btn btn-outline-light btn-lg px-4">Saiba Mais</a>
            </div>
        </div>
    </section>

    <!-- Seção de Recursos Rápidos -->
    <section class="py-5 bg-light">
        <div class="container">
            <h2 class="text-center mb-5">Acesso Rápido</h2>
            <div class="row g-4">
                <div class="col-md-3">
                    <a href="#agendar" class="text-decoration-none">
                        <div class="card feature-card shadow-sm text-center p-4">
                            <div class="feature-icon">
                                <i class="fas fa-calendar-alt"></i>
                            </div>
                            <h5>Agendar Consulta</h5>
                            <p>Marque sua consulta de forma rápida e prática</p>
                        </div>
                    </a>
                </div>
                <div class="col-md-3">
                    <a href="#especialidades" class="text-decoration-none">
                        <div class="card feature-card shadow-sm text-center p-4">
                            <div class="feature-icon">
                                <i class="fas fa-stethoscope"></i>
                            </div>
                            <h5>Especialidades</h5>
                            <p>Conheça os especialistas disponíveis</p>
                        </div>
                    </a>
                </div>
                <div class="col-md-3">
                    <a href="#duvidas" class="text-decoration-none">
                        <div class="card feature-card shadow-sm text-center p-4">
                            <div class="feature-icon">
                                <i class="fas fa-question"></i>
                            </div>
                            <h5>Tire suas Dúvidas</h5>
                            <p>Perguntas frequentes sobre o SUS</p>
                        </div>
                    </a>
                </div>
                <div class="col-md-3">
                    <a href="#monitor" class="text-decoration-none">
                        <div class="card feature-card shadow-sm text-center p-4">
                            <div class="feature-icon">
                                <i class="fas fa-heartbeat"></i>
                            </div>
                            <h5>Monitor SUS+Vida</h5>
                            <p>Relógio inteligente para sua saúde</p>
                        </div>
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Seção de Conteúdo Principal -->
    <section class="py-5" id="main-content">
        <div class="container">
            <ul class="nav nav-tabs" id="myTab" role="tablist">
                <li class="nav-item" role="presentation">
                    <button class="nav-link active" id="agendar-tab" data-bs-toggle="tab" data-bs-target="#agendar" type="button" role="tab">
                        <i class="fas fa-calendar-check me-1"></i> Agendar Consultas
                    </button>
                </li>
                <li class="nav-item" role="presentation">
                    <button class="nav-link" id="especialidades-tab" data-bs-toggle="tab" data-bs-target="#especialidades" type="button" role="tab">
                        <i class="fas fa-stethoscope me-1"></i> Especialidades
                    </button>
                </li>
                <li class="nav-item" role="presentation">
                    <button class="nav-link" id="cirurgias-tab" data-bs-toggle="tab" data-bs-target="#cirurgias" type="button" role="tab">
                        <i class="fas fa-procedures me-1"></i> Cirurgias
                    </button>
                </li>
                <li class="nav-item" role="presentation">
                    <button class="nav-link" id="duvidas-tab" data-bs-toggle="tab" data-bs-target="#duvidas" type="button" role="tab">
                        <i class="fas fa-question-circle me-1"></i> Dúvidas
                    </button>
                </li>
                <li class="nav-item" role="presentation">
                    <button class="nav-link" id="sintomas-tab" data-bs-toggle="tab" data-bs-target="#sintomas" type="button" role="tab">
                        <i class="fas fa-comment-medical me-1"></i> Fale seus Sintomas
                    </button>
                </li>
                <li class="nav-item" role="presentation">
                    <button class="nav-link" id="monitor-tab" data-bs-toggle="tab" data-bs-target="#monitor" type="button" role="tab">
                        <i class="fas fa-watch me-1"></i> Monitor SUS+Vida
                    </button>
                </li>
            </ul>
            
            <div class="tab-content" id="myTabContent">
                <!-- Tab Agendar Consultas -->
                <div class="tab-pane fade show active" id="agendar" role="tabpanel">
                    <h3 class="mb-4"><i class="fas fa-calendar-check text-success me-2"></i>Agendar Consulta Médica</h3>
                    <div class="row">
                        <div class="col-md-6">
                            <form>
                                <div class="mb-3">
                                    <label for="especialidade" class="form-label">Especialidade Médica</label>
                                    <select class="form-select" id="especialidade" required>
                                        <option value="">Selecione uma especialidade</option>
                                        <option>Clínica Geral</option>
                                        <option>Cardiologia</option>
                                        <option>Ginecologia</option>
                                        <option>Pediatria</option>
                                        <option>Psicologia</option>
                                        <option>Dermatologia</option>
                                        <option>Ortopedia</option>
                                    </select>
                                </div>
                                <div class="mb-3">
                                    <label for="data" class="form-label">Data da Consulta</label>
                                    <input type="date" class="form-control" id="data" required>
                                </div>
                                <div class="mb-3">
                                    <label for="horario" class="form-label">Horário Disponível</label>
                                    <select class="form-select" id="horario" required>
                                        <option value="">Selecione um horário</option>
                                        <option>08:00 - 08:30</option>
                                        <option>08:30 - 09:00</option>
                                        <option>09:00 - 09:30</option>
                                        <!-- Mais opções de horário -->
                                    </select>
                                </div>
                                <button type="submit" class="btn btn-sus">Confirmar Agendamento</button>
                            </form>
                        </div>
                        <div class="col-md-6">
                            <div class="card bg-light p-4">
                                <h5>Informações Importantes</h5>
                                <ul>
                                    <li>Chegue com 15 minutos de antecedência</li>
                                    <li>Traga seu cartão SUS e documento com foto</li>
                                    <li>Em caso de desistência, cancele com 24h de antecedência</li>
                                    <li>Faltas consecutivas podem gerar restrições</li>
                                </ul>
                                <div class="alert alert-info mt-3">
                                    Você receberá um e-mail de confirmação com todos os detalhes.
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Tab Especialidades -->
                <div class="tab-pane fade" id="especialidades" role="tabpanel">
                    <h3 class="mb-4"><i class="fas fa-stethoscope text-success me-2"></i>Especialidades Médicas Disponíveis</h3>
                    <div class="row">
                        <div class="col-md-4 mb-4">
                            <div class="card h-100">
                                <div class="card-body">
                                    <h5 class="card-title text-success">Clínica Geral</h5>
                                    <p class="card-text">Atendimento para diagnósticos gerais, encaminhamentos e cuidados básicos de saúde.</p>
                                    <a href="#" class="btn btn-sus btn-sm">Visualizar Profissionais</a>
                                </div>
                            </div>
                        </div>
                        <div class="col-md-4 mb-4">
                            <div class="card h-100">
                                <div class="card-body">
                                    <h5 class="card-title text-success">Cardiologia</h5>
                                    <p class="card-text">Especializada no diagnóstico e tratamento de doenças do coração e sistema circulatório.</p>
                                    <a href="#" class="btn btn-sus btn-sm">Visualizar Profissionais</a>
                                </div>
                            </div>
                        </div>
                        <div class="col-md-4 mb-4">
                            <div class="card h-100">
                                <div class="card-body">
                                    <h5 class="card-title text-success">Ginecologia</h5>
                                    <p class="card-text">Cuidados com a saúde da mulher, prevenção e tratamento de doenças do sistema reprodutivo.</p>
                                    <a href="#" class="btn btn-sus btn-sm">Visualizar Profissionais</a>
                                </div>
                            </div>
                        </div>
                        <div class="col-md-4 mb-4">
                            <div class="card h-100">
                                <div class="card-body">
                                    <h5 class="card-title text-success">Pediatria</h5>
                                    <p class="card-text">Atendimento especializado para crianças e adolescentes até 18 anos.</p>
                                    <a href="#" class="btn btn-sus btn-sm">Visualizar Profissionais</a>
                                </div>
                            </div>
                        </div>
                        <div class="col-md-4 mb-4">
                            <div class="card h-100">
                                <div class="card-body">
                                    <h5 class="card-title text-success">Psicologia</h5>
                                    <p class="card-text">Atendimento psicológico para promoção da saúde mental e tratamento de transtornos.</p>
                                    <a href="#" class="btn btn-sus btn-sm">Visualizar Profissionais</a>
                                </div>
                            </div>
                        </div>
                        <div class="col-md-4 mb-4">
                            <div class="card h-100">
                                <div class="card-body">
                                    <h5 class="card-title text-success">Ortopedia</h5>
                                    <p class="card-text">Diagnóstico e tratamento de problemas relacionados ao sistema músculo-esquelético.</p>
                                    <a href="#" class="btn btn-sus btn-sm">Visualizar Profissionais</a>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Tab Cirurgias -->
                <div class="tab-pane fade" id="cirurgias" role="tabpanel">
                    <h3 class="mb-4"><i class="fas fa-procedures text-success me-2"></i>Agendamento de Cirurgias</h3>
                    <div class="row">
                        <div class="col-md-6">
                            <div class="alert alert-info">
                                <p class="mb-0">Esta área é destinada a pacientes que já possuem encaminhamento médico para realização de procedimentos cirúrgicos.</p>
                            </div>
                            <form>
                                <div class="mb-3">
                                    <label for="tipo-cirurgia" class="form-label">Tipo de Cirurgia</label>
                                    <input type="text" class="form-control" id="tipo-cirurgia" required>
                                </div>
                                <div class="mb-3">
                                    <label for="medico-solicitante" class="form-label">Médico Solicitante</label>
                                    <input type="text" class="form-control" id="medico-solicitante" required>
                                </div>
                                <div class="mb-3">
                                    <label for="hospital-preferencia" class="form-label">Hospital de Preferência</label>
                                    <select class="form-select" id="hospital-preferencia" required>
                                        <option value="">Selecione um hospital</option>
                                        <option>Hospital Central</option>
                                        <option>Hospital Municipal</option>
                                        <option>Hospital da Criança</option>
                                        <option>Hospital da Mulher</option>
                                    </select>
                                </div>
                                <div class="mb-3">
                                    <label for="documentos" class="form-label">Documentos Médicos</label>
                                    <input type="file" class="form-control" id="documentos" required>
                                    <small class="text-muted">Upload do encaminhamento médico e exames pré-operatórios</small>
                                </div>
                                <button type="submit" class="btn btn-sus">Solicitar Agendamento</button>
                            </form>
                        </div>
                        <div class="col-md-6">
                            <div class="card bg-light p-4">
                                <h5 class="text-success">Status das Cirurgias</h5>
                                <div class="list-group mt-3">
                                    <div class="list-group-item">
                                        <div class="d-flex w-100 justify-content-between">
                                            <h6 class="mb-1">Cirurgia de Apêndice</h6>
                                            <small class="text-success">Confirmada</small>
                                        </div>
                                        <small>Hospital Central - 15/05/2024 - 08:00</small>
                                    </div>
                                    <div class="list-group-item">
                                        <div class="d-flex w-100 justify-content-between">
                                            <h6 class="mb-1">Histerectomia</h6>
                                            <small class="text-warning">Aguardando confirmação</small>
                                        </div>
                                    </div>
                                    <div class="list-group-item">
                                        <div class="d-flex w-100 justify-content-between">
                                            <h6 class="mb-1">Artroscopia de Joelho</h6>
                                            <small class="text-success">Realizada em 12/03/2024</small>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Tab Dúvidas -->
                <div class="tab-pane fade" id="duvidas" role="tabpanel">
                    <h3 class="mb-4"><i class="fas fa-question-circle text-success me-2"></i>Perguntas Frequentes</h3>
                    <div class="accordion" id="faqAccordion">
                        <div class="accordion-item">
                            <h2 class="accordion-header">
                                <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#faq1">
                                    Como faço para obter meu cartão SUS?
                                </button>
                            </h2>
                            <div id="faq1" class="accordion-collapse collapse show" data-bs-parent="#faqAccordion">
                                <div class="accordion-body">
                                    O cartão SUS pode ser obtido em qualquer unidade básica de saúde, apresentando documento de identidade com foto e comprovante de residência. O atendimento é gratuito e o cartão é emitido na hora.
                                </div>
                            </div>
                        </div>
                        <div class="accordion-item">
                            <h2 class="accordion-header">
                                <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#faq2">
                                    Posso escolher o médico que vai me atender?
                                </button>
                            </h2>
                            <div id="faq2" class="accordion-collapse collapse" data-bs-parent="#faqAccordion">
                                <div class="accordion-body">
                                    No SUS+Vida, você pode visualizar os profissionais disponíveis em cada especialidade e, quando possível, selecionar o médico de sua preferência. No entanto, em algumas situações, o atendimento será realizado pelo profissional disponível no momento.
                                </div>
                            </div>
                        </div>
                        <div class="accordion-item">
                            <h2 class="accordion-header">
                                <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#faq3">
                                    Quais documentos preciso levar para a consulta?
                                </button>
                            </h2>
                            <div id="faq3" class="accordion-collapse collapse" data-bs-parent="#faqAccordion">
                                <div class="accordion-body">
                                    Obrigatoriamente: Cartão SUS e documento oficial com foto (RG, CNH, passaporte, etc.). Recomenda-se também levar exames recentes, lista de medicamentos em uso e carteira de vacinação.
                                </div>
                            </div>
                        </div>
                        <div class="accordion-item">
                            <h2 class="accordion-header">
                                <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#faq4">
                                    Como cancelar ou remarcar uma consulta?
                                </button>
                            </h2>
                            <div id="faq4" class="accordion-collapse collapse" data-bs-parent="#faqAccordion">
                                <div class="accordion-body">
                                    Você pode cancelar ou remarcar consultas diretamente por este portal, na seção "Meus Agendamentos". O cancelamento deve ser feito com pelo menos 24 horas de antecedência para evitar restrições futuras.
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <div class="card mt-4">
                        <div class="card-body">
                            <h5 class="card-title">Não encontrou sua resposta?</h5>
                            <form>
                                <div class="mb-3">
                                    <label for="pergunta" class="form-label">Faça sua pergunta</label>
                                    <textarea class="form-control" id="pergunta" rows="3"></textarea>
                                </div>
                                <button type="submit" class="btn btn-sus">Enviar Pergunta</button>
                            </form>
                        </div>
                    </div>
                </div>
                
                <!-- Tab Sintomas -->
                <div class="tab-pane fade" id="sintomas" role="tabpanel">
                    <h3 class="mb-4"><i class="fas fa-comment-medical text-success me-2"></i>Fale seus Sintomas</h3>
                    <div class="alert alert-warning">
                        <i class="fas fa-exclamation-triangle me-2"></i>
                        Esta função não substitui o diagnóstico médico. O sistema fornece orientações iniciais com base nos sintomas relatados, mas uma avaliação médica presencial é sempre necessária para diagnóstico preciso e tratamento adequado.
                    </div>
                    <div class="row">
                        <div class="col-md-6">
                            <h5>Descreva seus sintomas</h5>
                            <div class="mb-3">
                                <textarea class="form-control symptoms-area" id="sintomas-texto" placeholder="Descreva detalhadamente seus sintomas, quando começaram, intensidade, fatores que melhoram ou pioram..."></textarea>
                            </div>
                            <button class="btn btn-outline-success mb-3" id="btn-gravacao">
                                <i class="fas fa-microphone me-2"></i>Gravar por Voz
                            </button>
                            <button class="btn btn-sus" id="analisar-sintomas">
                                <i class="fas fa-search me-2"></i>Analisar Sintomas
                            </button>
                        </div>
                        <div class="col-md-6">
                            <div class="card bg-light h-100">
                                <div class="card-body">
                                    <h5 class="card-title text-success">Orientação Preliminar</h5>
                                    <div id="resultado-sintomas" class="mt-3">
                                        <p class="text-muted">Após descrever seus sintomas e clicar em "Analisar Sintomas", você receberá orientações preliminares sobre os próximos passos recomendados.</p>
                                    </div>
                                    <div id="orientacao-ia" class="d-none">
                                        <div class="alert alert-info">
                                            <h6>Recomendação:</h6>
                                            <p id="texto-orientacao"></p>
                                        </div>
                                        <div class="d-grid gap-2">
                                            <button class="btn btn-sus">Agendar Consulta</button>
                                            <button class="btn btn-outline-success">Ver Unidades de Atendimento</button>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Tab Monitor SUS+Vida -->
                <div class="tab-pane fade" id="monitor" role="tabpanel">
                    <h3 class="mb-4"><i class="fas fa-watch text-success me-2"></i>Monitor SUS+Vida</h3>
                    <div class="row align-items-center">
                        <div class="col-md-6">
                            <img src="https://placehold.co/500x300?text=Relógio+Inteligente+SUS+Vida+com+monitoramento+de+saúde" class="img-fluid rounded" alt="Relógio inteligente SUS+Vida com tela retangular, pulseira verde e mostrando dados de batimento cardíaco">
                        </div>
                        <div class="col-md-6">
                            <h4 class="mb-3">Seu companheiro de saúde 24 horas</h4>
                            <ul class="list-group mb-4">
                                <li class="list-group-item d-flex align-items-center">
                                    <i class="fas fa-heartbeat text-success me-3"></i>
                                    <span>Monitoramento contínuo dos batimentos cardíacos</span>
                                </li>
                                <li class="list-group-item d-flex align-items-center">
                                    <i class="fas fa-tint text-success me-3"></i>
                                    <span>Controle da hidratação com lembretes para beber água</span>
                                </li>
                                <li class="list-group-item d-flex align-items-center">
                                    <i class="fas fa-pills text-success me-3"></i>
                                    <span>Alerta para horário de medicamentos</span>
                                </li>
                                <li class="list-group-item d-flex align-items-center">
                                    <i class="fas fa-walking text-success me-3"></i>
                                    <span>Contador de passos e calorias gastas</span>
                                </li>
                                <li class="list-group-item d-flex align-items-center">
                                    <i class="fas fa-sync-alt text-success me-3"></i>
                                    <span>Sincronização automática com seu prontuário SUS</span>
                                </li>
                            </ul>
                            <div class="card bg-light">
                                <div class="card-body">
                                    <h5 class="card-title">Solicite seu Monitor SUS+Vida</h5>
                                    <form>
                                        <div class="mb-3">
                                            <label class="form-label">Tipo de Beneficiário</label>
                                            <select class="form-select">
                                                <option>Paciente SUS (gratuito)</option>
                                                <option>Contribuinte (custo simbólico R$59,90)</option>
                                            </select>
                                        </div>
                                        <button type="submit" class="btn btn-sus">Solicitar Agora</button>
                                    </form>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Seção de Login/Perfil -->
    <section class="py-5 bg-light" id="login">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-md-8 col-lg-6">
                    <div class="card shadow-sm">
                        <div class="card-body p-5">
                            <h3 class="card-title text-center mb-4"><i class="fas fa-user-circle text-success me-2"></i>Área do Paciente</h3>
                            <form id="loginForm">
                                <div class="mb-3">
                                    <label for="cpf" class="form-label">CPF</label>
                                    <input type="text" class="form-control" id="cpf" placeholder="000.000.000-00" required>
                                </div>
                                <div class="mb-3">
                                    <label for="senha" class="form-label">Senha</label>
                                    <input type="password" class="form-control" id="senha" required>
                                </div>
                                <div class="mb-3 form-check">
                                    <input type="checkbox" class="form-check-input" id="lembrar">
                                    <label class="form-check-label" for="lembrar">Lembrar meus dados</label>
                                </div>
                                <div class="d-grid gap-2">
                                    <button type="submit" class="btn btn-sus mb-2">
                                        <i class="fas fa-sign-in-alt me-2"></i>Entrar
                                    </button>
                                    <a href="#" class="btn btn-outline-success">
                                        <i class="fas fa-user-plus me-2"></i>Cadastrar
                                    </a>
                                </div>
                            </form>
                            <div class="text-center mt-3">
                                <a href="#" class="text-success">Esqueci minha senha</a>
                                <span class="mx-2">|</span>
                                <a href="#" class="text-success">Acessar com Certificado Digital</a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Rodapé -->
    <footer class="footer">
        <div class="container">
            <div class="row">
                <div class="col-md-4">
                    <h5><i class="fas fa-heartbeat me-2"></i>SUS+Vida</h5>
                    <p>Tecnologia a serviço da saúde pública, facilitando o acesso aos serviços do SUS com praticidade e inovação.</p>
                    <div class="social-links">
                        <a href="#" class="text-white me-2"><i class="fab fa-facebook-f"></i></a>
                        <a href="#" class="text-white me-2"><i class="fab fa-instagram"></i></a>
                        <a href="#" class="text-white me-2"><i class="fab fa-twitter"></i></a>
                        <a href="#" class="text-white"><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                <div class="col-md-2">
                    <h5>Links Rápidos</h5>
                    <ul class="list-unstyled">
                        <li><a href="#" class="text-white">Início</a></li>
                        <li><a href="#" class="text-white">Agendar Consulta</a></li>
                        <li><a href="#" class="text-white">Especialidades</a></li>
                        <li><a href="#" class="text-white">Cirurgias</a></li>
                        <li><a href="#" class="text-white">Monitor SUS+Vida</a></li>
                    </ul>
                </div>
                <div class="col-md-3">
                    <h5>Contato</h5>
                    <ul class="list-unstyled">
                        <li><i class="fas fa-phone me-2"></i>136 - Central SUS</li>
                        <li><i class="fas fa-envelope me-2"></i>contato@susvida.gov.br</li>
                        <li><i class="fas fa-map-marker-alt me-2"></i>Ministério da Saúde, Brasília/DF</li>
                    </ul>
                </div>
                <div class="col-md-3">
                    <h5>Acessibilidade</h5>
                    <a href="#" class="btn btn-outline-light btn-sm mb-2"><i class="fas fa-eye me-1"></i> Alto Contraste</a>
                    <a href="#" class="btn btn-outline-light btn-sm mb-2"><i class="fas fa-volume-up me-1"></i> Leitor de Tela</a>
                    <a href="#" class="btn btn-outline-light btn-sm"><i class="fas fa-sign-language me-1"></i> Libras</a>
                </div>
            </div>
            <hr class="mt-4 mb-3 bg-light">
            <div class="row">
                <div class="col-md-6">
                    <p class="mb-0">© 2024 SUS+Vida. Todos os direitos reservados.</p>
                </div>
                <div class="col-md-6 text-md-end">
                    <a href="#" class="text-white me-3">Termos de Uso</a>
                    <a href="#" class="text-white me-3">Política de Privacidade</a>
                    <a href="#" class="text-white">Acessibilidade</a>
                </div>
            </div>
        </div>
    </footer>

    <!-- Ferramentas de Acessibilidade -->
    <div class="accessibility-tools">
        <div class="btn-group dropup">
            <button type="button" class="btn btn-success dropdown-toggle" data-bs-toggle="dropdown" aria-expanded="false">
                <i class="fas fa-universal-access"></i>
            </button>
            <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#"><i class="fas fa-eye me-2"></i>Alto Contraste</a></li>
                <li><a class="dropdown-item" href="#"><i class="fas fa-volume-up me-2"></i>Leitor de Tela</a></li>
                <li><a class="dropdown-item" href="#"><i class="fas fa-text-height me-2"></i>Aumentar Fonte</a></li>
                <li><a class="dropdown-item" href="#"><i class="fas fa-sign-language me-2"></i>Libras</a></li>
            </ul>
        </div>
    </div>

    <!-- Modal de Login -->
    <div class="modal fade" id="loginModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title">Acesso ao SUS+Vida</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <form>
                        <div class="mb-3">
                            <label for="modalCpf" class="form-label">CPF</label>
                            <input type="text" class="form-control" id="modalCpf" placeholder="000.000.000-00">
                        </div>
                        <div class="mb-3">
                            <label for="modalSenha" class="form-label">Senha</label>
                            <input type="password" class="form-control" id="modalSenha">
                        </div>
                        <div class="d-grid gap-2">
                            <button type="submit" class="btn btn-sus">Entrar</button>
                            <a href="#" class="btn btn-outline-success">Cadastre-se</a>
                        </div>
                    </form>
                    <div class="text-center mt-3">
                        <a href="#" class="text-success">Acessar com Certificado Digital</a>
                    </div>
                </div>
                <div class="modal-footer justify-content-center">
                    <p class="mb-0">Ao acessar, você concorda com nossos <a href="#">Termos de Uso</a> e <a href="#">Política de Privacidade</a>.</p>
                </div>
            </div>
        </div>
    </div>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
    <script>
        // Simulação do analisador de sintomas
        document.getElementById('analisar-sintomas').addEventListener('click', function(e) {
            e.preventDefault();
            const sintomas = document.getElementById('sintomas-texto').value;
            
            if(!sintomas) {
                alert('Por favor, descreva seus sintomas antes de solicitar a análise.');
                return;
            }
            
            // Simulação de análise de IA
            document.getElementById('resultado-sintomas').classList.add('d-none');
            document.getElementById('orientacao-ia').classList.remove('d-none');
            
            // Simulação de resposta variada
            const respostas = [
                "Baseado nos sintomas relatados, recomendamos que você agende uma consulta com um clínico geral nos próximos dias. Enquanto isso, mantenha repouso e hidratação adequada.",
                "Os sintomas descritos podem indicar uma condição que requer avaliação médica urgente. Recomendamos que você procure uma Unidade de Pronto Atendimento (UPA) mais próxima.",
                "A análise preliminar sugere que seus sintomas podem ser tratados inicialmente em casa com repouso e medicamentos básicos. Porém, se os sintomas persistirem por mais de 48 horas ou se agravarem, procure atendimento médico.",
                "Os sintomas relatados são inespecíficos. Recomendamos monitoramento por 24 horas e, havendo febre acima de 38°C ou piora dos sintomas, buscar atendimento médico."
            ];
            
            // Escolhe uma resposta aleatória para simulação
            const respostaAleatoria = respostas[Math.floor(Math.random() * respostas.length)];
            document.getElementById('texto-orientacao').textContent = respostaAleatoria;
        });
        
        // Simulação do botão de gravação
        document.getElementById('btn-gravacao').addEventListener('click', function(e) {
            e.preventDefault();
            alert('Funcionalidade de gravação por voz será implementada em breve!');
        });
        
        // Validação simples do formulário de login
        document.getElementById('loginForm').addEventListener('submit', function(e) {
            e.preventDefault();
            const cpf = document.getElementById('cpf').value;
            const senha = document.getElementById('senha').value;
            
            if(cpf && senha) {
                alert('Login realizado com sucesso! Redirecionando para sua área...');
            } else {
                alert('Por favor, preencha todos os campos.');
            }
        });
    </script>
</body>
</html>
