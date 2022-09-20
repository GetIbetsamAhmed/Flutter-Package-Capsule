## FLUTTER_RECIPE_PACKAGE # 1 ( Page Transaction )
It is really easy to use! You should ensure that you add the page_transition as a dependency in your flutter project.
<br>Installing command
```bash
page_transition: "^2.0.9" | "any"
```
Than you can use it with below examples.
```bash
Navigator.push(context, PageTransition(type: PageTransitionType.fade, child: DetailScreen()));

Navigator.push(context, PageTransition(type: PageTransitionType.leftToRight, child: DetailScreen()));

Navigator.push(context, PageTransition(type: PageTransitionType.rightToLeft, child: DetailScreen()));

Navigator.push(context, PageTransition(type: PageTransitionType.rightToLeft, child: DetailScreen(), isIos: true));

Navigator.push(context, PageTransition(type: PageTransitionType.topToBottom, child: DetailScreen()));

Navigator.push(context, PageTransition(type: PageTransitionType.bottomToTop, child: DetailScreen()));

Navigator.push(context, PageTransition(type: PageTransitionType.scale, alignment: Alignment.bottomCenter, child: DetailScreen()));

Navigator.push(context, PageTransition(type: PageTransitionType.size, alignment: Alignment.bottomCenter, child: DetailScreen()));

Navigator.push(context, PageTransition(type: PageTransitionType.rotate, duration: Duration(second: 1), child: DetailScreen()));

Navigator.push(context, PageTransition(type: PageTransitionType.rightToLeftWithFade, child: DetailScreen()));

Navigator.push(context, PageTransition(type: PageTransitionType.leftToRightWithFade, child: DetailScreen()));

Navigator.push(context, PageTransition(type: PageTransitionType.leftToRightJoined, child: DetailScreen(), childCurrent: this));

Navigator.push(context, PageTransition(type: PageTransitionType.rightToLeftJoined, child: DetailScreen(), childCurrent: this));

Navigator.push(context, PageTransition(type: PageTransitionType.topToBottomJoined, child: DetailScreen(), childCurrent: this));

Navigator.push(context, PageTransition(type: PageTransitionType.bottomToTopJoined, child: DetailScreen(), childCurrent: this));

Navigator.push(context, PageTransition(type: PageTransitionType.leftToRightPop, child: DetailScreen(), childCurrent: this));

Navigator.push(context, PageTransition(type: PageTransitionType.rightToLeftPop, child: DetailScreen(), childCurrent: this));

Navigator.push(context, PageTransition(type: PageTransitionType.topToBottomPop, child: DetailScreen(), childCurrent: this));

Navigator.push(context, PageTransition(type: PageTransitionType.bottomToTopPop, child: DetailScreen(), childCurrent: this));
```
