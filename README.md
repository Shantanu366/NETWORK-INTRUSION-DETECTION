# Network-Intrusion-Detection
# BUSINESS PROBLEM:
Your task to build network intrusion detection system to detect anamolies and attacks in the
network. There are two problems.
1. Binomial Classification: Activity is normal or attack
2. Multinomial classification: Activity is normal or DOS or PROBE or R2L or U2R
Please note that, currently the dependent variable (target variable) is not definied explicitly.
However, you can use attack variable to define the target variable as required.
# DATA AVAILABILITY:
This data is KDDCUP’99 data set, which is widely used as one of the few publicly available data sets
for network-based anomaly detection systems.
For more about data
# LIST OF COLUMNS FOR THE DATA SET:
["duration","protocol_type","service","flag","src_bytes","dst_bytes","land",
"wrong_fragment","urgent","hot","num_failed_logins","logged_in",
"num_compromised","root_shell","su_attempted","num_root","num_file_creations",
"num_shells","num_access_files","num_outbound_cmds","is_host_login",
"is_guest_login","count","srv_count","serror_rate", "srv_serror_rate",
"rerror_rate","srv_rerror_rate","same_srv_rate", "diff_srv_rate", 
"srv_diff_host_rate","dst_host_count","dst_host_srv_count","dst_host_same_srv_rate",
"dst_host_diff_srv_rate","dst_host_same_src_port_rate",
"dst_host_srv_diff_host_rate","dst_host_serror_rate","dst_host_srv_serror_rate",
"dst_host_rerror_rate","dst_host_srv_rerror_rate","attack", "last_flag"]
# ATTACK CLASS:
1. DOS: Denial of service is an attack category, which depletes the victim‟s resources thereby making it
unable to handle legitimate requests –e.g. syn flooding. Relevant features: “source bytes” and “percentage
of packets with errors”
2. Probing: Surveillance and other probing attack‟s objective is to gain information about the remote victim
e.g. port scanning. Relevant features: “duration of connection” and “source bytes”
3. U2R: unauthorized access to local super user (root) privileges is an attack type, by which an attacker uses
a normal account to login into a victim system and tries to gain root/administrator privileges by exploiting
some vulnerability in the victim e.g. buffer overflow attacks. Relevant features: “number of file creations”
and “number of shell prompts invoked,”
4. R2L: unauthorized access from a remote machine, the attacker intrudes into a remote machine and gains
local access of the victim machine. E.g. password guessing Relevant features: Network level features –
“duration of connection” and “service requested” and host level features - “number of failed login
attempts”
