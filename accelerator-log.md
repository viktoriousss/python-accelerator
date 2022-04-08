# Accelerator Log

## Options
```json
{
  "branch" : "main",
  "description" : "Python Accelerator",
  "icon" : "https://raw.githubusercontent.com/simple-starters/icons/master/icon-tanzu-light.png",
  "name" : "python",
  "projectName" : "python-accelerator",
  "url" : "https://github.com/TanzuDK/python-accelerator.git"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(Combo, UniquePath)
┃ ┏ engine.transformations[0] (Combo)
┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseLast))
┃ ┃ engine.transformations[0].merge (Chain)
┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┏ engine.transformations[0].merge.transformations[0] (Merge)
┃ ┃ ┃  Info Running Merge(YTT, Combo)
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0] (YTT)
┃ ┃ ┃ ┃ Debug Wrote values file with json content:   {"artifactVersion":"0.0.1-beta","icon":"https://raw.githubusercontent.com/simple-starters/icons/master/icon-tanzu-light.png","name":"python","description":"Python Accelerator","artifactId":"python-accelerator","projectName":"python-accelerator","branch":"main","url":"https://github.com/TanzuDK/python-accelerator.git"}
┃ ┃ ┃ ┗  Info Shelling out to YTT with args: [ytt, -f, /tmp/ytt-input1077696718254603690, --data-values-file, /tmp/accelerator-options4327946463648788287.json, --output-files, /tmp/ytt-output15233986437842771132]
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[1].include (Include)
┃ ┃ ┃ ┃  Info Will include [README.md]
┃ ┃ ┃ ┃ Debug LICENSE didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ Debug README.md matched [README.md] -> included
┃ ┃ ┃ ┃ Debug k8s-resource.yaml didn't match [README.md] -> excluded
┃ ┃ ┗ ┗ Debug new-accelerator.yaml didn't match [README.md] -> excluded
┃ ┗ ╺ engine.transformations[0].merge.transformations[1] (UniquePath)
┗ ╺ engine.transformations[1] (UniquePath)
```
