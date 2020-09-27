# Download

wget https://github.com/prometheus/prometheus/releases/download/v2.18.1/prometheus-2.18.1.linux-amd64.tar.gz

tar xvfz prometheus-2.18.1.linux-amd64.tar.gz

cd prometheus-2.18.1.linux-amd64



# Configure Prometheus
prometheus.yml

global:  
   scrape_interval: 5s  
   evaluation_interval: 5s
scrape_configs:  
   - job_name: 'prometheus'    
     static_configs:    
     - targets: ['localhost:9090']
     
Start

./prometheus
