## FLUTTER_RECIPE_PACKAGE No. 1 ( Page Transactions )
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

## FLUTTER_RECIPE_PACKAGE No. 2 ( Zoom Widget )
With this widget you can create a customizable canvas in which you can zoom in flutter.
<br>Installing command
```bash
zoom_widget: ^2.0.0 | "any"
```
Than you can use it with below examples.
```
Zoom(
  backgroundColor: Colors.white,
  initTotalZoomOut: true,
  child: Center(
    child: Image(
      image: NetworkImage("https://ichef.bbci.co.uk/news/640/cpsprodpb/C120/production/_104304494_mediaitem104304493.jpg"),
      fit: BoxFit.cover,
      frameBuilder: (context, child, frame, wasSynchronouslyLoaded) {
        return Padding(
          padding: const EdgeInsets.all(0.0),
          child: wasSynchronouslyLoaded ? child : child,
        );
      },
    ),
  ),
),
```
It is really easy to use! You should ensure that you add the Reorderable ListView as a dependency in your flutter project.
<br>Installing command
```bash
reorderable_grid_view: ^2.2.5
```
Than you can use it with below examples.
```
ReorderableGridView.count(
  crossAxisSpacing: 10,
  mainAxisSpacing: 10,
  crossAxisCount: 3,
  children: this.data.map((e) => buildItem("$e")).toList(),
  onReorder: (oldIndex, newIndex) {
    setState(() {
      final element = data.removeAt(oldIndex);
      data.insert(newIndex, element);
    });
  },
  footer: [
    Card(
      child: Center(
        child: Icon(Icons.add),
      ),
    ),
  ],
);
```
## FLUTTER_RECIPE_PACKAGE No. 3 ( Video calling )

