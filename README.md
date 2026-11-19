# pm25-explorer-0679
# PM2.5 Explorer

ระบบสำรวจคุณภาพอากาศ PM2.5 ของประเทศไทย (รายวิชา 1145100 Data Science Toolbox)

## วิธีติดตั้ง
uv iniy
git config --global user.name "ชื่อ นามสกุล"
git config --global user.email "อีเมลที่ใช้สมัคร GitHub"
git config --global init.defaultBranch main

$base = "https://raw.githubusercontent.com/popotaroman-cloud/data-science-toolbox/main"
Invoke-WebRequest "$base/environment.yml" -OutFile environment.yml    # ถ้าใช้ conda
Invoke-WebRequest "$base/pyproject.toml"  -OutFile pyproject.toml     # ถ้าใช้ uv

uv sync

python -c "import pandas, duckdb, plotly, streamlit; print('พร้อมใช้งาน')"

cd ~/projects                
git clone https://github.com/<username>/pm25-explorer.git
cd pm25-explorer
code .                   

## ผู้จัดทำ
แอนโทนี่ ดูบัชนี 67114540679 