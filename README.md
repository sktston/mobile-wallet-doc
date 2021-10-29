# Mobile Wallet (모바일지갑) 파트너 포탈 사용 가이드

URL : https://sktston.github.io/mobile-wallet-doc/

- Mobile Wallet 가이드 문서는 Sphinx 기반으로 작성되었습니다.
- Sphinx는 개발문서를 만들 때 사용하기 적합한 툴 입니다. Sphinx는 파이썬에서 제공하기 때문에 파이썬 설치가 되 있어야 합니다.

​
## Sphinx 설치 및 사용

아래 pip를 사용하여 shpinx를 설치한다

`$ pip instal Sphinx`

주요 파일 설명

    - Makefile, make.bat: 이 둘은 각각 유닉스 / 윈도우 계열에서 빌드할 때 사용하는 파일입니다.
    - build/ : 빌드 후 결과물이 저장되는 경로.
    - source/_static/:    이미지 같은 리소스 파일을 넣을 수 있습니다. (conf.py를 통해 경로변경 가능)
    - source/_templates/: 템플릿 같은 파일을 넣을 수 있습니다       (conf.py를 통해 경로변경 가능)
    - source/conf.py/:    설정파일 (앞에서 설정한 프로젝트 이름, 작성자, 버전 등 변경가능)
    - source/index.rst:   문서의 첫 번째 페이지가 된다. 해당 파일로 목차가 생성됨

### Build : HTML 생성

다음 명령어를 통해 source에 있는 파일을 html 결과파일로 바꿔줄 수 있습니다.

`$ make html`

아래와 같은 결과를 얻을 수 있습니다.

```
 % make html
Sphinx 버전 4.2.0 실행 중
번역을 불러오는 중 [ko]… 완료
pickle로 저장된 환경을 불러오는 중... 완료
myst v0.15.2: MdParserConfig(renderer='sphinx', commonmark_only=False, enable_extensions=['dollarmath'], dmath_allow_labels=True, dmath_allow_space=True, dmath_allow_digits=True, dmath_double_inline=False, update_mathjax=True, mathjax_classes='tex2jax_process|mathjax_process|math|output_area', disable_syntax=[], url_schemes=['http', 'https', 'mailto', 'ftp'], heading_anchors=None, heading_slug_func=None, html_meta=[], footnote_transition=True, substitutions=[], sub_delimiters=['{', '}'], words_per_minute=200)
빌드 중 [mo]: 오래된 0 개의 po 파일 대상
빌드 중 [html]: 오래된 2 개의 원본 파일 대상
환경을 갱신하는 중: [설정이 변경됨 ('project')] 2 개 추가됨, 0 개 변경됨, 0 개 제거됨
원본을 읽는 중… [ 50%] index                                                                                                                                                                                                                  원본을 읽는 중… [100%] portal/login
오래된 파일을 찾는 중… 찾은 것이 없음
pickle로 환경을 저장하는 중... 완료
일관성 확인 중... 완료
문서 준비 중... 완료
출력을 쓰는 중… [ 50%] index                                                                                                                                                                                                                  출력을 쓰는 중… [100%] portal/login
색인 생성 중... genindex 완료
추가 페이지 작성 중... search 완료
정적 파일을 복사하는 중... 완료
추가 파일을 복사하는 중... 완료
English (code: en)에서 검색 인덱스 덤프 중... 완료
객체 인벤토리 덤프 중... 완료
빌드 성공.

HTML 페이지는 ../build/html에 있습니다.
```


### Deploy : 배포 및 Web Server update


생성된 모든 file을 master branch에 push 하면 자동 업데이트 

## Document 주요 내용

1. 모바일지갑 파트너 관리자를 위한 매뉴얼
