# flutter code:
import 'package:flutter/material.dart';  

void main() {
  runApp(const MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(                 
      debugShowCheckedModeBanner: false, 
      home: Scaffold(
        appBar: AppBar(
          title: const Text("cubic page"), 
          backgroundColor: Colors.blue,
        ),
        body: Center(
          child: Container(
            width: 150,
            height: 150,
            color: Colors.red,
          ),
        ),
      ),
    );
  }
}
