# Useful Java Code Snippets

### Converting Strings to `int`, and `int` to String

```
String numToString = String.valueOf(2); // integer converted to numeric string
int stringToNum = Integer.parseInt(numToString); //numeric string converted to int
```

### Append text to file
```
BufferedWriter out = null;
try {
    out = new BufferedWriter(new FileWriter("filename", true));
    out.write("aString");
} catch (IOException e) {
    // errror processing code
} finally {
    if (out != null) {
        out.close();
    }
}
```