# GWAS

유전체 분석을 위한 SNP 검색 도구입니다.

## 개요

VCF 파일에서 특정 SNP 위치를 검색하고 관련 정보를 추출하는 도구입니다.

## 주요 기능

- VCF 파일 파싱
- SNP 위치 기반 검색
- 유전자 정보 추출
- 참조/대체 염기 정보 제공

## 사용 방법

```bash
python SearchingBySNP.py
```

## 요구사항

- Python 3.12
- pysam
- vcfpy

## 설치

### uv 설치

#### Windows
```powershell
# PowerShell에서 실행
irm https://astral.sh/uv/install.ps1 | iex
```

#### macOS / Linux
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

설치 후 터미널을 재시작하거나 다음 명령어로 PATH에 추가:
```bash
export PATH="$HOME/.cargo/bin:$PATH"
```

### 가상환경 설정

```bash
# Python 3.12 가상환경 생성
uv venv --python 3.12

# 가상환경 활성화
# Windows (PowerShell)
.venv\Scripts\Activate.ps1

# macOS / Linux
source .venv/bin/activate
```

### 패키지 설치

```bash
# uv를 사용한 패키지 설치
uv pip install -r requirements.txt
```

## 파일 구조

- `SearchingBySNP.py`: SNP 검색 메인 스크립트

## 데이터 형식

### VCF 파일 형식
표준 VCF 형식의 파일이 필요합니다.

### SNP 위치 리스트
코드 내에 검색할 SNP 위치가 하드코딩되어 있습니다. 필요에 따라 수정하세요.

## 참고

- 이 스크립트는 예제 코드이며, 실제 사용 시 VCF 파일 경로와 SNP 위치를 수정해야 합니다.
- pysam과 vcfpy는 유전체 데이터 분석에 널리 사용되는 라이브러리입니다.

---

해당 프로젝트는 Examples-Python의 Private Repository에서 공개 가능한 수준의 소스를 Public Repository로 변환한 것입니다.

