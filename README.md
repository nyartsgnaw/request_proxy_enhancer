## requests.get Proxy Enhancer
### copyright: Strayn Wang

#### Usage:  
- Copy "```./utils/proxies/```" and "```./utils/proxy_utils.py```" to the code directory.


- Initialize the environment, use download_page to replace "request.get" (```proxies``` directory will generate under same directory of ```proxy_utils.py```,if there isn't ).

```
from proxy_utils import initializer
download_page = initializer(timeout_duration=5,test_url='http://www.lrcgc.com/artist-11.html') 
```

#### Debug  
- Delete proxies file to reset generating environment. Run code to initialize environment, which creates a file called ```./utils/proxies/proxies_good```.
All proxies in that file will be used to secure the code, you can add them manually.  

```
python ./utils/proxy_utils.py  
```