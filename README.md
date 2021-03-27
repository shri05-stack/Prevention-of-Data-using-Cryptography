# Prevention-of-Data-using-Cryptography
Cryptography is a method of encryption and decryption so by encrypt and decrypt we perform data prevention. 
Prerequisites
You need to have Python2 on your system. Follow instructions at https://www.python.org/downloads/
You also need to install numpy and Image libraries.

On Ubuntu

sudo apt-get install python-numpy
sudo apt-get install python-imaging

Running
1.To encrypt an image, first place that image in the input/ folder

2.Then run
python encrypt.py <image_name>
The encrypted image can be found at the encrypted_images/ folder.
The keys generated during encryption is stored in the keys.txt file.
(Note: The number of iterations of encryption to be performed can be adjusted by changing the ITER_MAX value in the encrypt.py file. Larger values will make encryption more secure but it is more time consuming)

3.To decrypt the image, run
python decrypt.py <image_name>
And Then enter the value of the Keys (Kr, Kc and ITER_MAX)
The decrypted image can be found at the decrypted_images/ folder.

EXAMPLE -
1. To encrypt the image technology-trends.jpg stored in the input folder
![technology-trends](https://user-images.githubusercontent.com/64158567/112716192-e3d89900-8f0a-11eb-8482-08870ab9640b.jpg)
Run python encrypt.py technology-trends.jpg

The encrypted Picture can be found at encrypted_images/technology-trends.jpg
![pic3](https://user-images.githubusercontent.com/64158567/112716335-bcce9700-8f0b-11eb-81cc-114744fc9f4b.png)
The keys are stored in keys.txt

2. To decrypt the image 
Run python decrypt.py technology-trends.jpg
and enter key values (Kr,Kc and ITER_MAX)

The decrypted Pictures can be found at decrypted_images/technology-trends.jpg
![technology-trends](https://user-images.githubusercontent.com/64158567/112717419-93fdd000-8f12-11eb-9216-beff63fa91d8.jpg)
