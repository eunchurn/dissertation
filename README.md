# 단국대학교 건축공학과 석·박사학위 논문 TeX 템플릿
## Overview
 - LaTeX2ε 사용방법을 숙지하시고 시작하시는 것이 좋습니다. [처음시작하기](http://wiki.ktug.org/wiki/wiki.php/%EC%B2%98%EC%9D%8C%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0)
 - 주의 : 급하게 쓴거라 중복된 패키지나 오류가 있을 수 있습니다. 시간될 때 정리하도록 하겠습니다.
## Build 환경
 - TeXLive 2016 이후 버전으로 빌드. 
 - pdfLaTeX로 빌드 하였음.
 - 본 논문은 한글 폰트를 은글꼴을 사용하였음 `\usepackage{dhucs-untype1}` 그러나 TeXLive 최신버전에서는 나눔폰트가 기본으로 되어있음. 따라서 [KTUG사설저장소]{http://ftp.ktug.org/KTUG/texlive/tlnet/}가 추가되어있다면, `unfonts-base-type1`, `unfonts-other-type1`이 설치해야함.
 `<sudo> tlmgr install unfonts-base-type1 unfonts-other-type1`
 - 저장소 등록은 [KTUG 사설저장소 추가](http://wiki.ktug.org/wiki/wiki.php/KtugPrivateRepository?action=show&redirect=KTUG%20%EC%82%AC%EC%84%A4%EC%A0%80%EC%9E%A5%EC%86%8C) 참조.
## 수정해야 할 파일
 - 인준지는 `auth.tex`파일이며 박사학위논문을 기준으로 작성하였으므로 적당히 수정이 필요. (본 저장소의 템플릿은 주석처리되어있고 인준지 이미지 파일로 대체되어있음)
 - 논문 메인 파일 `dissertation.tex`이고 chapter 별로 파일로 분리되어 있음. `chap1.tex`, `chap2.tex`...
 - 필요하면 `\begin{part} \end{part}` 구문을 추가할 수 있음.
 - 참고문헌 `reference.bib`에 작성 [구글스칼라](https://scholar.google.co.kr/)에서 문헌 검색후 `bibTeX`를 선택후 복사해서 나열. `natbib`패키지를 사용. `\cite`, `\citep`, `\citet`을 적절히 활용. 사용법 : http://merkel.texture.rocks/Latex/natbib.php (프랑스 말로 되어 있으나, 이해할 수 있음)
 ## Build 방법
 - `pdflatex dissertation.tex` -> `bibtex dissertation` -> `pdflatex dissertation.tex` -> `pdflatex dissertation.tex` (최초 빌드 -> 참고문헌 빌드 -> 목차 및 그림 표 번호 인덱싱 -> 본문 표시)
 - TeXlive를 사용하면 TeXeditor에서 pdfLaTeX 빌드 한번 BibTex 빌드 후 pdfLaTeX 빌드 두번하면 된다.
 ## 주의 사항 
 - 저장소에 있는 본문은 저작권이 있으므로 참고용으로만 사용하시길 바랍니다.
 - 이 템플릿 파일을 사용해서 발생하는 모든 문제에 대해서 템플릿 작성자들은 어떠한 책임도 지지 않습니다.

