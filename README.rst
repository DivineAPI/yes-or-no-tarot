
#################################
Yes Or No Tarot - DivineAPI
#################################
Start your FREE Trial to get your API KEY,  `https://divineapi.com <https://divineapi.com>`_

|travis| |Docs| |Maintenance yes| |SayThanks| |Paypal|
    
    
.. image:: https://divineapi.com/assets/images/logo.svg
   :height: 412px
   :width: 898px
   :alt: divineapi logo
   :align: center
   

What is Yes Or No Tarot API?
==============
Divine API allows developers to access and gives them opportunity to integrate astrology
services to their website or application &amp; providing them with services like Daily Horoscope,
Yes or No Tarot API, Daily Tarot, Fortune Cookie &amp; Coffee Cup Reading.

..
  Feel free to contribute on `Github <http://github.com/divineapi/horoscope-api>`_.




Why Yes Or No Tarot API?
==========
Divine API has so much to offer. One of the features of divine API is the yes or no Tarot API.
Developers can add the yes or no tarot for their application users to decide on something
just with a flip of card.



Features
==========

- The cards created by the Yes or No Tarot API are advanced in appearance with the touch of traditional design.
- It provides yes or no response with rational description.
- The responses are on point and authentic.
- The user interface is extremely attractive.
- There are a large number of pre-designed cards for everyone.


Benefits
==========

- It helps your customer get past the question they have been holding on for a while.
- With Yes or No Tarot API, you can choose to take the tough decision with calculated risk.
- It has no bugs and is contains engaging content.


URL
===
.. code-block:: python

    POST: https://divineapi.com/api/1.0/get_yes_or_no_tarot.php


Parameters
==========

api_key : 
   Your API  KEY.
 


Result Example:
=====
.. code-block:: text


      {
          "success": 1,
          "message": "Yes or No Tarot result.",
          "data": {
              "prediction": {
                  "card": "Card1",
                  "category": "upright",
                  "yes_no": "yes",
                  "result": "Result1",
                  "image": "image_url"
              }
          }
      } 
      


Example 
=======


cURL
^^^^
.. code-block:: curl

    curl -d "api_key=YOUR_API_KEY" -X POST https://divineapi.com/api/1.0/get_yes_or_no_tarot.php


Python
^^^^^^
.. code-block:: python

   import requests
   from requests.structures import CaseInsensitiveDict

   url = "https://divineapi.com/api/1.0/get_yes_or_no_tarot.php"

   headers = CaseInsensitiveDict()
   headers["Content-Type"] = "application/x-www-form-urlencoded"

   data = "api_key=YOUR_API_KEY"


   resp = requests.post(url, headers=headers, data=data)

   print(resp.status_code)


Javascript
^^^^^^^
.. code-block:: javascript

   var url = "https://divineapi.com/api/1.0/get_yes_or_no_tarot.php";

   var xhr = new XMLHttpRequest();
   xhr.open("POST", url);

   xhr.setRequestHeader("Content-Type", "application/x-www-form-urlencoded");

   xhr.onreadystatechange = function () {
      if (xhr.readyState === 4) {
         console.log(xhr.status);
         console.log(xhr.responseText);
      }};

   var data = "api_key=YOUR_API_KEY";

   xhr.send(data);


PHP
^^^
.. code-block:: php

   <?php
    $url = "https://divineapi.com/api/1.0/get_yes_or_no_tarot.php";

    $curl = curl_init($url);
    curl_setopt($curl, CURLOPT_URL, $url);
    curl_setopt($curl, CURLOPT_POST, true);
    curl_setopt($curl, CURLOPT_RETURNTRANSFER, true);

    $headers = array(
       "Content-Type: application/x-www-form-urlencoded",
    );
    curl_setopt($curl, CURLOPT_HTTPHEADER, $headers);

    $data = "api_key=YOUR_API_KEY";

    curl_setopt($curl, CURLOPT_POSTFIELDS, $data);

    $resp = curl_exec($curl);
    curl_close($curl);
    var_dump($resp);
   ?>
    
    
jQuery Ajax
^^^^^^
.. code-block:: javascript

    $.ajax({
   type:'POST',
   url:'https://divineapi.com/api/1.0/get_yes_or_no_tarot.php',
   data: {api_key:'YOUR_API_KEY'},
   success:function(data){
   console.log(data);
   }
    });


ECMAScript (ES6)
^^^^^^
.. code-block:: javascript

    const URL = 'https://divineapi.com/api/1.0/get_yes_or_no_tarot.php?api_key=YOUR_API_KEY';
    fetch(URL, {
        method: 'POST'
    })
    .then(response => response.json())
    .then(json => {
        const date = json.current_date;
        console.log(date);
    });


License
=======

2021 Divine API

Licensed under the Apache License, Version 2.0 (the "License");

    http://www.apache.org/licenses/LICENSE-2.0



Contact
=======

Questions? Suggestions? Feel free to contact me at admin@divineapi.com


Credits
=======

"DivineAPI" was created by `Azhar <https://azhar-spiderdev.github.io/portfolio>`_

Source of updates - https://divineapi.com/yes-no-tarot-api

Please feel free to use and adapt this awesome API.

    
.. |Docs| image:: https://readthedocs.org/projects/aztro/badge/?version=latest
    :target: https://azhar-spiderdev.github.io/
    
.. |Maintenance yes| image:: https://img.shields.io/badge/Maintained%3F-yes-green.svg
   :target: https://azhar-spiderdev.github.io/


.. |Travis| image:: https://travis-ci.org/sameerkumar18/aztro.svg?branch=master
    :target: https://azhar-spiderdev.github.io/

.. |SayThanks| image:: https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg
    :target: https://azhar-spiderdev.github.io/

.. |Paypal| image:: https://img.shields.io/badge/Paypal-Donate-blue.svg
    :target: https://azhar-spiderdev.github.io/

.. Indices and tables
.. ==================

.. * :ref:`genindex`
.. * :ref:`modindex`
.. * :ref:`search`
