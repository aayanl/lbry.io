---
title: How do I use the LBRY Command Line Interface (CLI) tool?
category: setup
---

In addition to the JSON commands available in the [LBRY API Quickstart Guide](https://lbry.io/quickstart/api) as a method to interact with the LBRY protocol, there is another way through the command line tools (CLI). This will allow you to run any available commands from the [LBRY CLI documentation](https://lbryio.github.io/lbry/cli/). You must be running the LBRY app or daemon in order to interact with the protocol.

## Windows
1. Open a **Command Prompt** application window
1. Type `cd "c:\Program Files (x86)\LBRY\resources\app\dist"` and click Enter
1. Type `lbrynet-cli status` and click **Enter**. This will return the LBRYnet status data
1. See examples below or [LBRY CLI documentation](https://lbryio.github.io/lbry/cli/) for additional commands

## MacOS
1. Open a **Terminal** window
1. Type `cd /Applications/LBRY.app/Contents/Resources/app/dist`
1. Type `./lbrynet-cli status`  and click **Enter**. This will return the LBRYnet status data
1. See examples below or [LBRY CLI documentation](https://lbryio.github.io/lbry/cli/) for additional commands

## Ubuntu / Linux 
1. Open a **Terminal** window
1. Type `cd /opt/LBRY/resources/app/dist`
1. Type `./lbrynet-cli status`  and click **Enter**. This will return the LBRYnet status data
1. See examples below or [LBRY CLI documentation](https://lbryio.github.io/lbry/cli/) for additional commands

## Common/Sample Commands
- `lbrynet-cli claim list mine` - Show list of own claims, inlcluding channels
- `lbrynet-cli resolve one` - Retreive information about winning claim at lbry://one
- `lbrynet-cli claim_list one` - Retreive information about all claims at lbry://one
- `lbrynet-cli claim_abandon --claim_id=<claimid>` - Abandon claim by claim id (from claim info)
- `lbrynet-cli claim_abandon --txid=<txid> --nout=<nout>` - Abandon claim by transaction id and nout (from claim info)
