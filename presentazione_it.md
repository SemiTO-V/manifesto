\documentclass{article}
\usepackage{graphicx} % Required for inserting images
\usepackage{hyperref} % Required for better link formatting
\usepackage{mwe} % Better pictures
\usepackage{float} % Better placement

\title{Presentazione Team Studentesco "SemiTO-V"}
\author{Tan Siret Akıncı - Maurizio Contu - Vincenzo Butera}
\date

\begin{document}
\maketitle
\begin{center}
    \includegraphics[scale=0.7]{semito-v_logo.png}
\end{center}
\maketitle

\section{Visione}

SemiTO-V immagina un futuro in cui l'informatica sia veramente democratizzata — un futuro in cui sia il software che l'hardware siano completamente open-source, liberi da scatole nere (black box), restrizioni proprietarie e dipendenza da fornitori (vendor lock-in). Questo futuro è reso possibile da RISC-V, l'ISA (Instruction Set Architecture) aperta, che, grazie a un enorme supporto industriale, sblocca innovazione, collaborazione e accessibilità senza precedenti nell'informatica. Come studenti, miriamo a partecipare a questa rivoluzione informatica. In linea con questa visione, vogliamo costruire le nostre carriere in campi correlati a RISC-V e contribuire a RISC-V sia come studenti universitari che come laureati. Per raggiungere questo obiettivo, crediamo che il modo migliore per iniziare sia formare un team studentesco dedicato all'ISA RISC-V e alle tecnologie ad essa correlate.

\section{Missione}
SemiTO-V è un team studentesco che utilizza core basati sull'ISA RISC-V per creare processori personalizzati, firmware e software, nonché i nostri design di PCB, a livello dell'educazione triennale/magistrale. Stiamo padroneggiando tutto, dall'analisi dei circuiti all'architettura dei processori, e dalla progettazione RTL allo sviluppo software di basso livello per piattaforme RISC-V (RV32 e potenzialmente RV64). La nostra missione è utilizzare, sfruttare e migliorare i core RISC-V standardizzati/popolari, realizzando i nostri design di processori (MCU, PPU ecc.), progettando i nostri PCB con FPGA e altri componenti per eseguirli, ottimizzandoli per applicazioni del mondo reale (IMU, acceleratore AI ecc.) migliorando al contempo il loro ecosistema software/firmware e confrontandoli (benchmarking) con altri chip. Il problema principale dell'hardware RISC-V esistente è la mancanza di una buona compatibilità firmware e software. Per questo motivo, vogliamo concentrarci sulla massimizzazione delle prestazioni, dell'efficienza energetica e del supporto software per i chip RISC-V esistenti, assicurando che siano pienamente utilizzati in sistemi embedded, cloud, edge computing, HPC e oltre.

\section{Lavoro principale}

\paragraph{Sviluppo Hardware e Logico:}

\begin{itemize}
    \item Utilizzare core basati sull'ISA RISC-V (RV32/RV64), aggiungere istruzioni e moduli personalizzati
    \item Implementare SoC (System on Chip) mirati a FPGA
    \item Interfacciarsi con periferiche, rendere i nostri processori abilitati al Wi-Fi.
    \item Progettare PCB open source basati su chip FPGA e ASIC
    \item Esplorare funzionalità avanzate come il pipelining e l'elaborazione parallela (potenzialmente per HPC)
\end{itemize}
\paragraph{Sviluppo Software e Istruzioni:}

\begin{itemize}
    \item Sviluppare/migliorare implementazioni di firmware bare-metal, RTOS (FreeRTOS) e OS time-sharing (Linux per RV64)
    \item Eseguire il porting e ottimizzare i compilatori per i nostri processori
    \item Contribuire al software importante per l'ecosistema RISC-V (kernel Linux, LLVM, librerie vettoriali)
    \item Creare i nostri SDK, toolchain e simulatori per i nostri design
    \item Sviluppare benchmark/configurare quelli esistenti per eseguire test sui nostri design e su quelli esistenti, confrontando le prestazioni delle tecnologie RISC-V
\end{itemize}

\section{Il Nostro Approccio}

\paragraph{Open Source:}

\begin{itemize}
    \item Tutti i nostri design, codici e documentazione risiedono in repository pubblici
    \item Costruiamo su progetti RISC-V open source e contribuiamo ad essi
    \item Documentiamo tutto
\end{itemize}

\paragraph{Apprendimento Pratico:}

