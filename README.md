## How to use

1. Checkout the repository.
2. Build the image and the corresponding Compose service using 
   `docker-compose build` inside the checked out directory.
3. Open the directory as the project in PyCharm and add Docker Compose Python
   interpreter based on *docker-compose.yml* and *app* service inside it.
   Use *python3* as *Python interpreter path*:
   ![](Add%20Python%20Interpreter.png)
4. After finishing adding Python interpreter there are number of the skeleton 
   generation problems in *idea.log*:
   ```
   ...
   2020-05-17 18:19:06,820 [350842414]   INFO - .skeletons.PySkeletonGenerator - Sources and skeletons are loaded in 41277 millis. 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Some skeletons failed to generate 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._AES 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._ARC2 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._ARC4 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._Blowfish 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._CAST 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._DES 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._DES3 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._Salsa20 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._XOR 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._chacha20 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._raw_aes 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._raw_aesni 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._raw_arc2 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._raw_blowfish 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._raw_cast 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._raw_cbc 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._raw_cfb 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._raw_ctr 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._raw_des 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._raw_des3 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._raw_ecb 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._raw_eksblowfish 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._raw_ocb 
   2020-05-17 18:19:06,839 [350842433]   WARN - .skeletons.PySkeletonRefresher - Crypto.Cipher._raw_ofb 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.Hash._BLAKE2b 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.Hash._BLAKE2s 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.Hash._MD2 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.Hash._MD4 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.Hash._MD5 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.Hash._RIPEMD160 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.Hash._SHA1 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.Hash._SHA224 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.Hash._SHA256 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.Hash._SHA384 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.Hash._SHA512 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.Hash._ghash_clmul 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.Hash._ghash_portable 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.Hash._keccak 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.Hash._poly1305 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.Math._modexp 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.Protocol._scrypt 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.PublicKey._ec_ws 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.PublicKey._fastmath 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.Util._counter 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.Util._cpuid_c 
   2020-05-17 18:19:06,840 [350842434]   WARN - .skeletons.PySkeletonRefresher - Crypto.Util._strxor    
   ...
   ```
