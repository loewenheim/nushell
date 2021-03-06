# sys

This command gives information about the system nu is running on.

## Examples

```shell
> sys
━━━━━━━━━━━━━━━━┯━━━━━━━━━━━━━━━━┯━━━━━━━━━━━━━━━━━┯━━━━━━━━━━━━━━━━┯━━━━━━━━━━━━━━━━━━┯━━━━━━━━━━━━━━━━
 host           │ cpu            │ disks           │ mem            │ net              │ battery
────────────────┼────────────────┼─────────────────┼────────────────┼──────────────────┼────────────────
 [table: 1 row] │ [table: 1 row] │ [table: 3 rows] │ [table: 1 row] │ [table: 18 rows] │ [table: 1 row]
━━━━━━━━━━━━━━━━┷━━━━━━━━━━━━━━━━┷━━━━━━━━━━━━━━━━━┷━━━━━━━━━━━━━━━━┷━━━━━━━━━━━━━━━━━━┷━━━━━━━━━━━━━━━━
> sys | get host
━━━━━━━━┯━━━━━━━━━┯━━━━━━━━━━━━━━┯━━━━━━━━┯━━━━━━━━━━━━━━━━┯━━━━━━━━━━━━━━━━━━
 name   │ release │ hostname     │ arch   │ uptime         │ sessions
────────┼─────────┼──────────────┼────────┼────────────────┼──────────────────
 Darwin │ 18.7.0  │ C02Y437GJGH6 │ x86_64 │ [table: 1 row] │ [table: 17 rows]
━━━━━━━━┷━━━━━━━━━┷━━━━━━━━━━━━━━┷━━━━━━━━┷━━━━━━━━━━━━━━━━┷━━━━━━━━━━━━━━━━━━
> sys | get cpu
━━━━━━━┯━━━━━━━━━━━━━━━━━━━┯━━━━━━━━━━━━━━━━━━━┯━━━━━━━━━━━━━━━━━━━
 cores │ current ghz       │ min ghz           │ max ghz
───────┼───────────────────┼───────────────────┼───────────────────
    12 │ 2.600000000000000 │ 2.600000000000000 │ 2.600000000000000
━━━━━━━┷━━━━━━━━━━━━━━━━━━━┷━━━━━━━━━━━━━━━━━━━┷━━━━━━━━━━━━━━━━━━━
> sys | get mem
━━━━━━━━━┯━━━━━━━━━━┯━━━━━━━━━━━━┯━━━━━━━━━━━
 total   │ free     │ swap total │ swap free
─────────┼──────────┼────────────┼───────────
 34.4 GB │ 545.0 MB │     2.1 GB │  723.0 MB
━━━━━━━━━┷━━━━━━━━━━┷━━━━━━━━━━━━┷━━━━━━━━━━━
```
