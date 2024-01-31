## 📄 각종 환경 세팅 Script 저장소 📄

## 📂 Window

- **TimeConditionBatch.bat** : 특정 시간대에만 특정 프로그램들을 실행하고 헬스체크를 수행하는 배치파일

---

## 📂 Linux

- **GPU-Driver.sh** : Nvidia Driver, Cuda Tool Kit, OpenGL 세팅 스크립트
- **Remove-Nouveau.sh** : Nvidia Driver와 충돌나는 Nouveau 커널 드라이버 제거 스크립트
- **Redhat-Default-Setting.sh** : Reahat Enterprise 서버 기본 세팅 스크립트
- **Ubuntu-Default-Setting.sh** : Ubuntu 22.04 LTS 버전 서버 기본 세팅 스크립트
- **TigerVNC.md** : TigerVNC, X11 등 Remote GPU Rendering + Display 세팅
- **Run-FFmpeg.sh** : x개의 FFmpeg 프로세스 실행 및 .ts파일, .m3u8파일 생성 스크립트

---

## 📂 Jenkins

> **Jenkins Declarative Pipeline & Docker & Nginx를 이용한 Blue/Green 무중단 배포 스크립트 **

- **Server.sh** : RedHat 기반 Server Setting 스크립트
- **Dockerfile** : OpenJDK 이미지 베이스로 내부 명렁어 실행
- **Docker-HA.sh** : Jenkins 배포 시 blue/green 컨테이너 중 미실행 중인 곳에 새 버전 릴리즈 후 로드밸런싱 타겟 변경 / 기존 실행중인 컨테이너 중지
- **jenkinsfile** : Git Commit 시 태그 이름중 특정 단어가 들어간 커밋에만 배포 적용 (이파일에선 "cicd" 키워드 사용)
- **nginx.conf** : blue/green 컨테이너 포트인 8080/8081에 대한 트래픽 로드밸런싱 수행
- **service-url.inc** : Service URL 지정 (nginx.conf 내에 include 됨)