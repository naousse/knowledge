Module's migration
------------------

Operations

Creation of folders models, views, data and demo
document_page_view.xml moved to views and renamed to document_page
document_page_data.xml moved to data and renamed to document_page
document_page_demo.xml moved to demo and renamed to document_page
document_page.py moved to models and renamed to document_page

Module models initialise by the creation of the file __init__.py

wizard file reorganized
folder wizard created
document_page_create_menu.py and document_page_create_show_diff.py moved to wizard
document_page_create_menu_view.xml moved to document_page_create_menu.xml
document_page_create_show_diff_view.xml en document_page_create_show_diff.xml


__openerp_.py et __init__.py file edited in order to reflect the module organization

While the module knowledge is no more necessary the following menu was created
as based menu for future Operation's menu

<menuitem name="Knowledge"
          id="base.menu_document"  groups="base.group_system,base.group_document_user"
           sequence="116"/>

       <menuitem name="Configuration" id="base.menu_document_configuration"
           parent="base.menu_document" sequence="50"/>

       <menuitem name="Collaborative Content" id="base.menu_document2"
          parent="base.menu_document"/>
