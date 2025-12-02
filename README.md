<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8"/>
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Clube Essencial do Consultório — Mobile</title>
  <meta name="description" content="Clube Essencial do Consultório — organização prática para médicos. Materiais semanais, áudios e aulas ao vivo. Vagas fundadoras. R$79/mês." />
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;700&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">
  <style>
    /* MOBILE-FIRST: espaçamento generoso, tipografia legível, botões largos */
    :root{
      --bg:#fbfaf8;
      --card:#ffffff;
      --text:#151515;
      --muted:#6e6e6e;
      --accent:#bfa56a;
      --accent-strong:#9f834d;
      --gap:18px;
      --radius:12px;
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;font-family:Inter,system-ui,Arial,sans-serif;background:var(--bg);color:var(--text);-webkit-font-smoothing:antialiased}
    a{color:inherit;text-decoration:none}
    .wrap{max-width:780px;margin:0 auto;padding:18px}
    .top{
      display:flex;align-items:center;justify-content:space-between;gap:12px;margin-bottom:14px;
    }
    .logo{
      display:flex;align-items:center;gap:12px;
    }
    .logo-badge{
      width:52px;height:52px;border-radius:10px;background:linear-gradient(135deg, rgba(191,165,106,0.12), rgba(159,131,77,0.06));display:flex;align-items:center;justify-content:center;font-family:'Playfair Display',serif;color:var(--accent-strong);font-weight:700;font-size:18px;border:1px solid rgba(159,131,77,0.08)
    }
    .brand-title{font-family:'Playfair Display',serif;font-size:15px;margin:0}
    .brand-sub{font-size:12px;color:var(--muted);margin:0}

    /* HERO CARD */
    .hero{
      background:var(--card);border-radius:var(--radius);padding:16px;box-shadow:0 8px 24px rgba(20,20,20,0.04);border:1px solid rgba(16,16,16,0.03);
      margin-bottom:16px;
    }
    .kicker{display:inline-block;padding:6px 10px;border-radius:999px;background:rgba(191,165,106,0.12);color:var(--accent-strong);font-weight:600;font-size:12px;margin-bottom:8px}
    .hero h1{font-family:'Playfair Display',serif;font-size:20px;margin:6px 0;color:#111}
    .hero p.lead{margin:8px 0 12px 0;color:var(--muted);font-size:14px;line-height:1.45}

    .quick-feats{display:flex;gap:8px;overflow:auto;padding-top:6px;padding-bottom:6px}
    .feat{
      min-width:150px;background:linear-gradient(180deg,#fff,#fbfaf8);padding:10px;border-radius:10px;border:1px solid rgba(16,16,16,0.03);font-size:13px;color:var(--muted)
    }

    /* CTA sticky-ish visual */
    .cta-box{background:linear-gradient(180deg,#fff,#fbfaf8);padding:14px;border-radius:12px;border:1px solid rgba(159,131,77,0.08);box-shadow:0 12px 28px rgba(159,131,77,0.05);display:flex;flex-direction:column;gap:10px;margin-bottom:16px}
    .price-row{display:flex;align-items:baseline;justify-content:space-between;gap:12px}
    .price{font-family:'Playfair Display',serif;font-size:24px;color:var(--accent-strong);font-weight:700}
    .sub{font-size:13px;color:var(--muted)}
    .btn{
      display:block;width:100%;text-align:center;padding:12px 14px;border-radius:10px;background:var(--accent-strong);color:#fff;font-weight:700;font-size:15px;box-shadow:0 10px 22px rgba(159,131,77,0.18)
    }
    .btn-secondary{display:block;width:100%;text-align:center;padding:10px 12px;border-radius:10px;border:1px solid rgba(16,16,16,0.06);background:transparent;color:var(--text);font-weight:600;font-size:14px}

    /* content blocks stack */
    .card{background:var(--card);border-radius:12px;padding:14px;border:1px solid rgba(11,11,11,0.03);box-shadow:0 8px 20px rgba(14,14,14,0.03);margin-bottom:14px}
    h2{font-family:'Playfair Display',serif;font-size:18px;margin:0 0 8px 0}
    h3{font-family:'Playfair Display',serif;font-size:16px;margin:0 0 8px 0}
    p{margin:0 0 10px 0;color:var(--muted);font-size:14px;line-height:1.5}
    ul{padding-left:18px;margin:6px 0;color:var(--muted)}
    li{margin-bottom:8px}

    /* testimonials */
    .testi{display:flex;flex-direction:column;gap:8px}
    .testi p{color:#333;font-size:14px;margin:0}
    .author{font-weight:700;color:var(--text);font-size:13px}

    /* FAQ compact */
    .faq .q{font-weight:700;color:var(--text);margin-top:10px}
    .faq .a{color:var(--muted);font-size:14px;margin-top:6px}

    /* footer compact */
    .footer{display:flex;flex-direction:column;gap:6px;align-items:center;color:var(--muted);font-size:13px;padding:12px 0}

    /* larger screens keep refined layout */
    @media(min-width:760px){
      .wrap{padding:28px}
      .hero{display:flex;gap:20px;align-items:flex-start}
      .hero-left{flex:1}
      .side-cta{width:360px;flex:0 0 360px}
      .quick-feats{flex-wrap:wrap}
      .card-row{display:grid;grid-template-columns:1fr 1fr;gap:18px}
    }
  </style>
</head>
<body>
  <div class="wrap" role="main">

    <!-- TOP -->
    <header class="top" aria-label="cabecalho">
      <div class="logo">
        <div class="logo-badge">FS</div>
        <div>
          <div class="brand-title">Clube Essencial do Consultório</div>
          <div class="brand-sub">Isa Fernanda — FS Consultoria</div>
        </div>
      </div>
      <div style="text-align:right">
        <div style="font-weight:600;color:var(--muted);font-size:13px">Vagas Fundadoras</div>
        <div style="font-weight:700;color:var(--accent-strong);font-size:15px">R$ 79 / mês</div>
      </div>
    </header>

    <!-- HERO -->
    <section class="hero" aria-labelledby="hero-title">
      <div class="hero-left" id="hero-title">
        <div class="kicker">Essencial • Prático • Imediato</div>
        <h1>Organização prática. Rotina leve. Consultório lucrativo.</h1>
        <p class="lead">Materiais semanais e ações rápidas para médicos que querem sair da improvisação e ter um consultório previsível — em 10 minutos por dia.</p>

        <div class="quick-feats" aria-hidden="false">
          <div class="feat"><strong>Aplicável amanhã</strong><div style="font-size:12px;margin-top:6px;color:var(--muted)">Fluxos, scripts e checklists prontos</div></div>
          <div class="feat"><strong>Conciso</strong><div style="font-size:12px;margin-top:6px;color:var(--muted)">Áudios e ações curtas</div></div>
          <div class="feat"><strong>Foco em resultado</strong><div style="font-size:12px;margin-top:6px;color:var(--muted)">Reduz faltas e melhora retenção</div></div>
        </div>
      </div>
    </section>

    <!-- CTA Box (visível rápido) -->
    <aside class="cta-box" aria-label="oferta-principal">
      <div class="price-row">
        <div>
          <div style="font-size:12px;color:var(--muted);font-weight:600">Vagas Fundadoras</div>
          <div class="price">R$ 79 <span style="font-size:13px;color:var(--muted);font-weight:600">/ mês</span></div>
        </div>
        <div style="text-align:right" class="sub">Cancelar a qualquer momento</div>
      </div>

      <div style="font-size:14px;color:var(--muted)">Acesso imediato ao material da semana + bônus de lançamento. Entregas semanais práticas.</div>

      <!-- ATENÇÃO: substituir o link abaixo pelo link real de pagamento -->
      <a class="btn" href="https://pagamento.exemplo.com/checkout?produto=clube-essencial" target="_blank" rel="noopener noreferrer">Entrar agora — Pagar R$79</a>
      <a class="btn-secondary" href="mailto:consultoriaisasouza@gmail.com?subject=Quero%20saber%20mais%20sobre%20o%20Clube">Falar com Isa — tirar dúvida</a>

      <div style="font-size:13px;color:var(--muted)">Bônus: PDF "Fluxo completo de atendimento particular" + Áudio "Primeiros 90 dias".</div>
    </aside>

    <!-- WHAT YOU GET -->
    <section class="card" aria-label="o-que-voce-recebe">
      <h2>O que você recebe todas as semanas</h2>
      <p>Materiais pensados para aplicar imediatamente no consultório — sem teoria extensa.</p>
      <ul>
        <li><strong>PDF prático semanal:</strong> modelos, scripts, checklists e fluxos prontos.</li>
        <li><strong>Áudio curto semanal:</strong> orientação direta para aplicar no dia seguinte.</li>
        <li><strong>Guia de ação:</strong> tarefa simples de 10 minutos para cada semana.</li>
        <li><strong>Aula mensal ao vivo:</strong> perguntas rápidas e ajustes práticos.</li>
      </ul>
    </section>

    <!-- RESULTS -->
    <section class="card" aria-label="resultados">
      <h2>Resultados que você verá</h2>
      <p>Menos improviso, mais previsibilidade e mais caixa — com passos práticos.</p>
      <ul>
        <li>Agenda organizada e confirmada</li>
        <li>Fluxo de atendimento com padrão profissional</li>
        <li>Rotina de cobrança sem atrito</li>
        <li>Redução de faltas e cancelamentos</li>
      </ul>
    </section>

    <!-- AUTHORITY -->
    <section class="card" aria-label="quem-conduz">
      <h2>Quem conduz</h2>
      <p><strong>Isa Fernanda Souza Silva</strong> — consultora empresarial focada em consultórios médicos. Trabalho prático e direto para transformar rotina em resultado.</p>
      <p style="font-size:13px;color:var(--muted)">FS Consultoria — projetos entregues na Região dos Lagos e online, com foco em resultado financeiro e qualidade de atendimento.</p>
    </section>

    <!-- TESTIMONIALS -->
    <section class="card" aria-label="depoimentos">
      <h2>Depoimentos</h2>
      <div class="testi">
        <div class="test">
          <p>"As orientações reorganizaram minha agenda e reduziram faltas em 30% no primeiro mês."</p>
          <div class="author">— Médico (RJ)</div>
        </div>
        <div class="test">
          <p>"Os modelos de scripts e rotinas são diretos. Usei na semana seguinte e economizei tempo."</p>
          <div class="author">— Psicóloga Clínica</div>
        </div>
      </div>
      <p style="font-size:12px;color:var(--muted);margin-top:8px">Depoimentos com foto e cargo aumentam conversão — adicione quando tiver.</p>
    </section>

    <!-- INVESTMENT & BUY -->
    <section class="card" aria-label="investimento">
      <h2>Investimento & Bônus</h2>
      <p>Vagas fundadoras — preço promocional e benefícios por tempo limitado.</p>
      <ul>
        <li><strong>R$ 79 / mês</strong> — acesso completo</li>
        <li><strong>Bônus:</strong> PDF "Fluxo completo de atendimento particular"</li>
        <li><strong>Bônus:</strong> Áudio "Primeiros 90 dias para um consultório previsível"</li>
      </ul>
      <div style="margin-top:10px">
        <a class="btn" href="https://pagamento.exemplo.com/checkout?produto=clube-essencial" target="_blank" rel="noopener noreferrer">Entrar agora — Pagar R$79</a>
      </div>
    </section>

    <!-- FAQ -->
    <section class="card faq" aria-label="faq">
      <h2>Perguntas rápidas</h2>
      <div class="q">Como recebo o material?</div>
      <div class="a">Por e-mail e em uma área de membros (Notion / página privada). Áudios e PDFs disponíveis para download.</div>

      <div class="q">Preciso participar ao vivo?</div>
      <div class="a">Não — as aulas são gravadas e ficam disponíveis para quem não puder assistir.</div>

      <div class="q">Tem fidelidade?</div>
      <div class="a">Não. Cancelamento simples e sem burocracia.</div>

      <div class="q">Substitui consultoria individual?</div>
      <div class="a">Não. O clube é solução prática e recorrente. Para implementação personalizada, recomendo consultoria individual.</div>

      <div class="q">Reembolso?</div>
      <div class="a">Reembolso nos primeiros 7 dias mediante solicitação — casos analisados individualmente.</div>
    </section>

    <!-- FOOTER -->
    <footer class="footer" role="contentinfo">
      <div style="font-weight:700">FS Consultoria — Clube Essencial do Consultório</div>
      <div style="font-size:13px;color:var(--muted)">Isa Fernanda • consultoriaisasouza@gmail.com</div>
      <div style="font-size:12px;color:var(--muted)">© <span id="yr"></span> FS Consultoria. Política de Privacidade • Termos de Uso</div>
    </footer>

  </div>

  <script>
    document.getElementById('yr').textContent = new Date().getFullYear();
  </script>
</body>
</html>