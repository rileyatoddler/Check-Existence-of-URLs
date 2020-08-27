#%%
from urllib.request import urlopen
from urllib.error import URLError

def checkWebsiteExists2(url):
    try:
        r = urlopen(url)
    except URLError as e:
        r = e
    if r.code in (200, 401):
        print (url)
    elif r.code == 404:
        print ('not found')
       
for i in range (0, 10):
    website = 'https://www.example.com/%s'%(i)    
    checkWebsiteExists2(website)
