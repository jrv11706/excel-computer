# excel-computer
The 16-bit Excel Computer is a personal project that was a long awaited goal since first learning about logic design! It is highly inspired and possible due to the amazing nandgame.com. 
The computer has two registers A and D, and 65536 addresses of RAM. The ram addresses are pointed to by the A register. The computer has an ALU capable of addition, subtraction, bitwise AND, OR, XOR, and NOT.
Lastly, there is 65536 addresses of ROM that a user can write to in decimal. Decimal instructions can be generated using the Instruction Encoder sheet.
-
-
-
USING EXCEL COMPUTER:
The entire computer runs off of a 0.5 Hz clock that is based off of the current time, so running requires constant refreshing. This can be achieved by the user holding down the F9 key.
NOTE that this is a resource intensive method of recreating a clock, so most computers do not like it very much.
-
{CPU}
The CPU sheet has one interactable checkbox in the bright red cell that is meant as a RESET. Having the box checked will load a 0 into every register on the next clock cycle.
This leads to the Program Counter being set to 0, the A and D registers being set to 0, and every address in RAM being set to 0.
NOTE that you must un-check this box in order for any program to run.
-
{ROM-RAM}
Users can interact with the ROM-RAM sheet by editing the program ROM. Also on this sheet, you can see pointers on the side of the ROM and RAM stacks that show you how the computer is currently interacting with each!
The pointer on the ROM stack shows the user which instruction line is currently being executed, and the RAM pointers shows you which address is currently available to the instruction decoder.
-
{Instruction Encoder}
In case you are unable to just write decimal and get the instruction you want first try, the Instruction Encoder sheet is available with checkboxes that represent each bit of an instruction code. Each bit flag is labeled
with a name so it is slightly intuitive on how to craft which instruction you want. The results are: The instruction in decimal, the instruction in hex, and the translation of the instruction. Users can then copy the decimal
into the ROM, where it will also translate the decimal number to confirm the instruction.
-
-
-
The computer comes pre-loaded with the RESET box checked, and an example program in the ROM that writes numbers 0-65535 to RAM in increasing addresses.
Enjoy the 16-bit Excel Computer!
