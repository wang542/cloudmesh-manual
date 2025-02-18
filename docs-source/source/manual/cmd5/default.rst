default
=======

.. parsed-literal::

  Usage:
      default list [--context=CONTEXT] [--format=FORMAT]
      default delete --context=CONTEXT
      default delete KEY [--context=CONTEXT]
      default KEY [--context=CONTEXT]
      default KEY=VALUE [--CONTEXT=CONTEXT]

  Arguments:
    KEY    the name of the default
    VALUE  the value to set the key to

  Options:
     --context=CONTEXT    the name of the context
     --format=FORMAT  the output format. Values include
                      table, json, csv, yaml.

  Description:
    Cloudmesh has the ability to manage easily multiple
    clouds. One of the key concepts to manage multiple clouds
    is to use defaults for the cloud, the images, flavors,
    and other values. The default command is used to manage
    such default values. These defaults are used in other commands
    if they are not overwritten by a command parameter.

    The current default values can by listed with

        default list --all

    Via the default command you can list, set, get and delete
    default values. You can list the defaults with

       default list

    A default can be set with

        default KEY=VALUE

    To look up a default value you can say

        default KEY

    A default can be deleted with

        default delete KEY

    To be specific to a cloud you can specify the name of the
    cloud with the --cloud=CLOUD option. The list command can
    print the information in various formats iv specified.

  Examples:
    default list --all
        lists all default values

    default list --cloud=kilo
        lists the defaults for the cloud with the name kilo

    default image=xyz
        sets the default image for the default cloud to xyz

    default image=abc --cloud=kilo
        sets the default image for the cloud kilo to xyz

    default image
        list the default image of the default cloud

    default image --cloud=kilo
        list the default image of the cloud kilo

    default delete image
        deletes the value for the default image in the
        default cloud

    default delete image --cloud=kilo
        deletes the value for the default image in the
        cloud kilo

Timer: 0.0000s (man default --format=rst)
