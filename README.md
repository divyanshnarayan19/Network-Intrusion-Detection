### Network-Intrusion-Detection

With the enormous growth of computer networks usage and the huge increase in the number of applications running on top of it, network security is becoming increasingly more important. All the computer systems suffer from security vulnerabilities which are both technically difficult and economically costly to be solved by the manufacturers. Therefore, the role of Intrusion Detection Systems (IDSs), as special-purpose devices to detect anomalies and attacks in the network, is becoming more important.

The research in the intrusion detection field has been mostly focused on anomaly-based and misusebased detection techniques for a long time. While misuse-based detection is generally favored in commercial products due to its predictability and high accuracy, in academic research anomaly detection is typically conceived as a more powerful method due to its theoretical potential for addressing novel attacks.

Conducting a thorough analysis of the recent research trend in anomaly detection, one will encounter several machine learning methods reported to have a very high detection rate of 98% while keeping the false alarm rate at 1%. However, when we look at the state of the art IDS solutions and commercial tools, there is no evidence of using anomaly detection approaches, and practitioners still think that it is an immature technology. To find the reason of this contrast, lots of research was done done in anomaly detection and considered various aspects such as learning and detection approaches, training data sets, testing data sets, and evaluation methods.

Your task to build network intrusion detection system to detect anamolies and attacks in the network. There are two problems. 

1. Binomial Classification: Activity is normal or attack 

2. Multinomial classification: Activity is normal or DOS or PROBE or R2L or U2R 

Please note that, currently the dependent variable (target variable) is not definied explicitly. However, you can use attack variable to define the target variable as required.

LIST OF COLUMNS FOR THE DATA SET:

["duration","protocol_type","service","flag","src_bytes","dst_bytes","land", "wrong_fragment","urgent","hot","num_failed_logins","logged_in", "num_compromised","root_shell","su_attempted","num_root","num_file_creations", "num_shells","num_access_files","num_outbound_cmds","is_host_login", "is_guest_login","count","srv_count","serror_rate", "srv_serror_rate", "rerror_rate","srv_rerror_rate","same_srv_rate", "diff_srv_rate","srv_diff_host_rate","dst_host_count","dst_host_srv_count","dst_host_same_srv_rate", "dst_host_diff_srv_rate","dst_host_same_src_port_rate", "dst_host_srv_diff_host_rate","dst_host_serror_rate","dst_host_srv_serror_rate", "dst_host_rerror_rate","dst_host_srv_rerror_rate","attack", "last_flag"]


BASIC FEATURES OF EACH NETWORK CONNECTION VECTOR 

- Duration: Length of time duration of the connection 
- Protocol_type: Protocol used in the connection 
- Service: Destination network service used 
- Flag: Status of the connection – Normal or Error 
- Src_bytes: Number of data bytes transferred from source to destination in single connection 
- Dst_bytes: Number of data bytes transferred from destination to source in single connection 
- Land: if source and destination IP addresses and port numbers are equal then, this variable takes value 1 else 0 
- Wrong_fragment: Total number of wrong fragments in this connection 
- Urgent: Number of urgent packets in this connection. Urgent packets are packets with the urgent bit activated

- Hot: Number of „hot‟ indicators in the content such as: entering a system directory, creating programs and executing programs 
- Num_failed _logins: Count of failed login attempts 
- Logged_in Login Status: 1 if successfully logged in; 0 otherwise 
- Num_compromised: Number of ``compromised' ' conditions 
- Root_shell: 1 if root shell is obtained; 0 otherwise 
- Su_attempted: 1 if ``su root'' command attempted or used; 0 otherwise 
- Num_root: Number of ``root'' accesses or number of operations performed as a root in the connection 
- Num_file_creations: Number of file creation operations in the connection 
- Num_shells: Number of shell prompts 
- Num_access_files: Number of operations on access control files 
- Num_outbound_cmds: Number of outbound commands in an ftp session 
- Is_hot_login: 1 if the login belongs to the ``hot'' list i.e., root or admin; else 0 
- Is_guest_login: 1 if the login is a ``guest'' login; 0 otherwise
