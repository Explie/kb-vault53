
Analysing Remote Desktop Protocol (RDP) usage for Windows Hosts
=================================================================

EventLogs
++++++++++

.. tip::
    Windows EventLogs are located at ``C:\Windows\System32\winevt\Logs``.
    Which EventLogs are available heavily depends on the installed Windows 
    services and features and which 3rd party applications 
    are also using the Windows EventLog API.


Incoming connections
---------------------

**Security.evtx:**

``EventID 4624`` with ``LogonType 10``
    * SourceIP for the connections
    * UserName used for Logon

``Event ID 4778/4779``


**Microsoft-Windows-TerminalServices-RDPClient Operational.evtx:**

Microsoft-Windows-TerminalServices-RemoteConnectionManager%4Operational.evtx
261 
Listener RDP-Tcp hat eine Verbindung empfangen.

1149
Remotedesktopdienste: Die Benutzerauthentifizierung war erfolgreich:

Benutzer: Administrator
Domäne: EXPOTECHNIK
Quellnetzwerkadresse: 10.101.10.1.

Registry
----------

File System artefacts
---------------------
