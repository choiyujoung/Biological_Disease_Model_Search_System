# 🔎 Biological Disease Model Search System
📌 Project Overview
이 프로젝트는 엑셀에 정리된 질환 모델 데이터베이스에서 원하는 정보를 빠르게 검색하기 위해 만든 파이썬 프로그램입니다. 질병명이나 주요 타겟 유전자를 입력하면 그에 맞는 동물 실험 모델과 핵심 기전을 즉시 출력합니다.


<img width="1788" height="385" alt="image" src="https://github.com/user-attachments/assets/12ca4b08-6e64-4a1e-ba4d-97047b7a3113" />

🛠 Tech Stack
Language: Python

Library: Pandas

📂 주요 기능
데이터 로드 및 표준화: pd.read_excel을 이용해 데이터를 읽어오고, 분석하기 쉽게 컬럼 이름을 재정의했습니다.

조건부 검색 로직: Disease와 Key Target 컬럼에서 대소문자 구분 없이(case=False) 키워드를 포함하는 모든 행을 찾습니다.

결과 리포팅: 검색된 데이터 중 최적의 매칭 결과를 요약하여 리포트 형식으로 보여줍니다.

💻 실행 예시
Python
 'Glioblastoma' 질환을 검색할 경우
'''python print(biological_rag_system("Glioblastoma"))'''

 [출력 결과]
 - 추천 모델: Orthotopic brain tumor model
 - 핵심 기전: cp8 -> FLG upregulation -> MGMT suppression
 - 주요 타겟: FLG(Filaggrin), MGMT, HDAC6
 - 근거 논문: Dual suppression of stemness and redox adaptation...
🎯 프로젝트 성과
데이터 탐색 효율화: 수작업으로 엑셀을 필터링하는 번거로움을 자동화했습니다.

정밀한 검색: 문자열 처리 함수(.str.strip(), .contains())를 활용해 데이터의 노이즈를 제거하고 검색 정확도를 높였습니다.




# 🔎 Biological Disease Model Search System
📌 Project Overview
This project is a Python-based search tool designed to efficiently retrieve information from a biological disease model database. By inputting a disease name or a key biological target, the system instantly provides relevant animal models, core mechanisms, and supporting literature.

🛠 Tech Stack
Language: Python

Library: Pandas

📂 Key Features
Data Loading & Standardization: Uses pd.read_excel to load datasets and redefines column names for better data structure and accessibility.

Conditional Search Logic: Implements a search function that scans both Disease and Key Target columns. It handles data noise using .str.strip() and ensures case-insensitive matching with case=False.

Automated Reporting: Summarizes complex row data into a clean, readable report format including Recommended Model, Mechanism, Primary Target, and Evidence.

💻 Usage Example
Python
 Searching for 'Glioblastoma'
print(biological_rag_system("Glioblastoma"))

 [Output]
 - Recommended Model: Orthotopic brain tumor model
 - Key Mechanism: cp8 -> FLG upregulation -> MGMT suppression
 - Primary Target: FLG(Filaggrin), MGMT, HDAC6
 - Evidence: Dual suppression of stemness and redox adaptation...
🎯 Project Impact
Efficiency: Automated the tedious process of manually filtering Excel sheets for specific research data.

Accuracy: Improved search precision by utilizing string manipulation functions to handle inconsistent data entries.




