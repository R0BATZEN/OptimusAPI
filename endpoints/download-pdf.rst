Download PDF
==================
This API endpoint allows for the retrieval and download of benchmark content in the PDF format.

.. list-table::
	:header-rows: 1

	* - Request Type
	  - Visibility
	* - GET
	  - SecureSuite Members Only

Base URL
--------

::

	https://workbench.cisecurity.org/api/vendor/v1

Endpoint
--------

::

	/pdf/{workbenchId}

Request Payload/Parameters
--------------------------
In order to provide download authorization, members must first authenticate their license key using the :code:`/license` endpoint.  The response from that endpoint is an authorization token.


Request Headers
^^^^^^^^^^^^^^^
.. list-table::
	:header-rows: 1

	* - Header Name
	  - Description
	* - X-SecureSuite-Token
	  - The token received from a successful license key verification, e.g., :code:`1234|7b68c544113bc4notvalid358ffd4ba7f254e39c4a842cefed748`

URL Parameters
^^^^^^^^^^^^^^
.. list-table::
	:header-rows: 1

	* - URL Parameter
	  - Description
	* - workbenchId
	  - The unique identifier for a specific PDF as stored in CIS WorkBench.

Response Payload
----------------


Media Type
^^^^^^^^^^

::

	.pdf


Description/Fields
^^^^^^^^^^^^^^^^^^
The response payload will contain a PDF (.pdf) download.

Response Example
^^^^^^^^^^^^^^^^
None



.. history
.. authors
.. license
