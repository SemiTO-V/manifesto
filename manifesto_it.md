\documentclass{article}
\usepackage{graphicx} % Required for inserting images

\title{Manifesto di SemiTO-V}
\author{Tan Siret Akıncı}
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

\subsection{Cosa Facciamo}

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

\subsection{Il Nostro Approccio}

\paragraph{Open Source Sempre e Comunque:}

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

\section{Unisciti a Noi}

Se sei appassionato di architetture di processori, circuiti elettronici digitali, linguaggi di descrizione dell'hardware, compilatori o software di basso livello — vieni a costruire con noi! Noi costruiamo processori!

\paragraph{Inviare le candidature a: semitofive@gmail.com}

\subparagraph{\textit{SemiTO-V: Team Studentesco RISC-V del Politecnico di Torino}}
\end{document}

