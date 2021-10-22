| Check Item                               | Answer                   | Example Ans |
| - | - | - |
| Project / Die ID                         | Project Genesis          | ChipTop |
| Revision Type                            | Full                     | Metal/FULL Layer Revision |
| Place & Route Style                      | Full chip                | Block / Chiptop |
| Package Scheme                           | Wirebond                 | Wirebond / Flip chip |
| Place & Route Type ? Flat/Hierarchical   | Hier                     | Flat |

## Design Files                                                                                                              
| Check Item                                                           | Answer                                 | Example Ans |
| - | - | - |
| Cavity / Floorplan format                                            | 1.8mm x 2.1mm \--> 2mm x 3mm           | DEF ; design.def or Size |
| Does the Design use Low Power Intent file?<br>If so, need CPF/UPF    | KC to confirm                          | Yes; path : |
| Is the netlist hierarchical?                                         | Yes                                    |  |
| Is the netlist unique?                                               | KC to confirm                          | |
| ECO Netlist                                                          | No                                     | |
| Is no-load setup clean?                                              |                                        | Yes |
| Are there any assign statement in netlist?                           |                                        | No |
| Are there any wand statements in netlist?                            |                                        | No |
| Design constraint file                                               |                                        | scan.sdc, func.sdc|
| Any CTS spec file provided ?                                         | No --> Handled by OpenFPGA methodology | No |

## Technology
| Check Item                                  | Answer              | Example Ans |
| - | - | - |
| Foundry                                     | TSMC                | TSMC        |
| Process Node                                | ULP 22              | 40nm        |
| Design Kit Version                          | CLN22US41001-22 nm  | xxxx        |
| Tech Files                                  | /home/users/pdks/tech\_files/PRTF\_ICC2\_22nm\_001\_Syn\_V11\_1a/PR\_tech/Synopsys/TechFile/VHV/PRTF\_ICC2\_22nm\_7M\_5X1ZRDL\_9T.11\_1a.tf |             |
| TLU+ files                                  | /home/users/pdks/tlu+\_files/tlu+files  |             |
| Metal Scheme                                | 7M\_5X1ZRDL\_9T, VHV                    | 12M6X2Y2R2Z |
| Rule Decks<br>1\. DRC<br>2\. LVS<br>3\. ARC |                                         |             |

## Models   
| Check Item                                                       | Answer                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | Example Ans |
| - | - | - |
| List the Hard Macros and Custom Blocks used inside the PnR block |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | ROM, OTP                                                  |
| List the Hard Macros - Library Path & Version                    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |                                                           |
| List the Hard Macros - LEF Path & Version                        |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |                                                           |
| Standard Cells - VT type                                         | KC to confirm                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | HVT/RVT/LVT                                               |
| Standard Cells - Timing Library                                  | /home/users/pdks/std\_cells\_lib/ccs/TSMCHOME/digital/Front\_End/timing\_power\_noise/CCS/tcbn22ulpbwp30p140\_100d/tcbn22ulpbwp30p140ffg1p05v125c\_ccs.db<br>/home/users/pdks/std\_cells\_lib/ccs/TSMCHOME/digital/Front\_End/timing\_power\_noise/CCS/tcbn22ulpbwp30p140\_100d/tcbn22ulpbwp30p140ssg0p72vm40c\_ccs.db<br>/home/users/pdks/std\_cells\_lib/ccs/TSMCHOME/digital/Front\_End/timing\_power\_noise/CCS/tcbn22ulpbwp30p140\_100d/tcbn22ulpbwp30p140tt0p9v25c\_ccs.db |                                                           |
| Standard Cells - Physical library                                | /home/users/pdks/std\_cells\_lib/ndm/TSMCHOME/digital/Back\_End/ndm/tcbn22ulpbwp30p140\_100a/tcbn22ulpbwp30p140\_physicalonly.ndm                                                                                                                                                                                                                                                                                                                                                |                                                           |
| IO Pads - Library Path & Versions                                | /home/users/pdks/ios/                                                                                                                                                                                                                                                                                                                                                                                                                                                            |                                                           |
| IO Pads - LEF Path & Versions                                    | /home/users/pdks/ios/                                                                                                                                                                                                                                                                                                                                                                                                                                                            |                                                           |
| CDL files (std cells, IO, macros)                                | /home/users/pdks/                                                                                                                                                                                                                                                                                                                                                                                                                                                                |                                                           |
| GDS Files (std cells, IO, Macros)                                | /home/users/pdks/                                                                                                                                                                                                                                                                                                                                                                                                                                                                |                                                           |
| GDS Map file                                                     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |                                                           |
| Specify RC Extraction Corners (List all the needed Corners)      |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |                                                           |

## Place & Route
| Check Item                                                      | Answer                                 | Example Ans |
| - | - | - |
| 1\. Syn + PnR  (RTL 2 GDSII) or<br>2\. Only PnR  (GATE 2 GDSII) |                                        | 1                                    |
| No of Analog IP/PLL/DLL/EFUSE/MACRO                             | 1\. PLL                                | 2PLL, 1EFUSE                         |
| No of Blocks                                                    | 1\. eFPGA<br>2\. FPGA Controller Block | XX                                   |
| Voltage Domain                                                  | 0.8V, 1.8V                             | 0.9V,1.8V,3.3V                       |
| Voltage Supply name, Voltage                                    |                                        | VDDL, 1.0V, VSS, 0V                  |
| Operating Voltage                                               | 0.8V                                   |                                      |
| Frequency (GHz) (max,operating)                                 | CTS freq - 800MHz                      | block freq 1GHz, Chip Freq 400MHZ    |
| No. of  modes                                                   |                                        | Func/Scan/BIST/JTAG                  |

