## Hey, this is us 👋

안녕하세요, 방문해주셔서 감사합니다. 저희는 이 곳에 [블로그](https://cse-study.github.io/main/home/)를 만들어 CS 관련 스터디를 진행하고 있습니다. 현재는 알고리즘/코테 스터디와, 간단한 AI 스터디를 진행하고 있습니다! 

- `blog`: 블로그의 전체 컨텐츠를 저장하는 공간입니다. 블로그 UI와 관련된 모든 작업이 이 곳에서 이루어지며, 아래 세 개의 저장소를 submodule로 가집니다.
- `cse-study.github.io` (`blog/public` submodule): Hugo 블로그 배포를 위한 저장소입니다.
- `algorithm` (`blog/content/algorithm` submodule): 알고리즘, 코딩테스트 스터디 자료를 저장하는 공간입니다.
- `weekly-ai` (`blog/content/ai` submodule): AI 관련 소식, 정보를 공유하는 공간입니다.

전체 배포 과정은 아래의 순서로 진행됩니다. Github action으로 자동화하여 유지/보수의 수고를 최대한 덜고자했습니다 🙌 (...아직 적용되지 않았습니다.)

1. `algorithm`, `weekly-ai` 저장소에 마크다운 파일 업로드(push)
2. `blog` 저장소에 `algorithm`, `weekly-ai`의 변경사항 자동으로 반영
3. `blog` 저장소에 변경사항이 생길 때 마다 배포용 스크립트가 동작하면서, `cse-study.github.io`에 블로그 자동으로 배포

