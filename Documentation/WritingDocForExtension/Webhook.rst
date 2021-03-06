.. include:: ../Includes.txt

.. _webhook:

=======
Webhook
=======

This section describes how to add webhooks for auto rendering to an repository.

.. _webhook-github:

GitHub
======

Add auto rendering for an Repository via GitHub webhook in five steps:

.. rst-class:: bignums-xxl

#. Go to "Settings" tab within the repository

   .. figure:: /images/webhook/github/repository-start.png
      :width: 932

#. Go to "Webhooks" section within the repository settings

   .. figure:: /images/webhook/github/settings-tab.png
      :width: 932

#. Add webhook

   .. figure:: /images/webhook/github/webhook-section.png
      :width: 932

#. Fill in webhook configuration

   #. Configure URL ``https://docs-hook.typo3.org`` for field "Payload URL".

   #. Select ``application/json`` as "Content type".

   #. Enable "SSL verification".

   #. Select ``Just the push event.`` for "Which events would you like to trigger this webhook?".

   #. Enable "Activate".

   #. Click on "Add webhook"

   .. figure:: /images/webhook/github/webhook-add.png
      :width: 932

#. Webhook was added

   GitHub should show an notice that creation of Webhook was successful.

   .. figure:: /images/webhook/github/webhook-added.png
      :width: 932

#. (Optional) visit intercept and check request

   If curious, visit https://intercept.typo3.com/admin/docs/deployments and
   check "Recent actions" (scroll down). The repository should have created an
   "Docs hook ping from github repository".

   .. figure:: /images/webhook/github/intercept-feedback.png
      :width: 932
