# 🧮 4-bit Binary Multiplier – Custom Digital Design using Cadence Virtuoso

This project demonstrates the full-custom VLSI design flow of a 4-bit binary multiplier using Cadence Virtuoso and Spectre simulator. The design is implemented from schematic to post-layout simulation using industry-grade tools.

---

## 📌 Tools Used

- **Cadence Virtuoso** – Schematic, Symbol, Layout, DRC, LVS
- **Spectre / ADEL** – Functional and post-layout simulation
- **Assura / Calibre** – DRC and LVS checks
- **Calculator Tool** – For delay estimation

---

## 🚀 Project Flow

1. **Schematic Design**
   - Created a 4-bit multiplier schematic using Boolean equation converting it 	schematic using NMOS and PMOS connecting in parallel and series.

2. **Symbol Generation**
   - Generated a reusable symbol in Virtuoso attaching the input port upward and 	output port downwards.

3. **Functional Simulation (Pre-layout)**
   - Verified correct multiplication operation using Spectre.

4. **Layout Design**
   - Designed full custom layout and custom routing using Euler's rule and make it 	size compact as it could.

5. **DRC & LVS**
   - Verified design rule compliance and schematic-layout equivalence.

6. **PEX (Parasitic Extraction)**
   - Extracted parasitic netlist  the precapicitor and preresistor developed after 	layout in physical design using Assura PEX.

7. **Post-Layout Simulation**
   - Simulated extracted netlist using Spectre for accurate timing and compare the 	layout vs schematic simulation.

8. **Delay Estimation**
   - Calculated propagation delay from waveform analysis.

---

## 📷 Snapshots

- ✅ Schematic and Symbol  
- ✅ Layout View  
- ✅ DRC / LVS Passed Screenshots  
- ✅ Simulation Results (Pre & Post Layout)  
- ✅ Delay Calculation Screenshot

---

## 📈 Performance Summary

| Parameter                 | Value             |
|---------------------------|-------------------|
| Technology Node           | 45 nm	        |
| Delay (Post-Layout)       | 20 ns             |
| mosfet Used               | 600               |
| layout Design             | Custom            |
| Parasitics Considered     | Yes (via PEX)     |

---

## 📁 Repository Structure

- `schematic/` – Schematic and symbol images  
- `layout/` – Layout view and PEX files  
- `simulation/` – Simulation waveforms  
- `parasitic extraction/` – Extracted netlist and results  
- `doc/` – Full project report and calculations  
- `results/` – Summary and delay analysis

---

## 🎯 Future Scope

- Extend to an 8-bit or 16-bit multiplier
- Use synthesis + place & route flow for ASIC tape-out
- Integrate into an ALU design
- Compare with Booth’s multiplier or Wallace Tree structure

---

## 📜 License

MIT License (you can change it as needed)
