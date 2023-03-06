# Developer Environments Setup

## Macbook

### `Homebrew`

  - Install Homebrew
  
        /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
  
  -  Add Homebrew to PATH
  
        (echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> /Users/amiteshrai/.zprofile

  - eval "$(/opt/homebrew/bin/brew shellenv)"
 
### `git`

  - Install git
  
        brew install git
  
  - If you need to have curl first in your PATH, run:
  
        echo 'export PATH="/opt/homebrew/opt/curl/bin:$PATH"' >> ~/.zshrc
  
  - For compilers to find curl you may need to set:
  
        export LDFLAGS="-L/opt/homebrew/opt/curl/lib"
        export CPPFLAGS="-I/opt/homebrew/opt/curl/include"
  
  - For pkg-config to find curl you may need to set:
  
        export PKG_CONFIG_PATH="/opt/homebrew/opt/curl/lib/pkgconfig"
