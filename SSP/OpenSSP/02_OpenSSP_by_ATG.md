# OpenSSP by ATG
* <http://openssp.org/>

* open-source supply-side platform for general use with full OpenRTB support.


* OpenSSP
  - so-called multi-channel SSP
    - which mean
      - support RTB,
      - channel to ad server,
      - further SSP implementaton.
  - support the OpenRTB standard
    - can be deliver
      - banner impressions
      - videoad impressions etc.
    - Feel free to examine the code and modify it as you need.


* General SSP Functionality:
  - A tag with a link to OpenSSP needs to
    - be placed on a website that contains the ad placement.
  - OpenSSP is called from the tag and the parameters are extracted and validated.
  - OpenSSP resovles the request data,
    - e.g. the website or publisher which is identified by an ID
    - and loads additional data from cache (more information on data caching)
  - OpenSSP starts the ExchangeServer and the ExecutorService to call a demand service
    (DSP, SSP, Adserver etc.) and waits for the response to start the auction.
  - After the auction is finished, the winner is evaluated and a response to the client will be sent.







