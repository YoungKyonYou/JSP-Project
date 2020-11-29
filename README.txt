//////////기본 배점(3점)//////////
1. 모델 2 방식으로 프로그램 작성(MVC 패턴)
-controlServlet.java
-pControlServlet.java

2. CSS 파일 분리 작성
-index.jsp<->home.css
-register.jsp<->register.css
-home.jsp<->main.css
-grands.jsp<->grands.css, bootstrap.min.css
-grand.jsp<->bootstrap.min.css
-uprights.jsp<->grands.css, bootstrap.min.css
-upright.jsp<->bootstrap.css
-pianist.jsp<->pianist.css
-mypage.jsp<->mypage.css
-login.jsp<->login.css
-rank.jsp<->rank.css

3. 모델 기능은 VO, DAO 클래스를 분리해서 작성
-PersonDAO.java, PianistDAO.java, PianoDAO.java, RankDAO.java
-PersonVO.java, PianistVO.java, PianoVO.java, RankVO.java

4. 자바 클래스 역할 별(Controller, Persistence, Domain) 패키지 분리 작성
-Controller
-Domain, pianist.domain, piano.domain
-Persistence, pianist.persistence, piano.persistence

5.JDBC를 사용하여 CRUD를 구현할 것(R(Read)는 목록보기 기능 포함)
Create->Insert=PersonDAO.add() 함수
Read->Select=RankingDAO.read() 함수->rank.jsp에서 사용
Update->Update=PersonDAO.update() 함수
Delete->Delete=PersonDAO.delete() 함수
///////////////////////////////////////////////////////////////////////////////

//////////추가(3점)//////////
1. 표현 언어
-grands.jsp, grands.jsp, home.jsp, login.jsp, mypage.jsp, pianist.jsp, register.jsp, upright.jsp, uprights.jsp

2. 커스텀 태그 사용
-WEB-INF/tags/info.tag, WEB-INF/tags/info2.tag, WEB-INF/tags/info3.tag, WEB-INF/tags/info4.tag
-home.jsp-info.tag, info2.tag, info3.tag
-index.jsp-info4.tag
-rank.tag-rank.jsp

3. JSTL 사용
-grands.jsp-><c:forEach>사용
-uprights.jsp-><c:forEach> 사용
-pianist.jsp-><c:forEach> 사용
-rank.tag-><c:forEach> 사용
///////////////////////////////////////////////////////////////////////////


