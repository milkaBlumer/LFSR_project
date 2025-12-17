🎯 Mini UVM Project – LFSR Verification
This project is a compact UVM verification environment for an LFSR (Linear Feedback Shift Register) block.
It demonstrates the main concepts of UVM in a small, educational setup.

🗂 **Project Structure**
🔹 LFSR_agent.sv       # Combines driver, monitor, and sequencer into a single agent
🔹 LFSR_design.sv      # DUT (LFSR design)
🔹 LFSR_driver.sv      # Sends transactions to DUT based on sequence items
🔹 LFSR_env.sv         # Environment
🔹 LFSR_if.sv          # Interface
🔹 LFSR_monitor.sv     # Observes DUT outputs and forwards to scoreboard
🔹 LFSR_pkg.sv         # Package includes & macros
🔹 LFSR_scoreboard.sv  # Compares expected vs actual
🔹 LFSR_seq_item.sv    # Transactions
🔹 LFSR_seq_lib.sv     # Sequence Items Library
🔹 LFSR_sequence.sv    # Driving sequence
🔹 LFSR_sequencer.sv   # Driving sequencer
🔹 LFSR_test.sv        # Test instance
🔹 testbench.sv        # Top-level testbench

⚡ **Features**

✅ Transaction-level verification (sequence items)

✅ Agent with driver, monitor, sequencer

✅ Scoreboard validates expected vs actual outputs

✅ Supports multiple polynomials & seed values

✅ Waveform dump (dump.vcd) for easy inspection

🚀 How to Run

Compile all files with your simulator:

vlog *.sv


**Run the test:**

vsim -c -do "run -all; quit" LFSR_tb


**View waveform:**

gtkwave dump.vcd

🧠 **Notes**

Designed for learning & demonstration

Minimal, clear UVM architecture

Easy to extend for more complex tests
