# zookeeper_setup

- created the hashed password for zookeeper with:
  python3 -c 'import crypt; print(crypt.crypt("here_stands_the_passord", crypt.mksalt(crypt.METHOD_SHA512)))'

- used the vault feature to encrypt (analog for decrypt) the vars-file with the hashed passwords:
  ansible-vault encrypt roles/users/vars/main.yml

