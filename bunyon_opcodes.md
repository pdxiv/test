# Bunyon opcodes

| Opcode | Mnemonic | Arguments | Comment |
| ------ | -------- | --------- | ------- |
| 0xB7 | has | 1 | |
| 0xB8 | here | 1 | |
| 0xB9 | avail | 1 | |
| 0xBA | !here | 1 | |
| 0xBB | !has | 1 | |
| 0xBC | !avail | 1 | |
| 0xBD | exists | 1 | |
| 0xBE | !exists | 1 | |
| 0xBF | in | 1 | |
| 0xC0 | !in | 1 | |
| 0xC1 | set | 1 | |
| 0xC2 | !set | 1 | |
| 0xC3 | something | 0 | |
| 0xC4 | nothing | 0 | |
| 0xC5 | le | 1 | |
| 0xC6 | gt | 1 | |
| 0xC7 | eq | 1 | |
| 0xC8 | !moved | 1 | |
| 0xC9 | moved | 1 | |
| 0xCA | --0xCA-- | 0 | |
| 0xCB | --0xCB-- | 0 | |
| 0xCC | --0xCC-- | 0 | |
| 0xCD | --0xCD-- | 0 | |
| 0xCE | --0xCE-- | 0 | |
| 0xCF | --0xCF-- | 0 | |
| 0xD0 | --0xD0-- | 0 | |
| 0xD1 | --0xD1-- | 0 | |
| 0xD2 | --0xD2-- | 0 | |
| 0xD3 | --0xD3-- | 0 | |
| 0xD4 | cls | 0 | |
| 0xD5 | pic | 0 | |
| 0xD6 | inv | 0 | |
| 0xD7 | !inv | 0 | |
| 0xD8 | ignore | 0 | |
| 0xD9 | success | 0 | |
| 0xDA | try | 1 | |
| 0xDB | get | 1 | |
| 0xDC | drop | 1 | |
| 0xDD | goto | 1 | |
| 0xDE | zap | 1 | |
| 0xDF | on | 0 | On dark |
| 0xE0 | off | 0 | Off dark |
| 0xE1 | on | 1 | Set flag |
| 0xE2 | off | 1 | Clear flag |
| 0xE3 | on | 0 | |
| 0xE4 | off | 0 | |
| 0xE5 | die | 0 | |
| 0xE6 | move | 2 | |
| 0xE7 | quit | 0 | |
| 0xE8 | .score | 0 | |
| 0xE9 | .inv | 0 | |
| 0xEA | refill | 0 | |
| 0xEB | save | 0 | |
| 0xEC | swap | 2 | Swap items |
| 0xED | steal | 1 | |
| 0xEE | same | 2 | |
| 0xEF | nop | 0 | |
| 0xF0 | .room | 0 | |
| 0xF1 | --0xF1-- | 0 | |
| 0xF2 | add | 0 | |
| 0xF3 | sub | 0 | |
| 0xF4 | .timer | 0 | |
| 0xF5 | timer | 1 | |
| 0xF6 | add | 1 | |
| 0xF7 | sub | 1 | |
| 0xF8 | select_rv | 0 | |
| 0xF9 | swap_rv | 1 | |
| 0xFA | swap | 1 | Swap flag |
| 0xFB | .noun | 0 | |
| 0xFC | .noun_nl | 0 | |
| 0xFD | .nl | 0 | |
| 0xFE | delay | 0 | |
| 0xFF |  | 0 | |