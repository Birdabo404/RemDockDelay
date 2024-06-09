# RemDockDelay

This simple repo eliminates the annoying lag on macOS dock, making your Dock feel snappier and more responsive.

## Features

* Eliminates Dock auto-hide delay.
* Lightweight and easy to use.
* Open source (MIT License).
  
## 🔧 Installation

1. Open your Terminal app.
2. Paste and run one of the following commands, depending on your preference:

   **Keep smooth animation time, but remove delay:**

   ```bash
   defaults write com.apple.dock autohide-delay -float 0; killall Dock
   ```
   
   **Instant Reveal, Zero animation:**
   
   ```bash
   defaults write com.apple.dock autohide-time-modifier -int 0; killall Dock
   ```

   **If you want to restore the default behavior, use this command:**
   ```bash
   defaults delete com.apple.dock autohide-delay; killall Dock
   ```
