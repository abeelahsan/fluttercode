# flutter code:
import 'package:flutter/material.dart';   // ✅ Missing import

void main() {
  runApp(const MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(                 // ✅ Removed const (optional for beginners)
      debugShowCheckedModeBanner: false, // ✅ Optional
      home: Scaffold(
        appBar: AppBar(
          title: const Text("cubic page"), // ✅ const added
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
