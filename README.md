# NAME

SOAP::WSDL::Server::Dancer2 - Dancer2 for SOAP::WSDL Server

# SYNOPSIS

    use Dancer2;
    use SOAP::WSDL::Server::Dancer2;

    post '/payment_validation' => sub {
        soap_wsdl_server(
            dispatch_to => 'HelloWorld::Impl',
            soap_service => 'HelloWorld::Server::XXX::XXXServicePort',
        );
    };

# DESCRIPTION

A module copied from [SOAP::WSDL::Server::Plack](https://metacpan.org/pod/SOAP::WSDL::Server::Plack) but for Dancer2

# AUTHOR

Fayland Lam <fayland@gmail.com>

# COPYRIGHT

Copyright 2016- Fayland Lam

# LICENSE

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.

# SEE ALSO

[SOAP::WSDL::Server::Plack](https://metacpan.org/pod/SOAP::WSDL::Server::Plack), [SOAP::WSDL](https://metacpan.org/pod/SOAP::WSDL)
