#### Replace first line with string
```
sed "1s=.*=String to be inserted=" original.txt > updated.txt
```

#### Remove first line of a file
```
sed '1d' $filename > $new_filename
```

#### Remove last line of a file
```
sed -i '$ d' $filename
```

#### Remove first and last lines of a file at once
```
sed -i '1d;$d' $filename
```

#### Replace occuranses of a string
```
sed s/"string_to_replace"//g file.txt
```

#### Replace string with the other one
```
sed -i s/string_to_replace/new_string/g file.txt
```

#### Replace string with URL
```
sed -i s,placeholder,http://example.com,g file.txt
```
