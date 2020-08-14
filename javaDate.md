# Java Date

## code :
```Java
package javaDATE;

import java.util.Date;
import java.time.LocalDate;
import java.time.LocalTime;
import java.time.LocalDateTime;
import java.time.format.DateTimeFormatter;

public class DateDEMO {

	public static void main(String[] args) {
		
		Date myDate = new Date();
		System.out.println(myDate);
		
		LocalDate myLDate = LocalDate.now();
		System.out.println(myLDate);
		
		LocalTime myLTime = LocalTime.now();
		System.out.println(myLTime);
		
		LocalDateTime myLDnT = LocalDateTime.now();
		System.out.println(myLDnT);
		
		DateTimeFormatter FormatterObj = DateTimeFormatter.ofPattern("dd-MM-yyyy   HH:mm:ss");
		System.out.println(myLDnT.format(FormatterObj));
		
		
	}

}

```

## output :
````java
Fri Aug 14 15:10:48 IST 2020
2020-08-14
15:10:48.287
2020-08-14T15:10:48.287
14-08-2020   15:10:48
````