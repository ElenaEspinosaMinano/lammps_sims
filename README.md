<h3 align="center">Summer Project 2024 LAMMPS simulations</h3>

---

Simulations consist of representing a 5 Mbp chromatin region around the mouse _Sox2_ gene as a coarse-grained polymer chain of beads (each bead representing ~1 kbp of chromatin) and representing binding proteins as diffusing beads which interact with the polymer with a specified attraction strength. See [report](https://github.com/ElenaEspinosaMinano/lammps_sims/blob/main/Summer_Project_Report.pdf) and [poster](https://github.com/ElenaEspinosaMinano/lammps_sims/blob/main/Summer_Project_Poster.pdf) for more info.

The **first** investigation (**non_swi_lammps_sims** folder) conisted of running Models 1-4 which contain 5300 atoms in total:
- 5000 polymer beads (4669 type 1, 81 type 2 and 250 type 3 beads)
- 300 non-switching protein beads (type 4)

The **second** investigation (**switching_lammps_sims** folder) conisted of running Models 5-8 which contain 5600 atoms in total:
- 5000 polymer beads (4669 type 1, 81 type 2 and 250 type 3 beads)
- 600 switching protein beads (on average 300 type 4-ON + 5-OFF)

The **third** investigation (**lammps_script_7_multi**) consisted of varying the switching interval of the proteins between 300 and 700 timesteps for Model 7.

The **fourth** investigation (**var_nop** folder) consisted of varying the number of proteins from 300-600 for models 5-8.

  
<!-- This is what the HTML below will output :) chatGPT helped ;)
|               Models                |   Interaction strength (kBT)   |
|-------------------------------------|--------------------------------|
|   Switching OFF  |   Switching ON   | Type 2-4 | Type 3-4 | Type 4-4 |
|------------------|------------------|----------|----------|----------|
|         1        |         5        |    8     |    1     |    1     |
|         2        |         6        |    8     |    4     |    1     |
|         3        |         7        |    8     |    4     |    4     |
|         4        |         8        |    8     |    4     |   1-8/2  |
|         -        |         0        |    1     |    1     |    1     |
 -->

<table>
  <thead>
    <tr>
      <th colspan="2">Models</th>
      <th colspan="3">Interaction strength (kBT)</th>
    </tr>
    <tr>
      <th>Switching OFF</th>
      <th>Switching ON</th>
      <th>Type 2-4</th>
      <th>Type 3-4</th>
      <th>Type 4-4</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>5</td>
      <td>8</td>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <td>2</td>
      <td>6</td>
      <td>8</td>
      <td>4</td>
      <td>1</td>
    </tr>
    <tr>
      <td>3</td>
      <td>7</td>
      <td>8</td>
      <td>4</td>
      <td>4</td>
    </tr>
    <tr>
      <td>4</td>
      <td>8</td>
      <td>8</td>
      <td>4</td>
      <td>1-8 / 2</td>
    </tr>
    <tr>
      <td>-</td>
      <td>0</td>
      <td>1</td>
      <td>1</td>
      <td>1</td>
    </tr>
  </tbody>
</table>
