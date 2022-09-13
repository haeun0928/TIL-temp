# Today I learned
> 매일매일 배운 것을 기록합니다.

##2022-09-13
### RPA 1기, 웹프로그래밍 기획과 기본
#### 리눅스 커맨드라인 기초
- 'pwd': print working directory의 약자로 현재 작업 경로를 출력해주는 명령어
- 'cd': change directory의 약자로 현재 작업 경로를 변경할 때 쓰는 명령어
  - 절대 경로는 '/'로 시작함
  - 상위 경로는 '..'으로 나타냄
  - 'tab'을 사용하면 경로 자동 완성이 됨
- 'ls': list의 약자로 현재 작업 경로에 있는 파일이나 디렉터리를 출력해주는 명령어
  - 'ls', '-a', 'ls -l', 'ls -al'과 같은 옵션을 붙일 수 있음
#### vim 사용법
- 명령 모드와 입력모드
  - vim에디터를 열때는 명령 모드로 진입함
  - 명령모드에서는 입력이 불가능
  - 입력을 하려면 입력모드로 바꿔야 함
    - 키보드에서 'i'를 누름
  - 입력이 끝나고, 저장하고 나오려면 명령 모드로 바꿔야함
    - 키보드에서 'ESC' 누름
  - 입력 가능한 명령어
    - ':w': 저장하기
    - ':q': 나오기
    - ':wq': 저장하고 나오기
    
  - 참고자료 [링크](http://zeddios.tistory.com/122)
- 비정상적으로 종료시 해결 방법
  - vim이 비정상 종료 되었을 때 'swp'파일이 생성됨
    - ATTENTION 문구가 뜨는 경후
      1. 두 프로세스, 두 사람이 동시에 한 파일을 수정하는 경우
      2. crash가 나서 vim이 비정상적으로 닫힌 경우
  - 기존에 입력했던 내용을 복구하고 싶을 때는 'vim -r파일명'을 입력하거나 Recovery모드로 진입
  - 정상 종료후, swp파일 삭제
    - 'rm .789.txt.swp'<-- 'rm'명령어는 remove 약자

#### 마크다운 문법
#외부 링크 추가
* 외부링크
```
사용문법: [Title](link)
적용예: [Google](https://google.com, "google link")
```
Link: [Google](https://google.com, "google link")

```java
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```
