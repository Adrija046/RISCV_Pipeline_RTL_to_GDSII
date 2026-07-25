# Clock Tree Synthesis (CTS) Stage

## Specifications

| Parameter | Value |
|---|---|
| Clock Net | clk |
| Total Sinks | 1,844 |
| Sinks After Clustering | 134 |
| Clock Buffers Inserted | 159 |
| Buffer Cell Used | sky130_fd_sc_hd__clkbuf_8 |
| Clock Buffer Levels (min/max) | 4 / 4 (balanced) |
| Average Sink Wire Length | 1994.78 μm |
| Worst Setup Slack | 2.74 ns (MET) |
| Worst Hold Slack | 0.00 ns (MET) |

## Description
Clock Tree Synthesis balances clock distribution to all 1,844 sequential element sinks by
inserting 159 buffer cells across a uniform 4-level buffer tree, minimizing clock skew.
Post-CTS static timing analysis confirms all setup and hold timing checks are met, with
2.74 ns of positive setup slack margin.

## Logs
See `logs/` for detailed CTS synthesis and post-CTS STA logs.

## Artifacts
See `def/` for the CTS-stage DEF file.
