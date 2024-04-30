# java-console (JAR Library)

`java-console.jar` is a Java library that provides utility classes for console-based interaction in Java applications. This library includes classes for handling notifications, working with lists, and scanning user input.

## Features

- **NotificationHandler**
    - Check for data presence in a list and display status messages.
    - Notify about specific actions with customizable messages.

- **ListUtils**
    - Display the contents of a list with indexed numbering.
    - Check if a list is not null and not empty.

- **Scan**
    - Scan and retrieve user input for strings, integers, doubles, and `BigDecimal` values.
    - Prompt users with customizable messages for input.

- **ColorConstants**
    - Provides ANSI color constants for styling console output with colors.

## Usage

1. **Download**
    - Download the `java-console.jar` file.

2. **Include in Your Project**
    - Add `java-console.jar` to your Java project's classpath.

3. **Import Required Classes**
    - Import the necessary classes in your Java files:
      ```java
      import com.pdp.backend.NotificationHandler;
      import com.pdp.backend.ListUtils;
      import com.pdp.backend.Scan;
      import com.pdp.support.ColorConstants;
      import com.pdp.support.Ui;
      ```

4. **Use the Utility Classes**

    - **NotificationHandler**
      ```java
      NotificationHandler.checkData(myList);
      NotificationHandler.notifyAction("Object", "creation", true);
      ```

    - **ListUtils**
      ```java
      ListUtils.displayList(myList);
      boolean hasData = ListUtils.checkDataForNotNull(myList);
      ```

    - **Scan**
      ```java
      String userInput = Scan.scanStr("Enter your name");
      int userAge = Scan.scanInt("Enter your age");
      ```

    - **ColorConstants**
      ```java
      System.out.println(ColorConstants.ANSI_GREEN + "Success!" + ColorConstants.ANSI_RESET);
      ```

## Dependencies
- This JAR file may require Java Runtime Environment (JRE) 8 or later.