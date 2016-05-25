# NAME 

WebService::UrbanAirship - routines for Urban Airship APIs

# SYNOPSIS

    # create the object
    my $o = WebService::UrbanAirship::APNS->new(application_key         => 'C9mvZ******************8QGW',
                                                application_secret      => 'DQvNtylF***************MgVG',
                                                application_push_secret => 'HGrBg37****************ylFA');

    # now do something, like register the device
    my $o->register_device(device_token => 'FE66489F304DC75B8D6E8200DFF8A456E8DAEACEC428B427E9518741C92C6660',
                           alias        => 'de039f61e64d3300aa0ce521fd6a65f780cc814e',

# DESCRIPTION

WebService::UrbanAirship is a base class for accessing the
Urban Airship API, as described in http://urbanairship.com/docs/

currently, the only useful class is WebService::UrbanAirship::APNS,
which serves as an API for the Apple Push Notification service
for the iPhone.  additional classes may come as Urban Airship
offers support for the Apple Store Kit and other APIs in the future.

# DEBUGGING

if you are interested in verbose error messages when something 
doesn't go according to plan you can enable debugging as follows:

    use WebService::UrbanAirship;
    $WebService::UrbanAirship::DEBUG = 1;

# SEE ALSO

http://urbanairship.com/docs/

WebService::UrbanAirship::APNS

# AUTHOR

Geoffrey Young <geoff@modperlcookbook.org>

http://www.modperlcookbook.org/

# COPYRIGHT

Copyright (c) 2009, Geoffrey Young
All rights reserved.

This module is free software.  It may be used, redistributed
and/or modified under the same terms as Perl itself.