## Floor Plan
| Check Item                                                                   | Answer                      | Example Ans |
| - | - | - |
| Tap cell distance                                                            |                             | 25                                 |
| End cap / boundary cell requirement                                          |                             | Yes, Top and Bottom of the boundary|
| Bump Information (If flip-chip)                                              |                             |                                    |
| Are the IO buffers required to be added at each of the IO ports of the block |                             |                                    |
| IO pad list                                                                  |                             |                                    |
| Number of IO regions                                                         |                             |                                    |
| IO Pad placement instructions                                                |                             |                                    |
| (1) Specify Buffer Type                                                      |                             |                                    |
| (2) List the exclusion ports if any                                          |                             |                                    |
| Are the Antenna Diodes required to be added for all the io ports?            |                             |                                    |

## Macro Placement
| Check Item                                                            | Answer                             | Example Ans |
| - | - | - |
| Allowable Macro Orientation                                           |                                    | R0, R180, MX, MY                   |
| Isolation requirement for macro?                                      |                                    | Yes, 2 nm                          |
| Need to put any guard ring around the macro                           |                                    | Yes                                |
| Need to put any special cell ( like boundary cell ) around the macro  |                                    | No                                 |
| analog nets / other special net                                       |                                    | No                                 |
| Macro clearance, spacing between macro                                |                                    | 2                                  |
| Are there any additional macro placement  requirement ?               |                                    |                                    |

## Routing Spec
| Check Item                                                            | Answer                            | Example Ans |
| - | - | - |
| Metal Layers Available in Technology file :                           | 10                                |                                     |
| · Metal layers used for Power Routes                                  | See from TSMC DRM                 | M10, M9                             |
| · Most top metal layer usable for Signal Routes                       |                                   | M8                                  |
| Reserved routing layer if any                                         |                                   |                                     |
| List of pre-routes                                                    |                                   |                                     |
| List of nets to be shielded                                           |                                   |                                     |
| List of Non default rules if required                                 |                                   |                                     |
| If multi-cut vias are required to be added                            |                                   |                                     |

## Spare Cell Addition
| Check Item | Answer | Example Ans |
| - | - | - |
| Already added in Netlist. If Yes; the give the identification pattern                                                        |                  | Yes,                       |
| To be added during PnR -<br>i. Number of Modules/ count<br>ii.  Spare Cell List in each module                               |                  |                            |
| For spare cell distribution, please choose (1) Clustered as groups or (2) Fully distributed (homogeneous) or (3) Do not care |                  |                            |


## Others
| Check Item                                                                                                          | Answer           | Example Ans |
| - | - | - |
| List of Synchronizer cell list if any                                                                               |                  | No                        |
| List the "don’t\_touch" cells or give the file name, if applicable                                                  |                  | yes, don't\_touch.tcl     |
| List the "don't\_use" cells or give the file name, if applicable                                                    |                  | No                        |
| List the "size-only" cells or give the file name, if applicable                                                     |                  | No                        |
| Specify any library cells that cannot be used during optimizations.                                                 |                  | xxx                       |
| Provide the scan def for PnR Flow                                                                                   |                  | scan.def                  |
| Decap Filler Cell Insertion Requirement: (1) Wherever possible (2) Only under power/ground nets, Or (3) Not at all  |                  | 1                         |

## Signoff
| Check Item                                                         | Answer                                                  | Example Ans |
| - | - | - |
| STA                                                                |                                                         |                                                           |
| List the timing closure Modes and their corresponding SDC files    |                                                         | Scan mode ; scan.sdc<br>Func mode ; func.sdc              |
| List of timing corner (RC Extraction + PVT/ Operating Condition)   |                                                         | rcBest + 125C, 0.99V<br>cWorst + -40C, 0.81V              |
| Uncertainty                                                        |                                                         |                                                           |
| OCV / AOCV / Derating                                              |                                                         | 3%                                                        |
| Physical Verification check                                        |                                                         | Yes                                                       |
|      -  DRC                                                        |                                                         | Yes                                                       |
|      -  LVS                                                        |                                                         | Yes                                                       |
|      -  ARC                                                        |                                                         |                                                           |
| IR Requirement                                                     |                                                         |                                                           |
| Power Analysis / IR drop Analysis Required?                        |                                                         | Yes                                                       |
| List the PVT ( Operating Conditions) of all corners/cases          |                                                         | func\_mode\_lt\_cbest\_m40c (cbest\_m40c + tcbn40lpbwplt) |
| Dynamic/Static                                                     |                                                         | Static                                                    |
| Activity factor/VCD file                                           |                                                         | VCD                                                       |
| Input switching activity                                           |                                                         | 0.2                                                       |
| Sequential switching activity                                      |                                                         | 0.15                                                      |
| EM Requirement                                                     |                                                         |                                                           |
| EM analysis required ?                                             |                                                         |                                                           |
| List the PVT ( Operating Conditions) of all corners/cases          |                                                         |                                                           |
| Power EM                                                           |                                                         |                                                           |
| Signal EM                                                          |                                                         |                                                           |
|                                                                    |                                                         |                                                           |
