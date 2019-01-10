# TI99/4A opcodes

The opcodes in the TI99/4A file format are fairly different from the ones in the TRS-80 text format.

Codes 0x00 to 0xB6 *seem* to be reserved for text messages. (If so, this means that the file format theoretically allows up to 183 text messages.)

The first 19 opcodes (0xB7 to 0xC9) fill a similar function as "conditions" in the TRS-80 format.

The last 44 opcodes (0xD4 to 0xFF) fill a similar function as "commands" in the TRS-80 format.

| Opcode | Mnemonic | Arguments | Comment |
| ------ | -------- | --------- | ------- |
| 0xB7 | has | 1 | ITEM is in inventory |
| 0xB8 | here | 1 | ITEM is in room |
| 0xB9 | avail | 1 | Is ITEM available (in inventory or in room) |
| 0xBA | !here | 1 | ITEM is NOT in room |
| 0xBB | !has | 1 | ITEM is NOT in inventory |
| 0xBC | !avail | 1 | Is ITEM NOT available (in inventory or in room) |
| 0xBD | exists | 1 | Object exists |
| 0xBE | !exists | 1 | Object NOT exists |
| 0xBF | in | 1 | Player is in room X |
| 0xC0 | !in | 1 | Player not in room X |
| 0xC1 | set | 1 | Check if flag N is SET, return TRUE.. |
| 0xC2 | !set | 1 | Check if flag N is NOT SET, return TRUE.. |
| 0xC3 | something | 0 | Something |
| 0xC4 | nothing | 0 | Nothing |
| 0xC5 | le | 1 | Less than or equal to |
| 0xC6 | gt | 1 | Greater than |
| 0xC7 | eq | 1 | == |
| 0xC8 | !moved | 1 | Not moved item? |
| 0xC9 | moved | 1 | Moved item? |
| 0xCA | --0xCA-- | 0 | Unknown |
| 0xCB | --0xCB-- | 0 | Unknown |
| 0xCC | --0xCC-- | 0 | Unknown |
| 0xCD | --0xCD-- | 0 | Unknown |
| 0xCE | --0xCE-- | 0 | Unknown |
| 0xCF | --0xCF-- | 0 | Unknown |
| 0xD0 | --0xD0-- | 0 | Unknown |
| 0xD1 | --0xD1-- | 0 | Unknown |
| 0xD2 | --0xD2-- | 0 | Unknown |
| 0xD3 | --0xD3-- | 0 | Unknown |
| 0xD4 | cls | 0 | Clear screen |
| 0xD5 | pic | 0 | Inv |
| 0xD6 | inv | 0 | !inv. Turn automatic inventory on |
| 0xD7 | !inv | 0 | Ignore. Turn automatic inventory off |
| 0xD8 | ignore | 0 | Success |
| 0xD9 | success | 0 | TODO: fix this opcode! try? |
| 0xDA | try | 1 | Try |
| 0xDB | get | 1 | Get item |
| 0xDC | drop | 1 | Drop item |
| 0xDD | goto | 1 | Goto room |
| 0xDE | zap | 1 | Move item B to room A |
| 0xDF | on | 0 | On darkness |
| 0xE0 | off | 0 | Off darkness |
| 0xE1 | on | 1 | Set flag X on |
| 0xE2 | off | 1 | Set flag X off |
| 0xE3 | on | 0 | Set flag 0 ON |
| 0xE4 | off | 0 | Set flag 0 OFF |
| 0xE5 | die | 0 | Die |
| 0xE6 | move | 2 | Move item B to room A |
| 0xE7 | quit | 0 | Quit |
| 0xE8 | .score | 0 | Print score |
| 0xE9 | .inv | 0 | List contents of inventory |
| 0xEA | refill | 0 | Refill |
| 0xEB | save | 0 | Save |
| 0xEC | swap | 2 | Swap items 1 and 2 around |
| 0xED | steal | 1 | Move an item to the inventory |
| 0xEE | same | 2 | Make item1 same room as item2 |
| 0xEF | nop | 0 | Nop |
| 0xF0 | .room | 0 | Look at room |
| 0xF1 | --0xF1-- | 0 | Unknown |
| 0xF2 | add | 0 | Add 1 to timer |
| 0xF3 | sub | 0 | Sub 1 from timer |
| 0xF4 | .timer | 0 | Print current timer |
| 0xF5 | timer | 1 | Set timer |
| 0xF6 | add | 1 | Add to timer |
| 0xF7 | sub | 1 | Sub from timer |
| 0xF8 | select_rv | 0 | Select room counter |
| 0xF9 | swap_rv | 1 | Swap room counter |
| 0xFA | swap | 1 | Swap timer |
| 0xFB | .noun | 0 | Print noun |
| 0xFC | .noun_nl | 0 | Print noun + newline |
| 0xFD | .nl | 0 | Print newline |
| 0xFE | delay | 0 | Delay |
| 0xFF |   | 0 | End of code block. |