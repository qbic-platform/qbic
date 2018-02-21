### Seeds ###

Utility to generate the seeds.txt list that is compiled into the client
(see [src/chainparamsseeds.h](/src/chainparamsseeds.h) and other utilities in [contrib/seeds](/contrib/seeds)).

The seeds compiled into the release are created from sipa's DNS seed data, like this:

    qbic-cli masternodelist full ENABLED | awk '{printf ("%s\t%s\n", $10, $7)|"sort -t',' -gk2"}' | cut -d\" -f 1 | tail -n 30 > nodes_main.txt
    python generate-seeds.py .
