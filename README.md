# install_older_geth_ubuntu
Cách cài đặt phiên bản cũ hơn của go-ethereum trên ubuntu
# Cài đặt các dependency cần thiết
  - sudo apt-get install software-properties-common
  - sudo add-apt-repository -y ppa:ethereum/ethereum
  - sudo apt-get update
# Cài đặt golang
  - sudo apt-get install -y golang
# Clone go-ethereum trên git về
  - git clone https://github.com/ethereum/go-ethereum.git
  - cd go-ethereum
  - git checkout v[geth-version]
  - make geth
# Kiểm tra phiên bản geth
  - ./build/bin/geth version

# Một số lỗi xảy ra trong quá trình cài
  - Phải tải phiên bản geth phù hợp trên trang chủ go-ethereum
  + Lỗi không đưa được geth ra môi trường bên ngoài
  + sudp cp /đường/dẫn/đến/thư/mục/go-ethereum/build/bin/geth /usr/bin/

