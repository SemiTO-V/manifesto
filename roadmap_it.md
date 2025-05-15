\documentclass{article}
\usepackage{graphicx} % Required for inserting images

\title{Prima Roadmap Annuale di SemiTO-V}
\author{Tan Siret Akıncı}
\date

\begin{document}
\maketitle
\begin{center}
    \includegraphics[scale=0.7]{semito-v_logo.png}
\end{center}

\section{Fase 1: Avvio del progetto (Maggio 2025 - Ottobre 2025)}
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

\section{Fase 2: Sviluppo del Core (Novembre 2025 - Gennaio 2026)}
Migliorare le capacità del nostro MCU basato su RV32.

\subsection{Hardware}
\begin{itemize}
    \item Integrare periferiche SPI/I2C
    \item Implementare DMA di base
    \item Aggiungere istruzioni personalizzate (opzionale)
    \item Iniziare la progettazione del PCB che conterrà un chip FPGA e altri componenti/periferiche per eseguire il nostro MCU
\end{itemize}

\subsection{Software}
\begin{itemize}
    \item Eseguire il porting di firmware popolari e svilupparne di propri
    \item Continuare a sviluppare software bare-metal (specialmente benchmark), confrontando le prestazioni con altri chip/design
    \item Creare driver di base e leggermente complessi (GPIO, comunicazione seriale con altri MCU come ESP32C6, LCD di base)
    \item Ottimizzare i flag del compilatore (opzionale)
    \item Migliorare il flusso di lavoro di debug
\end{itemize}

\subsection{PR e Promozione}
\begin{itemize}
    \item Accelerare le attività di reclutamento aprendo stand nel campus principale del PoliTO, mostrare demo software dal vivo in esecuzione su MCU RV32
    \item Entrare in contatto con aziende RISC-V, candidarsi per testare in beta i loro prodotti, ottenere il loro aiuto per la visibilità e i loro consigli per il team
    \item Entrare in contatto con RISC-V International, candidarsi per i loro programmi
    \item Organizzare workshop e conferenze su RISC-V. Invitare persone influenti di aziende/organizzazioni nel campus.
\end{itemize}

\section{Fase 3: Funzionalità Avanzate (Febbraio 2026 - Maggio 2026)}
Espandere le funzionalità.

\subsection{Hardware}
\begin{itemize}
    \item Sviluppare ulteriormente l'interfaccia periferica (Collegare sensori e moduli come DAC, connettersi a WiFi/Bluetooth con MCU esterni come ESP32C6)
    \item Migliorare il controller degli interrupt
    \item Confrontare il design attuale con altri MCU RV32 come ESP32C6, ESP32P4 e Pi Pico 2
\end{itemize}

\subsection{Software}
\begin{itemize}
    \item Sviluppare un SDK personalizzato
    \item Contribuire alla compatibilità GCC/LLVM per RV32
    \item Continuare a sviluppare applicazioni di benchmark e demo che spingano i limiti della CPU, confrontandola con altri MCU RV32
\end{itemize}

\subsection{PR e Promozione}
\begin{itemize}
    \item Ricercare aziende nel mercato RV32, invitare i loro CEO a tenere presentazioni a scuola
    \item Continuare a contattare aziende di PCB, FPGA e software RISC-V per utilizzare i loro prodotti/servizi
    \item Ricercare e candidarsi per eventi a cui possiamo partecipare dove possiamo mostrare i nostri progetti (RISC-V Summit Demo Day, Embedded World, Maker Faire)
    \item Organizzare workshop con persone dei dipartimenti HW e SW
    \item Realizzare poster, magliette e altro materiale promozionale
    \item Continuare le attività di reclutamento, mettere i nostri progetti (FPGA con i nostri design ecc.) sul tavolo, facendo demo dal vivo e test di benchmark
\end{itemize}

\section{Fase 4: Stadio Finale (Maggio 2026 - Ottobre 2026)}
Prepararsi per i passi successivi.

\subsection{Hardware}
\begin{itemize}
    \item Finalizzare il design RTL del SoC RV32
    \item Ultimi ritocchi al PCB
    \item Inviarlo ad altri team studenteschi spiegando le funzionalità in modo che possano testarlo in beta nei loro progetti (circuiti musicali PoliTek, cervello dei robot RoboTO ecc.)
    \item Ricercare l'architettura, i core e le estensioni RV64
\end{itemize}

\subsection{Software}
\begin{itemize}
    \item Completare la documentazione
    \item Garantire build riproducibili
    \item Ricercare l'ecosistema RV64
\end{itemize}

\subsection{PR e Coordinamento Team}
\begin{itemize}
    \item Ricercare e candidarsi per altri eventi
    \item Mantenere i contatti con le aziende nel mercato RV32
    \item Pianificare la roadmap e i progetti del secondo anno discutendo con tutti i membri attivi, molto probabilmente orientandosi verso RV64 e Linux per l'ecosistema RISC-V
    \item Pianificare le attività di reclutamento e assegnazione dei ruoli per il prossimo progetto
\end{itemize}

\section{Rischi}
\begin{itemize}
    \item Le roadmap di Maggio - Ottobre potrebbero subire slittamenti a causa delle sessioni d'esame
    \item Gli obiettivi contrassegnati come opzionali possono slittare ad altre fasi o non essere completati del tutto
    \item L'intera roadmap potrebbe subire ulteriori slittamenti se le attività di reclutamento non andassero a buon fine e/o i membri non fossero attivi
\end{itemize}

\end{document}

