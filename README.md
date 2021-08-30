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







