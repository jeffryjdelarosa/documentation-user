==========
Use Routes
==========

A route is a collection of :doc:`push and pull rules <pull_push_rules>`. In Odoo, you can manage
advanced push/pull routes configuration, like:

-  Manage product manufacturing chains; 
-  Manage default locations per product; 
-  Define routes within your warehouse according to business needs, such as quality control, after-sales services or supplier returns; 
-  Help rental management, by generating automated return move for rented products. 

.. note::
      - You can find documentation about those subjects `here <https://www.odoo.com/documentation/user/13.0/inventory.html>`__

Configuration
=============

To configure routes, open the *Inventory* application. Then, go to
:menuselection:`Configuration --> Settings` and enable the *Multi-Step Routes*
feature.

.. note::
         Doing so, the *Storage Locations* feature will also be activated.

.. image:: media/use_routes_01.png
   :align: center

Pre-Configured Routes
=====================

Of course, Odoo has some pre-configured routes for your warehouses. To
see them, open the *Warehouses* menu, under *Configuration*.

In the *Warehouse Configuration* tab, some routes are automatically
created based on your choices for *Incoming Shipments* and *Outgoing
Shipments*.

.. image:: media/use_routes_02.png
   :align: center

Custom Routes
=============

In the *Inventory* application, open :menuselection:`Configuration --> Routes`. Then,
you have to select the places where this route can be selected. You can
combine several choices if needed.

Routes applied on warehouses
----------------------------

If you tick *Warehouses*, you have to choose on which warehouse it
will be applied. The route will be set for all transfers in that
warehouse that would meet the conditions of the pull and push rules.

.. image:: media/use_routes_03.png
   :align: center

Routes applied to products
--------------------------

If you choose *Products*, you have to manually set on which product it
will be applied.

.. image:: media/use_routes_04.png
   :align: center

To do so, open the product on which you want to apply the routes. Open
the *Inventory tab* and select the route you’ve created.

.. image:: media/use_routes_05.png
   :align: center

Routes applied on Product Category
----------------------------------

Then, you can also choose to apply routes to *product categories*.
Just like you did for products, you will have to manually set on which
categories it will be applied.

.. image:: media/use_routes_06.png
   :align: center

To do so, open the product category you want to apply the route to.
Then, select the route under the *Logistic* section.

.. image:: media/use_routes_07.png
   :align: center

Routes applied on Sales Order Lines
-----------------------------------

You can also apply routes on sales order lines. For that, tick *Sales
Order Lines* on your route form.

.. image:: media/use_routes_08.png
   :align: center

Next, open a sale order. You can now add the *Route* in the view. Once
done, you can choose the routes for each of your sales orders’ lines.

.. image:: media/use_routes_09.png
   :align: center

.. image:: media/use_routes_10.png
   :align: center

Pull and Push Rules
-------------------

.. seealso::
      - :doc:`pull_push_rules`

Pull Configuration
------------------

When doing a procurement request, you can force the route you want to
use. On the product, click on *Replenish*. Then, choose the route you
want to use.

.. image:: media/use_routes_11.png
   :align: center

.. image:: media/use_routes_12.png
   :align: center

Replenish on Order (MTO) Route
------------------------------

If you work without stock, it is better to use the *Replenish on Order
(MTO)* route. Combined with the *Buy* or *Manufacturing* routes, it
will automatically trigger the purchase order or manufacturing order
when your products are out-of-stock.