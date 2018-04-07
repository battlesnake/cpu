# Info

Tool for turning cores on/off, changing min/max speed limits, changing governors.


# TODO

 - Add `intel_pstate` support, if it offers better control than the current "cpu speed" implementation, on supported processors.


# Syntax

`cpu <command> <subcommand> [args...]`

command: core / governor / boost / speed / help

subcommand: (typically) get / set

Enabled core count:

    cpu core get
    cpu core set <count>

Governor:

    cpu governor get
    cpu governor set
    cpu governor set <name>

Boost (AMD):

    cpu boost get
    cpu boost set (enabled|disabled)

Speed:

    cpu speed get
    cpu speed set <min> <max> - may use certain SI suffixes e.g. 2700M, 3G, etc


