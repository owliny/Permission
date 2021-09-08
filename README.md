# Permission
설정 파일에 작성하는 명세에는 권한 명세와 기능 명세 2가지가 있습니다.
권한명세는 해당 데이터나 기능의 사용여부를 설정하고,기능명세는 해당 기능이 있는 안드로이드폰에서만 내려받을 수 있도록 플레이스토어에서 내려받는 것을 방지합니다
권한은 일반권한, 위험권한, 서명권한 세가지 보호수준으로 나뉩니다.
일반 권한으로 설정파일인 AndroudMenifest.xml에 명세하면 설치 시 사용자에게 권한 승인을 묻는 팝업창을 보여줍니다. 인터넷 사용, 알람 설정 등이 일반 권한에 포함됩니다.
위험권한은 앱이 사용자의 개인정보와 관련된 데이터나 기능을 액세스 하거나 다른 앱 및 기기의 작동에 영향을 줄 우려가 있는 권한입니다.
서명 권한은 권한을 사용하려는 앱이 권한을 정의하는 앱과 동일한 인증서로 서명된 경우 시스템은 권한을 자동으로 부여합니다.
풀어서 설명하면 구글에서 만든 앱은 권한이 자동으로 부여되는 것과 같다. 
권한 요청 흐름: 1.앱이 권한을 요청한다-예:사용권한을 정의한다.-사용권한을 정의한다-정의한 권한이 위험권한인가?-예:실행시간에 권한 요청-코드실행
                                      아니요:권한을 사용하지 않는다-코드 실행                                아니요:코드 실행
출처: 이것이 안드로이드다, 고돈호 지음,한빛 미디어
