.. The contents of this file may be included in multiple topics (using the includes directive).
.. The contents of this file should be modified in a way that preserves its ability to appear in multiple topics.

The ``GET`` method is used to return the names of all recipes in the most recent cookbook versions.

This method has no parameters.

**Request**

.. code-block:: none

   GET /organizations/NAME/cookbooks/_recipes

**Response**

The response is similar to:

.. code-block:: javascript

   {
   
   }

**Response Codes**

.. list-table::
   :widths: 200 300
   :header-rows: 1

   * - Response Code
     - Description
   * - ``200``
     - OK. The request was successful.
   * - ``401``
     - Unauthorized. The user or client who made the request could not be authenticated. Verify the user/client name, and that the correct key was used to sign the request.
   * - ``403``
     - Forbidden. The user who made the request is not authorized to perform the action.
   * - ``404``
     - Not found. The requested object does not exist.
