.. The contents of this file may be included in multiple topics (using the includes directive).
.. The contents of this file should be modified in a way that preserves its ability to appear in multiple topics.

The ``DELETE`` method is used to delete an environment.

This method has no parameters.

**Request**

.. code-block:: none

   DELETE /organizations/NAME/environments/NAME

**Response**

The response will return the JSON for the environment that was deleted, similar to:

.. code-block:: javascript

   {
     "name":"backend",
     "description":"",
     "cookbook_versions":{},
     "json_class":"Chef::Environment",
     "chef_type":"environment",
     "default_attributes":{},
     "override_attributes":{}
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
