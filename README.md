# review-images

Images that can be used in apps as reviews or ratings.

Example Python code to get image:

```Python
import requests
from PIL import Image
from io import BytesIO

rating = 5
image_url = "https://raw.githubusercontent.com/SamuelHarner/review-images/main/images/" + str(rating) + "_stars.png"

response = requests.get(image_url)
image = Image.open(BytesIO(response.content))
```
