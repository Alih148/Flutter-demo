import 'package:flutter/material.dart';

void main() => runApp(const MyApp());

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Flutter Demo Difficulty level 100',
      debugShowCheckedModeBanner: false,
      theme: ThemeData(
        primarySwatch: Colors.blue,
      ),
      home: const MyHomePage(title: 'PAWS Saver Zamboanga City'),
    );
  }
}

class MyHomePage extends StatefulWidget {
  final String title;

  const MyHomePage({
    super.key,
    required this.title,
  });

  @override
  State<MyHomePage> createState() => _MyHomePageState();
}

class _MyHomePageState extends State<MyHomePage> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text(widget.title,
            style: TextStyle(
              color: Colors.white,
            )),
        backgroundColor: Colors.blue,
      ),
      body: Column(children: [
        SizedBox(height: 20), // top margin
        Row(
          mainAxisAlignment: MainAxisAlignment.spaceEvenly,
          children: [
            Container(
              decoration: BoxDecoration(
                border: Border.all(color: Colors.grey),
                borderRadius: BorderRadius.circular(5),
                color: Colors.blue,
              ),
              height: 200,
              width: 100,
              
                child: Column(
                  mainAxisAlignment: MainAxisAlignment.end,
                  children: [
                    Text('Tite 1', style: TextStyle(color: Colors.black, fontSize: 24, fontWeight:                             FontWeight.bold,)),
                    Text('Hellow Worls', style: TextStyle(color: Colors.black)),
                  ],
                ),
              ),
            
            Container(
              decoration: BoxDecoration(
                border: Border.all(color: Colors.grey),
                borderRadius: BorderRadius.circular(5),
                color: Colors.blue,
              ),
              height: 200,
              width: 100,
              child: Column(
                  mainAxisAlignment: MainAxisAlignment.end,
                  children: [
                    Text('Title 2', style: TextStyle(color: Colors.black, fontSize: 24, fontWeight:                             FontWeight.bold,)),
                    Text('Hellow World', style: TextStyle(color: Colors.black)),
                  ],
                ),
            ),
            Container(
              decoration: BoxDecoration(
                border: Border.all(color: Colors.grey),
                borderRadius: BorderRadius.circular(5),
                color: Colors.blue,
              ),
              height: 200,
              width: 100,
              child: Column(
                  mainAxisAlignment: MainAxisAlignment.end,
                  children: [
                    Text('Title 3', style: TextStyle(color: Colors.black, fontSize: 24, fontWeight:                             FontWeight.bold,)),
                    Text('Hellow World', style: TextStyle(color: Colors.black)),
                  ],
                ),
            ),
          ],
        ),
      ]),
    );
  }
}
