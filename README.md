mojolicious-plugin-dbicadmin
============================

DBIx::Class admin plugin of mojolicious

Install 
----------
- from CPAN

     cpanm Mojolicious::Plugin::DBICAdmin

- from tarball

    #download the source use git or wget
    cd mojolicious-plugin-dbicadmin && cpanm .

Configure
----------
In Mojolicious App's ``startup`` method:

    $self->plugin('DBICAdmin' =>   {
                condition => 'login', # optional
                stylesheet => '/dbic-admin-pure.css', #optional
                # ... other configurations
    });

Use
---------
start app and view the URI :
>http://yourapp.domain/admin/dbic/