\begin{itemize}
    \item Imparare facendo: Progettare, programmare, testare, iterare
    \item Imparare seguendo e utilizzando le più recenti tecnologie basate su RISC-V
    \item Applicare la teoria appresa in aula utilizzando schede FPGA, progettando circuiti digitali complessi per realizzare le nostre schede, basandoci su architetture di processori aperte e utilizzando linguaggi di programmazione di basso livello per lo sviluppo di firmware/software
\end{itemize}

\paragraph{Focus sulla Comunità:}

\begin{itemize}
    \item Condividere la conoscenza attraverso workshop e tutorial
    \item Collaborare con altri gruppi RISC-V a livello globale
    \item Collegare mondo accademico, spazio utente (userspace) e industria attraverso la filosofia open source
\end{itemize}

\paragraph{Focus sul Settore:}

\begin{itemize}
    \item Conoscere le industrie dei chip e di RISC-V
    \item Testare in beta gli ultimi prodotti RISC-V open source e contribuire al loro sviluppo (RISC-V Development Partner Program, Codasip Studio Uni Program, ambasciatori del Deepcomputing Framework)
    \item Condividere i nostri progetti con le aziende per valutazione
    \item Scoprire opportunità di stage e lavoro relative a RISC-V grazie ai progetti del team
\end{itemize}

\section{Aree operative e ruoli del lavoro}
\begin{figure}[H]
    \centering
    \includegraphics[width=0.9\linewidth]{semitofive_hierarchy.png}
    \caption{La gerarchia semplificata del team}
    \label{fig:enter-label}
\end{figure}
A SemiTO-V abbiamo diversi ruoli sotto 3 aree che comprendono diverse discipline, sempre allineate con la nostra missione delle technologie basate su RISC-V ISA.

\subsection{Area Hardware and Logic Dev (HW)}
\begin{itemize}
    \item \textbf{Missione}: Contribuire allo sviluppo di disegno logica (implementazione delle architetture, core, CPU/MCU e moduli basati su RISC-V per i FPGA) e hardware intorno (progettazione degli circuiti e segnali, disegno degli PCB). Progettare disegni innovative, affidabili, aperte e documentate, valorizzando l'apprendimento pratico e il rigore tecnico.
    
    \item \textbf{Struttura}: L'area è organizzata per progetti. Ogni progetto è autonomo e coordinato da un capoprogetto HW, eletto tra i membri attivi dell'area. L'area può essere articolata nei seguenti ruoli:
    \begin{itemize}
        \item Ingegneri di sviluppo FPGA/descrizioni di logica
        \item Ingegneri elettronici delle schede
        \item Ingegneri di sviluppo embedded (hardware)
        \item Ingegneri di rete wireless
    \end{itemize}
\end{itemize}

\subsection{Area Software and Instruction Dev (SW)}
\begin{itemize}
    \item \textbf{Missione}: Contribuire allo sviluppo di soluzioni software e istruzioni per i processori RISC-V sia disegnato dentro club che già progettato in modo innovativo, robuste, accessibili e documentate, favorendo l'apprendimento, la sperimentazione e la diffusione della conoscenza tecnica.
    
    \item \textbf{Struttura}: L'area è organizzata su base progettuale. Ogni progetto software e di istruzioni personalizzati è coordinato da un Capoprogetto SW, eletto tra i membri attivi dell'area. L'area puo essere articolata in seguenti ruoli:
    \begin{itemize}
        \item Programmatori low-level di RISC-V assembly (RV32/RV64)
        \item Programmatori di sistemi operativi per RISC-V (Linux per RV64, RTOS per RV32)
        \item Ingegneri di firmware
        \item Ingegneri di sviluppo embedded (software)
        \item Architetti di calcolatori
    \end{itemize}
\end{itemize}

\subsection{Area Public Relations (PR) e Team Lead}

\begin{itemize}
    \item \textbf{Missione}: Curare i rapporti istituzionali, assicurare il supporto burocratico e logistico alle attività tecniche, promuovere l'immagine del team e garantirne la sostenibilità economica nel tempo.
    
    \item \textbf{Struttura}: L'area è articolata in quattro ruoli principali:
    \begin{itemize}
        \item Responsabile Amministrativo
        \item Responsabile Fundraising e Sponsorship
        \item Responsabile Eventi e Competizioni
        \item Responsabile Comunicazione
    \end{itemize}
\end{itemize}

