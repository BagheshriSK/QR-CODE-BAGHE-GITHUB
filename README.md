# QR-CODE-GENERATOR

pip install pyqrcode

pip install pypng

import pyqrcode #pyrcode is a module to generate QRcode

import png #pypng is a module to save image in png format

from pyqrcode import QRCode

str = "Welcome to Bagheshri's world" # String which denotes the QR code
  
url = pyqrcode.create(str) # QR code generator
  
url.svg("Bagqr.svg", scale = 8) # Create and save the svg file with the name "myqr.svg"
  
url.png('Bagqr.png', scale = 6) # Create and save the png file with the name "myqr.png"





