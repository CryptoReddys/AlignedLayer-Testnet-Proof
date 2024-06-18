# AlignedLayer - Testnet - Proof - Guide



![Logo](https://ibb.co/k6nqx7Q)


## Lets Get Start

```bash
sudo apt update -y
sudo apt upgrade -y
```


#### Install Curl
~~~bash
sudo apt-get install curl -y
~~~
#### Download ALignedProof
~~~bash
curl -L https://raw.githubusercontent.com/yetanotherco/aligned_layer/main/batcher/aligned/install_aligned.sh | bash
~~~
~~~bash
source /root/.bashrc
~~~
#### Download an example SP1 proof file with it's ELF file
~~~bash
curl -L https://raw.githubusercontent.com/yetanotherco/aligned_layer/main/batcher/aligned/get_proof_test_files.sh | bash
~~~
#### Sending Proof
~~~bash
rm -rf ~/aligned_verification_data/ &&
aligned submit \
--proving_system SP1 \
--proof ~/.aligned/test_files/sp1_fibonacci.proof \
--vm_program ~/.aligned/test_files/sp1_fibonacci-elf \
--aligned_verification_data_path ~/aligned_verification_data \
--conn wss://batcher.alignedlayer.com
~~~
### Click Explorer Link on ur Terminal : Check if its verified 

#### if its verified Copy the Explorer URL 

Tweet Format:

Just submitted a proof via @alignedlayer

I am now #aligned ✅

paste the Explorer URL

### Join Aligned Discord and submit ur Tweet Link

https://linktr.ee/AlignedLayer