\section{Attivita pre-fondazione}
Da quando abbiamo formato il nostro team in modo informale, a gennaio, eravamo in fase di brainstorming, ma non siamo rimasti fermi. Abbiamo:
\begin{itemize}
    \item Acquistato MCU basati su RV32 (ESP32 C6, RP2350) e ci abbiamo giocato, sviluppando software bare-metal e FreeRTOS, testando interfacce I2C/SPI/altre tramite l'assemblaggio RV32.
    \item Acquistato FPGA Tang Nano 9K a basso costo e ho eseguito alcuni core preliminari.
    \item Partecipato al RISC-V Hackathon del 10-14 aprile 2025. Abbiamo ridotto il conteggio dei cicli di un processore RV32I con un piccolo LLM da 29360 a 4839 (-25121, 83,85 percento) implementando istruzioni personalizzate su Codasip Studio.
    \item Incontro con Yuning Liang, CEO di DeepComputing. Abbiamo effettuato una settimana di beta testing eseguendo whisper.cpp sul prototipo di PC DC ROMA AI. Un nostro membro ha partecipato al RISC-V Summit del 12-15 maggio 2025 con questo progetto sotto la sponsorizzazione di DeepComputing.
\end{itemize}

\begin{figure}[H]
    \includegraphics[width=.45\textwidth]{hackathon.png}\hfill
    \includegraphics[width=.45\textwidth]{karavar.png}\hfill
    \\[\smallskipamount]
    \includegraphics[width=.45\textwidth]{dcromaaipcmotherboard.png}\hfill
    \includegraphics[width=.45\textwidth]{dcromaaitesting.png}
    \\[\smallskipamount]
    \caption{In senso orario dall'alta sinistra: [1] Partecipanti al RISC-V Hackathon April 2025 dal SemiTO-V Community. [2] Fotogramma dal video di presentazione del nostro Hackathon realizzato da Ece Karavar. [3] Test dimostrativo del modello whisper.cpp ai su DC ROMA AI PC, con benchmark rispetto a Raspberry Pi 4B 2gb di ram. [4] La motherboard del prototipo DC ROMA AI PC accanto all'MCU MILK-V Duo RV64 e all'MCU ESP32 C3 RV32.}\label{fig:foobar}
\end{figure}

\section{Fase 1 del nostro Roadmap: Avvio del progetto (Maggio 2025 - Ottobre 2025)}
Iniziare la creazione di un MCU basato su RV32 come primo progetto del team. Utilizzare un core RV32 già esistente. Costruire competenze fondamentali e infrastruttura di base.

\subsection{Hardware}
\begin{itemize}
    \item Selezionare un core RV32 (OpenHW, lowRISC ecc.)
    \item Ordinare una scheda FPGA popolare per iniziare a provare core e MCU già esistenti (FPGA basate su Diligent e Xilinx, come Nexys A7 e ZYNQ)
    \item Ordinare una scheda FPGA che contenga un chip FPGA compatibile con toolchain open source e che sia popolare nella comunità RISC-V (OrangeCrab basata su ECP5, Olimex basata su GateMate A1 di Cologne Chips)
    \item Ordinare periferiche di base per testare la comunicazione (LCD di base, LED, cavi, schermo VGA ecc.)
    \item Ordinare MCU basati su RV32 per sperimentare ed eseguire benchmark rispetto alle implementazioni FPGA (ESP32C6, Raspberry Pi Pico 2, CH32V003)
    \item Configurare le toolchain FPGA (Yosys/nextpnr per quelle che li supportano)
    \item Eseguire un core minimale con GPIO e alcune altre interfacce
\end{itemize}

\subsection{Software}
\begin{itemize}
    \item Sviluppare software bare-metal di base (benchmark, demo) per MCU RV32 già esistenti e design che eseguiremo su FPGA, confrontare le prestazioni
    \item Eseguire test GPIO di base
    \item Testare la toolchain RISC-V (GCC/LLVM) su MCU RV32 già esistenti e sul nostro design su FPGA
    \item Testare vari benchmark su MCU RV32 già esistenti e sul nostro design su FPGA
\end{itemize}

\subsection{PR e Promozione}
\begin{itemize}
    \item Realizzare poster, magliette e altro materiale promozionale
    \item Prepararsi per le attività di reclutamento aprendo stand nel campus principale del PoliTO
    \item Ricercare hackathon/competizioni a cui possiamo partecipare (RISC-V Hackathon, FPGA Hackathon, competizioni Hackster.io)
    \item Ricercare e candidarsi per eventi a cui possiamo partecipare dove possiamo vedere l'industria RISC-V da vicino (RISC-V Summit Europe, Embedded World)
\end{itemize}

Per prendere visione della roadmap completa e altri file in dettaglio, Vi invitiamo a consultare il nostro repository pubblico su GitHub al seguente link: \url{https://github.com/semito-v/team-docs}

\subparagraph{\textit{SemiTO-V: Team Studentesco RISC-V del Politecnico di Torino}}
\end{document}

