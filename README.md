# Developer Environments Setup

## Macbook

### `Homebrew`

  - Install dependencies for Homebrew

        xcode-select --install

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



If you need to have sqlite first in your PATH, run:
  echo 'export PATH="/opt/homebrew/opt/sqlite/bin:$PATH"' >> ~/.zshrc

For compilers to find sqlite you may need to set:
  export LDFLAGS="-L/opt/homebrew/opt/sqlite/lib"
  export CPPFLAGS="-I/opt/homebrew/opt/sqlite/include"

For pkg-config to find sqlite you may need to set:
  export PKG_CONFIG_PATH="/opt/homebrew/opt/sqlite/lib/pkgconfig"

==> zlib
zlib is keg-only, which means it was not symlinked into /opt/homebrew,
because macOS already provides this software and installing another version in
parallel can cause all kinds of trouble.

For compilers to find zlib you may need to set:
  export LDFLAGS="-L/opt/homebrew/opt/zlib/lib"
  export CPPFLAGS="-I/opt/homebrew/opt/zlib/include"

For pkg-config to find zlib you may need to set:
  export PKG_CONFIG_PATH="/opt/homebrew/opt/zlib/lib/pkgconfig"
