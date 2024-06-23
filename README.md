
!pip install pyqrcode
!pip install pypng

import pyqrcode  # pyqrcode is a module to generate QR codes
import png  # pypng is a module to save images in png format
from pyqrcode import QRCode
from IPython.display import Image

# URL of your GitHub profile
github_url = "https://github.com/BagheshriSK?tab=repositories"

# Generate the QR code
url = pyqrcode.create(github_url)

# Create and save the SVG file with the name "github_profile.svg"
url.svg("github_profile.svg", scale=8)

# Create and save the PNG file with the name "github_profile.png"
url.png('github_profile.png', scale=6)

# Display the PNG file within the notebook
display(Image(filename='github_profile.png'))

print("QR code generated and saved as github_profile.svg and github_profile.png")






