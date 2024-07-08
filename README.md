<h1 align="center"><b> Library/Driver file for MT25QL01GBBB8ESF-0SIT (1 Gbit) NOR Flash Memory.</b></h1>

<div align="justify">
  This library/driver can easily be used for other Microcontrollers with very less modifications. Integration of file system such as littlfs and smartfs is also possible with minimal modifications. Example implementaion code available in <i>Core/Src/main.c</i>. Library implememtation available at <i>Core/Src/MT25QL.c</i>.
</div>

<h2>Please Read the MT24QL01 Flash Memory Datasheet before using the library for easy use.<br><br>
Please make sure commands from datasheet match the commands defined in MT25QL01.h, <u>Commands differ for different part numbers.</u></h2>

<div>
  <h2>Check following before using the library:</h2>
  <ul>
    <li>
      Make sure you assign correct SPI to Flash Memory Functions
    </li>
    <li>
      Be sure to assign Debug UART to seee the debug messages or comment out the myprintf functions to remove debug messages
      <ul>
        <li>
          assign proper UART to DEBUG_STREAM definition
      </ul>
    </li>
    <li>
      Assign correct Chip Select line for corresponding SPI line. Make changes to FM_Enable() and FM_Disable() functions.
    </li>
    <li>
      Erase the corresponding sector/subsector of Flash Memory before rewriting. Read datasheet properly for easy use.
    </li>
  </ul>
</div>

