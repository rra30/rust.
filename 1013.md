# 예비용
까먹었거나 덜적었을때 예비용   
깃허브 작성할때 참고용 링크   
https://gist.github.com/ihoneymon/652be052a0727ad59601   
## Rust
Rust는 C++, C, Java 등 다른언어들과 비슷한점과 겹치는 고유명사의 개념도 있다.    
그렇기에 위에 말한 3가지 언어와 다른 언어들을 알고 한다면 편하다.   
일반적으로 확장자는 **".rs",".rslist"** 가 있다.     
__"Rust"__ 는 웹페이지에서 실행시키는 것과, 로컬에 설치하는 것 2가지가 있다.   
웹페이지의 경우는 아래 링크를 들어가면 끝이다.(파일 만들기도 할 필요 없다.)   
https://play.rust-lang.org/?version=stable&mode=debug&edition=2021   

로컬로 설치할려면 아래 링크에 들어가서   
https://visualstudio.microsoft.com/ko/visual-cpp-build-tools/   
__build-tools__ 를 다운로드 해주고 나서 실행을 해주고,   
아래 사진에 있는 __"C++를 사용한 데스크톱 개발"__ 을 클릭해주고
![스크린샷(32)](https://github.com/user-attachments/assets/6241c17e-3719-4fc6-a036-af96758ce153)   
선택사항도 사진과 같이 선택해주면 된다.(왼만해서는 기본선택되있을것이다.)   
설치가 끝나고 나면   
![스크린샷(33)](https://github.com/user-attachments/assets/7740f3f4-829b-47c6-ad1e-370fc97aa1d2)   
위 사진처럼 시작을 눌러준 다음 켜진 __Developer Command Prompt__ 에서 __"지정된 파일을 찾을 수 없습니다."__ 가 아닌 위 사진처럼 나온다면 성공이다.   
그 다음 아래 링크를 타고 들어가서 환경에 맞는걸 설치하면 끝이다.   
https://www.rust-lang.org/tools/install   

설치를 하고 난다음에는 __"rustup-init.exe"__ 가 설치가 되는데 이걸 실행시켜주면

아래 사진처럼 나오게 될텐데 여기서 (만약에 __Install the C++ build tools before proceeding.__ 이런 에러가 나오면 __build-tools__ 가 설치가 안된것이다.)   
![Untitled design](https://github.com/user-attachments/assets/99a244d4-e876-48f9-86e9-43de9b6d84f8)   
옵션이 3가지가 있는데 1번하는것이 좋다.   
이제 설치가 끝나면 명령프롬프트, 파워쉘 등 환경에 맞는 커맨드 라인을 켜주고   
![스크린샷(34)](https://github.com/user-attachments/assets/7129aebc-1c7a-46b6-9497-6e52e2548899)   
사진처럼 아래의 코드를 입력해보자.
<pre>
  <code>
    cargo --version
    rustc --version
  </code>
</pre>
입력한 후 버전이 나온다면 정상 설치가 된것임으로   
아래 __Rust 프로젝트 만들기__ 로 넘어가도 된다.
### Rust 프로젝트 만들기 (로컬로 설치를 한경우) 
__Rust__ 로 코딩을 하기 위해서는 일단 __VSCode__ 에서 할 것 임으로 __VSCode__ 도 설치를 해 줘야만 한다.   
__VSCode 설치링크__
https://code.visualstudio.com/download   
환경에 맞게 설치를 해주고   
이제 cmd, ps1, 등 커맨드 라인들을 이용해서 러스트 프로젝트 생성을 해야한다.   
환경을 생성하는 코드는
<pre>
  <code>
    cargo new (원하는 이름)
  </code>
</pre>
**이 코드를 입력할때 만약 위치가 "C:/" 에 있다면 그 위치에 프로젝트가 생성된다.**   

### Rust 프로젝트 생성 후 확인
프로젝트 생성 후 VSCode 에서 파일(프로젝트 이름.rs) 실행을 시켜보면 아래 코드가 입력되있는걸 볼수 있다
<pre>
  <code>
    fn main() {
      println!("Hello, World!");
    }
  </code>
</pre>
이 코드를 실행을 시킨다면, **"Hello, World!"** 가 출력되게 된다.

