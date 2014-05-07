# Android note

## 利用android-support, appcompat包支持多版本兼容

代码在不同版本之间用的是同一套代码，即基于android-support的代码，而在资源文件中
如res/values下，尤其对样式的指定时，需要对不同的版本分别指定样式,


## Fragment

Fragment 在config changes的时候，可以被保留，但是view
widget还是需要被重新创建的,即onCreateView, onActivityCreated等还是会被调用。



