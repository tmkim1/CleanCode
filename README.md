# CleanCode
CleanCode - Robert Cecil Martin

[서문 - 이해영] 
- 아무런 자극이 없으면 그 단계를 벗어나지 못한다.
- <b>많이 고민하고 생각</b>하는 만큼 여러분의 프로그래밍 실력이 늘어나리라 믿는다. 

[들어가면서] 
- <b>장인 정신</b>
  -   원칙, 패턴, 기법, 경험이라는 지식을 습득해야 한다.
  -   열심히 일하고 연습해 지식을 몸과 마음으로 체득해야 한다.

[깨끗한 코드] 
- 제대로 명시한 요구사항은 코드만큼 정형적이며 테스트 케이스로 사용해도 좋다.
- 구긍적으로 코드는 요구사항을 표현하는 언어라는 사실을 명심한다. 
- 르블랑의 법칙, <b> 나중은 결코 오지 않는다. </b>
- 기한을 맞추는 유일한 방법: 언제나 코드를 최대한 깨끗하게 유지하는 습관 

- 중복을 피하라.
- 한 기능만 수행하라.
- 제대로 표현하라.
- 작게 추상화하라.

[의미 있는 이름]
- 의도를 분명히 밝혀라 

``` JAVA
public List<Cell> getThem() {
  List<int[]> list1 = new ArrayList<int[]>();
  for (int[] x: theList)
    if (x[0] == 4)
      list1.add(x);
  return list1;
}
``` 

``` JAVA
public List<Cell> getFlaggedCelss() {
  List<Cell> flaggedCells = new ArrayList<Cell>();
  for (Cell cell: gameBoard)
    if (cell.isFlagged())
      flaggedCells.add(cell);
  return flaggedCells;
}
``` 

- 그릇된 정보를 피하라
  - 변수 명에 컨테이너 명을 포함하기 보다는 accounts, acccountGroup과 같이 사용
  - 실제 List Type이 아니라면, accountList라 명명하지 않는다.

- 발음하기 쉽고, 검색하기 쉬운 이름을 사용하라.

- 클래스: 명사나 명사구, 메서드: 동사나 동사구 

- 기발한 이름은 피하라 (농담, 소수만 아는 단어 등)

- 의미 있는 맥락을 추가하라
  - firstName, lastName 과 같은 변수명만 봐서는 무엇을 의미하는 Name인지 이해하기 어려움
  - addrFirstName, addrLastName과 같이 맥락을 분명히 해주도록 하거나 Address 클래스를 생성하여 사용해주도록 한다. 
  
[함수] 

- 작게 그리고 더 작게
- 함수는 한 가지 기능만 수행
- 서술적인 이름을 사용
  - testableHtml -> SetupTeardownIncluder.render (함수가 하는 일을 표현) 
- 함수의 인수 갯수는 적을수록 좋다, 플래그 인수는 최악 (함수가 한꺼번에 여러 가지를 처리한다고 대놓고 공표하는 셈) 







