<!DOCTYPE html>
<html lang="fr">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Virtual Lab - Pentest avec Metasploit</title>
    <link rel="stylesheet" href="main2.css" />
  </head>
  <body>
    <div class="header">
      <h1>🔒 Virtual Lab - Pentest avec Metasploit</h1>
      <p>
        Rapport académique sur la sécurité offensive et les tests d'intrusion
      </p>
      <div class="badges">
        <span class="badge">🛡️ Cybersécurité</span>
        <span class="badge">🔍 Pentest</span>
        <span class="badge">⚙️ Metasploit</span>
        <span class="badge">🌐 pfSense</span>
        <span class="badge">🖥️ Virtual Lab</span>
      </div>
    </div>

    <div class="container">
      <div class="section">
        <h2>📋 À propos du projet</h2>
        <p>
          Ce rapport présente un laboratoire virtuel complet de test d'intrusion
          utilisant <strong>Metasploit Framework</strong>. Le projet démontre
          une méthodologie professionnelle de pentest, de la reconnaissance
          réseau à l'exploitation avancée avec pivoting.
        </p>

        <div class="highlight-box">
          <h3>🎯 Objectifs du projet</h3>
          <ul style="margin-left: 1.5rem; margin-top: 0.5rem">
            <li>
              Mettre en place un environnement virtuel sécurisé pour les tests
              d'intrusion
            </li>
            <li>
              Configurer un pare-feu pfSense avec règles de filtrage
              personnalisées
            </li>
            <li>Exploiter des vulnérabilités avec Metasploit Framework</li>
            <li>
              Réaliser des attaques avancées (pivoting, pass-the-hash, brute
              force)
            </li>
            <li>
              Documenter les techniques d'exploitation et recommandations de
              sécurité
            </li>
          </ul>
        </div>
      </div>

      <div class="section">
        <h2>🎓 Compétences développées</h2>
        <div class="highlight-box">
          <ul style="margin-left: 1.5rem">
            <li>
              <strong>Reconnaissance réseau</strong> : Nmap, arp-scan,
              énumération de services
            </li>
            <li>
              <strong>Exploitation de vulnérabilités</strong> : Metasploit,
              attaques brute force, exploitation MySQL
            </li>
            <li>
              <strong>Post-exploitation</strong> : Meterpreter, extraction de
              hash, pass-the-hash
            </li>
            <li>
              <strong>Techniques avancées</strong> : Pivoting, proxy SOCKS,
              routage réseau
            </li>
            <li>
              <strong>Craquage de mots de passe</strong> : John the Ripper,
              analyse de hashes
            </li>
            <li>
              <strong>Configuration pare-feu</strong> : pfSense, règles de
              filtrage, segmentation réseau
            </li>
            <li>
              <strong>Accès à distance</strong> : RDP, FTP, contrôle graphique
            </li>
          </ul>
        </div>
      </div>

      <div class="section" id="menu-rapport">
        <h2>📚 Contenu Détaillé du Rapport</h2>
        <div class="tools-grid">
          <div class="tool-card tool-toggle">
            <div class="tool-icon">🎯</div>
            <div class="tool-name">Metasploit 6</div>
            <a href="#metasploit-install" class="tool-desc-link">
              <div class="tool-desc">
                Présentation et installation du Framework
              </div>
            </a>
          </div>

          <div class="tool-card tool-toggle">
            <div class="tool-icon">⚙️</div>
            <div class="tool-name">Laboratoire virtuel</div>
            <a href="#config-reseau-detail" class="tool-desc-link">
              <div class="tool-desc">
                Configuration réseau des machines cibles et de la machine
                attaquante
              </div>
            </a>
          </div>

          <div class="tool-card tool-toggle">
            <div class="tool-icon">🛡️</div>
            <div class="tool-name">pfSense</div>
            <a href="#pfsense-detail" class="tool-desc-link">
              <div class="tool-desc">
                Organisation du réseau avec Pare-feu et routeur open source
              </div>
            </a>
          </div>

          <div class="tool-card large-grouping-card tool-toggle">
            <div class="tool-icon">💣</div>
            <div class="tool-name">Phases d'attaques / Outils Pentest</div>
            <a href="#outils-pentest-resume" class="tool-desc-link">
              <div class="tool-desc">
                Outils clés utilisés pour l'exploitation et la
                post-exploitation.
              </div>
            </a>

            <div class="grouped-tools-list">
              <a href="#nmap-scan" class="grouped-tool-link">
                <div class="grouped-tool-item">
                  <div class="icon">🔍</div>
                  <div class="label">Nmap : Scan et énumération</div>
                </div>
              </a>
              <a href="#meterpreter-payload" class="grouped-tool-link">
                <div class="grouped-tool-item">
                  <div class="icon">💻</div>
                  <div class="label">Meterpreter : Payload avancé</div>
                </div>
              </a>
              <a href="#john-the-ripper" class="grouped-tool-link">
                <div class="grouped-tool-item">
                  <div class="icon">🔓</div>
                  <div class="label">
                    John the Ripper : Craquage de mots de passe
                  </div>
                </div>
              </a>
              <a href="#proxychains-pivoting" class="grouped-tool-link">
                <div class="grouped-tool-item">
                  <div class="icon">🌐</div>
                  <div class="label">Proxychains : Routage et Pivoting</div>
                </div>
              </a>
            </div>
          </div>
        </div>
      </div>

      <div class="section content-section" id="metasploit-install">
        <h2>🎯 Installation de Metasploit Framework</h2>
        <div class="highlight-box" style="margin-top: 2rem">
          <a href="#menu-rapport" class="btn" style="background: #38b4ff">
            ⬅️ Revenir au menu du rapport
          </a>
        </div>
      </div>

      <div class="section content-section" id="nmap-scan">
        <h2>🔍 Nmap : Scan et énumération</h2>
        <div class="highlight-box" style="margin-top: 2rem">
          <a href="#menu-rapport" class="btn" style="background: #38b4ff">
            ⬅️ Revenir au menu du rapport
          </a>
        </div>
      </div>

      <div class="section">
        <a href="#" class="btn secondary-btn"
          >⭐ Mes autres projets sur GitHub</a
        >
      </div>
    </div>

    <div class="footer">
      <p>🔐 Projet réalisé dans un cadre académique et éthique</p>
      <p style="margin-top: 0.5rem; font-size: 0.9rem">
        Les techniques présentées sont destinées uniquement à des fins
        éducatives et doivent être utilisées de manière responsable.
      </p>
    </div>
    <script>
      document.addEventListener("DOMContentLoaded", () => {
        const toggles = document.querySelectorAll(".tool-toggle");
        const allLinks = document.querySelectorAll(
          ".tool-desc-link, .grouped-tool-link"
        );

        // 1. GESTION DE L'ACCORDÉON (Clic sur la carte DIV)
        toggles.forEach((card) => {
          card.addEventListener("click", (e) => {
            // S'assurer que le clic n'est pas sur un lien interne (qui gère la navigation)
            if (e.target.closest("a")) {
              return;
            }

            const isExpanded = card.classList.contains("is-expanded");

            // Ferme toutes les cartes actuellement ouvertes
            document
              .querySelectorAll(".tool-toggle.is-expanded")
              .forEach((openCard) => {
                openCard.classList.remove("is-expanded");
              });

            // Ouvre ou ferme la carte cliquée
            if (!isExpanded) {
              card.classList.add("is-expanded");
            }
          });
        });

        // 2. GESTION DU LIEN ET DU SURLIGNAGE
        allLinks.forEach((link) => {
          link.addEventListener("click", (e) => {
            // Retire le surlignage de tous les liens
            allLinks.forEach((l) => l.classList.remove("is-selected"));

            // Applique le surlignage au lien cliqué
            link.classList.add("is-selected");

            // Ferme l'accordéon après la sélection (bonne UX)
            const parentCard = link.closest(".tool-toggle");
            if (parentCard) {
              parentCard.classList.remove("is-expanded");
            }

            // Le comportement par défaut du lien (navigation vers le #hash) s'exécute ensuite.
          });
        });

        // GESTION DU SURLIGNAGE AU CHARGEMENT DE LA PAGE (si un hash est présent dans l'URL)
        const currentHash = window.location.hash;
        if (currentHash) {
          const targetLink = document.querySelector(`a[href="${currentHash}"]`);
          if (targetLink) {
            targetLink.classList.add("is-selected");
          }
        }
      });
    </script>
  </body>
</html>
