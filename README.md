

}




\section{Introduction}
\subsection{Context}
In this paper, I will design and specify the Requirement, UI and Hardware of the device I am making virtually/Imaginary it doesn't exist it is just for prototyping and showcase of my knowledge in Interactive System Design.
I am designing a medical device that is used for detecting heart attack before it happens with the help of a patch sensor that detects Cardiac Bookmakers, heartbeat, Oxygen Level and change of electric impulse in the heart
\subsection{Problem}
Since the user is free to travel and used modern-day technologies it can be difficult to call the emergency hot-line just using normal connectivity of modern-day life such as Bluetooth and WiFi as Bluetooth can be used by headphones or speakers etc.. and WiFi can be unavailable due to any reason. For the patch, it is made of Polyaniline Coated Filter Paper and it is based on Impedance Spectroscopy-Based Detection 
\subsection{Motivation}
I would like to thanks all my colleagues for giving feedback which helped me increase the level of writing,diagram and understanding



\subsection{Image of Medical Device and Use Case}

In the Fig. 1. there is a sensor substrate that will be attach to user body and it will be attached to wearable device from which the data transmission to the cloud and if required call to emergency service will take place. 

\section{Designing and Concept}
\subsection{Requirements}

\subsubsection{Design}
\begin{itemize}
\item It should be under specific weight as it is needed to be carried by user.
\item It should be design right as it will be carried by user
\item It should also satisfy all the system requirements
\end{itemize}
\subsubsection{System}
\begin{itemize}
\item It should be able to communicate with other devices/Networks
\item It should be able to send SOS Alert when needed
\item It should be refined from the Government policies on medical device
\item It should have a User Interface which is easy to use
\end{itemize}

\subsection{Hardware}
\subsubsection{Connectivity}

\begin{itemize}
    \item GSM - OPTIGA™ Connect Consumer OC1120 - eSIM solution
    \item Wifi Bluetooth - WL1835MOD
\end{itemize}
\subsubsection{Others}
\begin{itemize}
    \item Medical Sensor (Sensor for detecting change in heart rate, cardiac biomarkers)
    \subitem The Sensor designed by D.Mondal and his team  in [1] is being used in this project.
    \item 66AK2G12 Processor Texas Instruments 
    \subitem The use of this processor because it is designed for networking and also for security which satisfy the need of product being both secure and safe.
    Processor is integrated with high-speed peripheral and memory interfaces, hardware acceleration for network and cryptography functions.
    \item 1 GB memory 
    \item Buzzer
    \subitem It is needed for vibrating the device to let the user know to check their status or in case of failure of system.
    \item  LED  (Green, Orange , Red , Yellow  )
    \subitem It is used as indicator to let user know their health status it is also used for indicating system failure, low battery.
    \item Speaker 
    \subitem It is used to let user know their status or device status through auditory perception
    \item Button
    \subitem It is needed to turn on or off the device and also to activate the speaker for that instance.
\end{itemize}

\subsection{Redundancy}
For Redundancy the system will always check the condition of software,will also store data from the sensor two time and in case of failure it will try to self boot in safe mode and alert the user.
For Sensor Two sensor are used with each subdivided in two part giving us the total 2\textsuperscript{n} values.
For better accuracy we use Advanced Evidence Theory or Demspter Shafer Theory for combining the data from sensor
To know when the Sensor is not working we use Divergence Measure to Measure the conflict in data from the sensor
We Store this Conflict and calculate error rate over time and once the time period is over we notify the user that need of servicing of sensor is needed


\subsection{Models}
\newpage
\begin{strip}
  \centering
  \includegraphics[scale=0.54]{Requiremts.png}
  \caption{Requirements}
\end{strip}

\begin{strip}
  \centering
  \includegraphics[scale=0.6]{Use.png}
  \caption{UseCase}
\end{strip}
\begin{strip}
  \centering
  \includegraphics[scale=0.7]{ACT.png}
  \caption{Activity}
\end{strip}

\begin{strip}
  \centering
  \includegraphics[scale=0.54]{SM.png}
  \caption{StateMachine}
\end{strip}

% \begin{strip}
%   \centering
%   \includegraphics[scale=0.55]{Use.png}
% \end{strip}
\newpage
\subsection{User Interface}
\begin{strip}
    \centering
    \includegraphics[scale = 1.8]{Untitled00.png}
    \label{fig:my_label}
\end{strip}

\newpage
\begin{strip}
    \centering
    \includegraphics[scale = 0.75]{Device.pdf}
    \label{fig:my_label}
\end{strip}
% \begin{strip}[b]
%     \centering
%     \includepdf[pages=2]{UI_1.pdf}
%     \label{fig:my_label}
% \end{strip}

