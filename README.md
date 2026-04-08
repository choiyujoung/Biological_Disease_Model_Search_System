# 🔎 Biological Disease Model Search System
📌 Project Overview
이 프로젝트는 엑셀에 정리된 질환 모델 데이터베이스에서 원하는 정보를 빠르게 검색하기 위해 만든 파이썬 프로그램입니다. 질병명이나 주요 타겟 유전자를 입력하면 그에 맞는 동물 실험 모델과 핵심 기전을 즉시 출력합니다.

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
print(biological_rag_system("Glioblastoma"))

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



	Title	Abstract	Disease	Model	Species	Key Target	Keywords
1	"Dual suppression of stemness and redox adaptation in glioblastoma through filaggrin upregulation by an abiraterone-based HDAC inhibitor
(PMID: 41943081)"	"Mechanism:
1. cp8 -> FLG upregulation -> MGMT suppression
2. HDAC6 inhibition"	TMZ-resistant Glioblastoma	Orthotopic brain tumor model (Intracranial implantation)	Mouse (C57BL/6J, NOD/SCID), Rat (Sprague-Dawley)	FLG(Filaggrin), MGMT, HDAC6	glioblastoma, TMZ resistance, HDAC inhibitor, FLG, MGMT, redox adaptation
2	"Aquaporin 9 regulates acetaldehyde uptake, alcohol-induced liver injury, and drinking behavior
(PMID: 41941046)"	"Hepatic AQP9 expression is downregulated in ALD patients
AQP9 knockout improved early-stage ALD by reducing hepatic lipogenesis, lipid peroxidation, and inflammation"	Alcohol-associated liver disease	Aqp9 global knockout (KO), Aldh2*2 knock-in (KI), Aqp9 KO x Aldh2*2 KI (KOKI)	"Mouse (C57BL/6J)
"	AQP9, AQP8, ALDH2, Acetaldehyde (AcH)	cetaldehyde; alcohol‐associated liver disease (ALD); aquaporin 9 (AQP9); drinking behavior; ethanol metabolism.
3	"Long non-coding RNA profiling of hypertrophic cardiomyopathy in mice 
(PMID: 41942516)"	Transcriptome-wide analysis identified differentially expressed lncRNAs in HCM across human and mouse models, providing candidate regulators of pathological hypertrophy.	Hypertrophic cardiomyopathy	TNNT2 ∆160 mutation mouse model (HCM model)	Mouse (C57BL/6J)	IncRNAs (differentially expressed in HCM)	IncRNAs, Hypertrophic cardiomyopathy (HCM), transcription
4	"A refined chronic MPTP/probenecid model of Parkinson's disease in mature adult mice 
(PMID: 41941954)"	"A refined chronic low-dose MPTP/probenecid (MPTP/p) regimen was developed to model progressive Parkinson's disease (PD) in mice.
MPTP/p recapitulate the gradual emergence of motor, cognivitve. and neuropathological hallmarks of PD, while maintaining animal survival rate"	Parkinson's disease	chronic low-dose MPTP/probenecid model	Mouse (C57BL/6J)	Dopaminergic neurous, Tyrosine hydroxylase, α-synuclein (phosphorylated)	Chronic regimen; MPTP; Mouse model; Parkinson's disease.
5	"Zanthoxylum bungeanum essential oil alleviates DSS-induced ulcerative colitis in mice by modulating gut microbiota-dependent AhR/Nrf2 signaling 
(PMID: 41942225)"	Zanthoxylum bungeanum essential oil (ZBO) attenuates DSS-induced ulcerative colitis by suppressing pro-inflammatory mediators and enhancing intestinal barrier function. Its therapeutic effect is mediated through modulation of gut microbiota and activation of the AhR/Nrf2 signaling pathway	Ulcerative colitis	DSS-induced ulcerative colitis model	Mouse (C57BL/6J)	lL-6, IL-1ß, TNF-α, CCL20, AhR/Nrf2 signaling pathway, Gut microbiota	AhR/Nrf2 signaling pathway; Gut microbiota; Intestinal barrier; Ulcerative colitis; Zanthoxylum bungeanum.<img width="1788" height="385" alt="image" src="https://github.com/user-attachments/assets/12ca4b08-6e64-4a1e-ba4d-97047b7a3113" />

