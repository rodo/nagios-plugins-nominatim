nagios-plugins-nominatim
========================

Nagios plugins for Nominatim

* check_nominatim

Usage : check_nominatim!PORT!QUERYSTRING

Sample :

    define service {
        host_name                       nominatim.quiedeville.org
        service_description             nominatim
        check_command                   check_nominatim!80!vannes
        use                             generic-service
        notification_interval           0
    }

