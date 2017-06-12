Changelog
=========

v4.0.0
------

* Replaced ``payer`` with ``extra_fields``, which allow sending a lot more
  custom data to MercadoPago when creating preferences.

v3.0.0
------

* Allow sending ``payer`` and ``description`` when creating preferences.
* Replaced ``MERCADOPAGO_ASYNC`` with the opposite ``MERCADOPAGO_AUTOPROCESS``
  setting, since asynchronous processing will never be built in (only the
  necessary helpers)
* Fire a signal when a notification is received. The docs mention how to listen
  to it, which you might want to do if you'd like to do asynchronous
  processing.
* Add a management command to poll unpaid preferences.
* Introduced this changelog.