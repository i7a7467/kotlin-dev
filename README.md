### init command
```
gradle init --type=kotlin-application

# change package name
old_pkg="org.example"; new_pkg="com.github.i7a7467"; find . -type f \( -name "*.kt" -o -name "*.kts" \) -exec sed -i '' "s/$old_pkg/$new_pkg/g" {} +

# move files
mkdir -p app/src/main/kotlin/com/github/i7a7467

mv app/src/main/kotlin/org/example/*.kt app/src/main/kotlin/com/github/i7a7467/

rmdir app/src/main/kotlin/org
```