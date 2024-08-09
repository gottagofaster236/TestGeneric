```java
package org.example;

import java.util.EnumMap;

@SuppressWarnings({"rawtypes", "unchecked"})
public class Main {
    private enum MyEnum { VALUE }

    public static void main(String[] args) {
        EnumMap map = new EnumMap(MyEnum.class);
        Object value = MyEnum.VALUE;
        map.put(value, "value");
        System.out.println("It works!");
    }
}
```
