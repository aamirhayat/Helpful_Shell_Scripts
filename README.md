# Helpful_Shell_Scripts

# Helpful_Shell_Scripts

#### Rename the image files inside a folder in increasing number
```
find . -name '*.jpg' | gawk 'BEGIN{ a=1 }{ printf "mv \"%s\" %04d.jpg\n", $0, a++ }' | bash
```

#### Move the selected images from one folder to another
```
cp /home/user/{1,4,7,10}".png" /home/user/Documents/c1
```
####  Make copy of a file 100 times with diff name from command line
```
for i in {1..100}; do cp test.ogg "test$i.ogg"; done
```
