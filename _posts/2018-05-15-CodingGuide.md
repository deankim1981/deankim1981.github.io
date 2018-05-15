### Coding Convention

- [코딩 규칙 #1](http://www.csharpstudy.com/Guide/Coding-guide.aspx), [코딩 규칙 #2](https://docs.microsoft.com/ko-kr/dotnet/csharp/programming-guide/inside-a-program/coding-conventions) 를 준수한다.
- Private Field, Parameter Variable : Camel Case Style
- Event, Property, Function, Const : Pascal Case Style
- 예외적으로 Private Field의 경우 _(underscore)를 붙인다.

### Xml Namespace 선언 방법
- View : xmlns:v
- ViewModel : xmlns:vm
- Model : xmlns:m
- ValueConverter : xmlns:vc
- UserControl : xmlns:uc
- Commons.Commands : xmlns:cmd
- Selector : xmlns:sel

### log4net 설정 및 사용
- NuGet 패키지 설치 (log4net)
- AssemblyInfo.cs 로그 설정 추가 ([assembly: log4net.Config.XmlConfigurator(Watch = true)])
- App.config 로그 섹션 및 기록 방법 설정
- 로거 인터페이스를 이용하여 로그를 기록 (ILog log = LogManager.GetLogger(typeof(ClassName)));
- 로그 레벨 7가지 사용 (ALL, OFF, Debug, Info, Warn, Error, Fatal)
- 로그 사용시 Perfomance 관련하여 Level 체크 필요 (IsDebugEnabled, IsErrorEnabled...)

