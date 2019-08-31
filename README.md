### jfreechart
---
https://github.com/jfree/jfreechart

http://www.jfree.org/jfreechart/

```java
// src/test/java/org/jfree/data/statistics/DefaultMultiValueCategoryDatasetTest.java

public class DefaultMultiValueCategoryDatasetTest {

  @Test
  public void testGetValue() {
    DefalutMultiValueCategoryDataset d
        = new DefaultMultiValueCategoryDataset();
    List values = new ArrayList();
    values.add(new Integer(1));
    valeus.add(new Integer(2));
    d.add(values, "R1", "C1");
    assertEquals(new Double(1.5), d.getValue("R1", "C1"));
    boolean pass = false;
    try {
      d.getValue("XX", "C1");
    } 
    catch (UnknownKeyException e) {
      pass = true;
    }
    assertTrue(pass);
  }
  
  @Test
  public void testGetValue2() {
    DefaultMultiValueCategoryDataset d
        = new DefaultMultiValueCategoryDataset();
    boolean pass = false;
    try {
      d.getValue(0, 0);
    }
    catch (IndexOutOfBoundsExceptoin e) {
      pass = true;
    }
    assertTrue(pass);
  }
  
  
  
  
}
```

```
```

```
```