% \begin{center}
%   \makebox[\textwidth]{\includegraphics[width=\textwidth,height=\textheight,keepaspectratio]{Requiremts.png}}
% \end{center}
% \begin{center}
%   \makebox[\textwidth]{\includegraphics[scale=0.2]{Use.png}}
% \end{center}
%\begin{center}[t]
%  \noindent\makebox[\textwidth]{\includegraphics[width=\paperwidth]{Use.png}}
%\end{center}
% \begin{figure}[htbp]
%     \centering
%     \includegraphics[width=1.0\textwidth,height=0.5\textwidth, scale = 0.5]{Use.png}
%     \caption{Caption}
%     \label{fig:my_label}
% \end{figure}
%\begin{center}
%  \noindent\makebox[\textwidth]{\includegraphics[width=\paperwidth]{SM.png}}
%\end{center}

%\begin{center}
%  \noindent\makebox[\textwidth]{\includegraphics[width=\paperwidth]{ACT.png}}
%\end{center}

% \begin{figure}[htbp]
%     \centering
%     \includegraphics[width=1.0\textwidth,height=0.5\textwidth, scale = 0.5]{SM.png}
%     \caption{Caption}
%   \label{fig:my_label}
% \end{figure}

% \begin{figure}[htbp]
%     \centering
%   \includegraphics[width=1.0\textwidth,height=0.5\textwidth, scale = 0.5]{ACT.png}
%     \caption{Caption}
%     \label{fig:my_label}
% \end{figure}
% \begin{figure}
%     \centering
%     \includegraphics{UI.pdf}
%     \caption{Caption}
%     \label{fig:my_label}
% \end{figure}
% \begin{figure}
%     \centering
%     \includegraphics[page =2,scale=0.2]{UI.pdf}
%     \caption{Caption}
%     \label{fig:my_label}
% \end{figure}
%\includegraphics[scale=0.75]{UI.pdf}
%\includegraphics[scale=0.75,page =2]{UI.pdf}]
\section{Discussion}
\subsection{Concept}
My concept was to convert the prototype into state of the art device easy to use by people of all ages and also for people with disability. My task was also to get rid of connection to power and audio on the Mobile phone as displayed in fig 1. It was also to make a emergency request with Location of user in case of emergency without relaying on WiFi and Bluetooth which may be unavailable to us due to any circumstances.

\subsection{Initial Problem}
Not only does it solve the initial problem of having peripheral device connected to your cell phone via wire it also efficiently increase the readiness for user to get medical feedback via doctor or emergency service making user more safe.

\subsection{Improvement}
During lecture via the feedback of my colleague i was able to identify a clause in my requirement which i later on not only corrected but also improved it.
For Hardware i was using quite a high amount of memory given today memory is comparatively cheap but i reduce the amount of memory needed saving us from money in development.

\section{Conclusion and Future Direction}
\subsection{Overview}
\begin{itemize}
    \item In this project i have designed a device which can be used by people easily as it is also made for people with disability and people who doesn't like or cant to use mobile phone.
    \item It is also made possible for doctor to read your daily Heart rate,oxygen and Cardiac Bio-maker value so that if needed he can consult the user.
    \item It is also made possible to contact the emergency service with the location of user with the error of up to 30 cm without the use WiFi and Bluetooth to make it more reliable, available to user.
    \item With keeping the regulation of government on medical device in the requirement it is also safe for user
    \item With current up to art technologies in the field of I.O.T and connection it is to be said that the device is also secure for user
\end{itemize}

\subsection{Future Direction}
\begin{itemize}
    \item I believe for future we can also add communication via satellite to make the device more reliable for its emergency service as connection using satellite consume more power one need to work on it. 
    \item There can also be addition of new sensor to same device for multi functionality keeping it small and easy to carry.
\end{itemize}
% In this project i have designed a device which can be used by people easily as it is also made for people with disability and people who doesn't like or cant to use mobile phone.
% It is also made possible for doctor to read your daily Heart rate,oxygen and Cardiac Bio-maker value so that if needed he can consult the user.
% It is also made possible to contact the emergency service with the location of user with the error of up to 30 cm without the use WiFi and Bluetooth to make it more reliable, available to user.
% With keeping the regulation of government on medical device in the requirement it is also safe for use
% With current up to art technologies in the field of I.O.T and connection it is to be said that the device is also secure for user
\begin{thebibliography}{00}
\bibitem{b1} D. Mondal, D. Paul and S. Mukherji, "Impedance Spectroscopy-Based Detection of Cardiac Biomarkers on Polyaniline Coated Filter Paper," in IEEE Sensors Journal, vol. 17, no. 16, pp. 5021-5029, 15 Aug.15, 2017, doi: 10.1109/JSEN.2017.2717701.
\bibitem{b2}  "Now, Your Smartphone Can Help You Detect A Heart Attack" IIT Bombay. 2018
[Online] Available
https://www.iitb.ac.in/en/research-highlight/now-your-smartphone-can-help-you-detect-heart-attack




    
