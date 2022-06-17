

kube-prometheus-stack-36.0.2 
This stack contains Critical CVE which are related to Busybox and Go

BusyBox through 1.35.0 allows remote attackers to execute arbitrary code if netstat is used to print a DNS PTR record\'s value to a VT compatible terminal. Alternatively, the attacker could choose to change the terminal\'s colors.
https://nvd.nist.gov/vuln/detail/CVE-2022-28391


An attacker-controlled pointer free in Busybox\'s hush applet leads to denial of service and possible code execution when processing a crafted shell command, due to the shell mishandling the &&& string. This may be used for remote code execution under rare conditions of filtered command input.
https://nvd.nist.gov/vuln/detail/CVE-2022-23806

Following versions which are scanned 
quay.io/prometheus/prometheus:v2.36.1
quay.io/prometheus-operator/prometheus-operator:v0.57.0
quay.io/prometheus/alertmanager:v0.24.0
registry.k8s.io/kube-state-metrics/kube-state-metrics:v2.5.0
