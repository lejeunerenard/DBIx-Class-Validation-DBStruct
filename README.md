# NAME

DBIx::Class::Validation::Structure - DBIx::Class Validation based on the column meta data

# SYNOPSIS

    package MyApp::Schema::Result::Artist;
    use base qw/DBIx::Class::Core/;

    __PACKAGE__->table('artist');
    __PACKAGE__->add_columns(qw/ artistid name /);
    __PACKAGE__->set_primary_key('artistid');
    __PACKAGE__->has_many(cds => 'MyApp::Schema::Result::CD');



# DESCRIPTION

DBIx::Class::Validation::Structure is DBIx::Class Validation based on the column meta data set in add\_columns or add\_column.

# AUTHOR

Sean Zellmer <sean@lejeunerenard.com>

# COPYRIGHT

Copyright 2013- Sean Zellmer

# LICENSE

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.

# SEE ALSO
