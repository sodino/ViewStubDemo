ViewStubDemo 
在Android开发中，经常会遇到这样的情况，
	在程序运行过程中动态的根据当前条件来决定是否显示某个控件或布局，这时就可以使用惰性控件ViewStub来方便的完成这一功能。
惰性控件ViewStub是一个轻量级的View，可以实现动态布局加载。
ViewStub对象是一个看不见的，零大小的视图，并在程序运行时根据需要进行动态加载。
只有当ViewStub对象被设置为可见，或是调用了ViewStub.inflate()方法时，ViewStub对象所指向的布局才会被实例化，并加载到指向的父布局中。
这样，便通过惰性控件ViewStub实现了动态加载某个控件或布局。

 ViewStub组件和<include>标签的作用类似，主要是为了提高布局的重用性，及布局的模块化。
 它们之间最大的差别是:
 	ViewStub中的布局不会随着它所在布局的渲染而渲染，
 	而<include>标签中的布局会随着它所在布局的渲染而渲染，
 	ViewStub中的布局只有在你需要的时候才会渲染到主界面中。

在本篇博文中，我们将通过一个实例来演示如何使用惰性控件ViewStub完成动态加载布局操作。


参考:
http://www.cnblogs.com/menlsh/archive/2013/03/17/2965217.html
http://blog.csdn.net/mayingcai1987/article/details/6238609