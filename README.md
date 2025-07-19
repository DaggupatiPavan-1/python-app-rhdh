pkg=./
archive=$(npm pack --silent $pkg )
tar -xzf "$archive" && rm "$archive"
finalName=$(echo $archive | sed -e 's:\.tgz$::')
rm -fr "$finalName"
mv package "$finalName"
mv "$finalName" ~/rhdh/dynamic-plugins-root/

### ~/rhdh/dynamic-plugins/wrappers/backstage-community-plugin-*/
```
yarn build
yarn tsc
```
```
pkg=./
archive=$(npm pack --silent $pkg )
tar -xzf "$archive" && rm "$archive"
finalName=$(echo $archive | sed -e 's:\.tgz$::')
rm -fr "$finalName"
mv package "$finalName"
mv "$finalName" ~/rhdh/dynamic-plugins-root/
```
run above script in <here we need to run the script>

it generate a folder called backstage-community-plugin-rbac-1.42.0 <something like this>

#mv backstage-community-plugin-rbac-1.42.0 ~/rhdh/dynamic-plugins-root/

#move to dynamic-plugin-root/ directory
