<div align="center">
   <picture>
      <img src="./ReadmeAssets/octo.png" width="150" height="150">
   </picture>
   <h2>Luna</h2>
</div>

# Luna: The Future of Native Linux Development

Welcome to Luna, a groundbreaking new programming language crafted specifically for the Linux ecosystem. Imagine the elegance and power of Swift and SwiftUI, but built from the ground up to thrive on your favorite open-source platform. Luna isn't just another language; it's a complete development experience designed to empower Linux developers to create stunning, high-performance applications with unparalleled ease.

## Why Luna?

For too long, Linux developers have yearned for a truly modern, intuitive language with integrated UI capabilities that rivals the best on other platforms. Luna answers that call. We're bringing:

- Swift-Inspired Syntax: If you love Swift's clean, expressive, and safe syntax, you'll feel right at home with Luna. We've adopted its best features to provide a highly readable and enjoyable coding experience.

- Native Linux Focus: Luna is engineered to be a first-class citizen on Linux. This means deep integration with system services, optimized performance, and a language that feels truly "at home" on your distribution.

- Intuitive GUI Development: Forget complex, arcane UI frameworks. Luna includes a powerful, declarative UI framework—much like SwiftUI—that lets you build beautiful, responsive graphical applications with minimal code. Design your interfaces visually and bring them to life with Luna's elegant syntax.

- Robust Package Management: Building and distributing your applications has never been easier. Luna features its own sophisticated package manager, lunapack, for seamless dependency management. But we go a step further: Luna can effortlessly export your projects into widely used Linux package formats like .deb (for Debian/Ubuntu), .rpm (for Fedora/RHEL), and Pacman packages (for Arch Linux), ensuring your creations are easily installable by anyone. We even support Flatpak for universal distribution!
  Getting Started with Luna
  Ready to embark on your Luna journey? Here's how to get started:
  Installation
  To install Luna, simply run our convenient setup script:
  
  > not avalable yet !

This will install the Luna compiler, the lunapack package manager, and the Luna UI framework.
Your First Luna Program: "Hello, Linux!"
Let's write a classic. Create a file named hello.luna and add the following:

```
// hello.luna
import Foundation // For basic I/O operations

func main() {
 print("Hello, Linux!")
}
```

Now, compile and run it from your terminal:

```
luna run hello.luna
```

You should see: Hello, Linux!
Building a Simple GUI App
Creating a windowed application is just as straightforward. Consider this my_app.luna example:

```
// my_app.luna
import LunaUI // Our native UI framework

struct MyApp: App {
 var body: some View {
 Window("My First Luna App") {
 VStack { // Vertical Stack
 Text("Welcome to Luna!")
 .font(.largeTitle)
 .padding()

            Button("Click Me!") {
                print("Button was clicked!")
            }
        }
    }
}


}

// Entry point for the application
LunaUI.runApp(MyApp())
```

Compile and run this, and you'll have a native Linux window with a title, text, and a clickable button!

```
luna build
```

Packaging Your Luna Application
One of Luna's superpowers is its integrated packaging capabilities. After compiling your application, you can easily create distribution-ready packages:

```
#Create a .deb package
lunapack export --format deb

#Create an .rpm package
lunapack export --format rpm

# Create a Pacman package
lunapack export --format pacman

# Create a Flatpak
lunapack export --format flatpak
```

This generates the respective package files in your project directory, ready for distribution on various Linux distributions.

## Contributing to Luna

Luna is an ambitious open-source project, and we welcome contributions from developers of all skill levels! Whether you want to fix bugs, implement new features, improve documentation, or just spread the word, your help is invaluable.
Please refer to our CONTRIBUTING.md for detailed guidelines on how to get involved.

## License

Luna is released under the MIT License. This means it's free to use, modify, and distribute, even for commercial purposes.