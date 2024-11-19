git clone https://github.com/burnt-labs/xion.git
git clone https://github.com/burnt-labs/xion.git -b vX.Y.Z
# install xiond
make install
xiond version

#output e.g.
9.0.0
docker compose up testnet
# Run the following command
xiond
# Outputs xiond information
xion daemon (server)

Usage:
  xiond [command]

Available Commands:
  completion  Generate the autocompletion script for the specified shell
  config      Create or query an application CLI configuration file
  debug       Tool for helping with debugging your application
  export      Export state to JSON
  genesis     Application's genesis-related subcommands
  help        Help about any command
  init        Initialize private validator, p2p, genesis, and application configuration files
  keys        Manage your application's keys
  prune       Prune app history states by keeping the recent heights and deleting old heights
  query       Querying subcommands
  rollback    rollback cosmos-sdk and tendermint state by one height
  rosetta     spin up a rosetta server
  snapshots   Manage local snapshots
  start       Run the full node
  status      Query remote node for status
  tendermint  Tendermint subcommands
  tx          Transactions subcommands
  version     Print the application binary version information

Flags:
  -h, --help                help for xiond
      --home string         directory for config and data (default "/Users/admin/.xiond")
      --log_format string   The logging format (json|plain) (default "plain")
      --log_level string    The logging level (trace|debug|info|warn|error|fatal|panic) (default "info")
      --log_no_color        Disable colored logs
      --trace               print out full stack trace on errors

Use "xiond [command] --help" for more information about a command.
xiond keys add <alias>
> xiond keys add mywallet

- address: xion1l3r75pkwlg2fmasn9lk8umda0pjnjy7cq0x9gz
  name: mywallet
  pubkey: '{"@type":"/cosmos.crypto.secp256k1.PubKey","key":"A20kOEVZuZxVGdQiFExGsO7fO+4B+QbTRJYhvaRSMkWy"}'
  type: local

**Important** write this mnemonic phrase in a safe place.
It is the only way to recover your account if you ever forget your password.

trend express cheap ... room upset hair
> xiond keys show mywallet

- address: xion1l3r75pkwlg2fmasn9lk8umda0pjnjy7cq0x9gz
  name: mywallet
  pubkey: '{"@type":"/cosmos.crypto.secp256k1.PubKey","key":"A20kOEVZuZxVGdQiFExGsO7fO+4B+QbTRJYhvaRSMkWy"}'
  type: local
