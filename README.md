# PyConsole
os console in python
- 자주 사용하는 파일 및 디렉토리 탭누르면 자동 완성
- 멀티쓰레드로 작업
- Queue에 작업을 요청하면 진행하는 방식 ( 예를 들면 svn cleanup, svn update, svn revert 등 여러명령을 한번에 시켜놓으면 순차적으로 처리 )
- Windows, Linux 모두 동일한 명령어 사용
- QT GUI

함수를 wrapping하여 사용하는 방식 
```
def dir():
    if os.isWindows:
        return os.system('dir')
    else:
        return os.system('ls')
```
기본적으로 python console을 그대로 사용한다
