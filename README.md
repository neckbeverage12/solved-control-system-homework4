Download Link: https://assignmentchef.com/product/solved-control-system-homework4
<br>
Control System Homework 4

<ol>

 <li>Consider a unity feedback control system with Gc(s)=K and R(s)=0 for inverted pendulum (example 3.3) in textbook. Use Simulink to simulate the output response for different K in s-domain.</li>

 <li>Use ode45 to simulate the output response for different K in time-</li>

</ol>

Analyze C = [0,0,1,0],[0,0,1,1] and [0,1,1,1] and different K.

For this homework, you should additionally submit a report including your analysis. Give the reason if you can’t reach the expected control goal.

<em>EXAMPLE 3.3</em><strong> Inverted pendulum control</strong>

The problem of balancing a broomstick on a person’s hand is illustrated in Figure 3.18. The only equilibrium condition is <em>0(t) </em>= 0 and <em>dO(t)/dt = </em>0. The problem of balanc­ing a broomstick on one’s hand is not unlike the problem of controlling the attitude of a missile during the initial stages of launch. This problem is the classic and intrigu­ing problem of the inverted pendulum mounted on a cart, as shown in Figure 3.19. The cart must be moved so that mass m is always in an upright position. The state variables must be expressed in terms of the angular rotation <em>0(0 </em>and the position of the cart <em>y(t), </em>The differential equations describing the motion of the system can be obtained by writing the sum of the forces in the horizontal direction and the sum of the moments about the pivot point [2, 3, 10, 23], We will assume that Al &gt;&gt; in and the angle of rotation <em>0(t), </em>is small so that the equations are linear. The sum of the forces in the horizontal direction is

h1 t)+                      <em>tt(t) </em>= 0,                                          (3.63)

where <em>rs(t) </em>equals the force on the cart, and is the distance from the mass <em>in </em>to the pivot point. The sum of the torques about the pivot point is

<em>in/y(t)        m1<sup>2</sup>0(t) </em>— <em>ig0(t) = </em>0.                               (3.64)

The state variables for the two second-order equations arc chosen as (x<sub>i</sub><em> (t), </em>x<sub>2</sub>(t), x<sub>3</sub>(0, x<sub>4</sub>(t) ) = <em>(y(1), At), 9(t), 0(0). </em>Then Equations (3,63) and (3.64) are written in terms of the state variables as

<em>Mi<sub>2</sub>(t) + mii<sub>4</sub>(t) — u(t) = </em>0                                  (3.65)

and

<em>k<sub>2</sub>(t) + 11<sub>4</sub>(t) — gx-4t) = </em>0.                                            (3.66)




To obtain the necessary first-order differential equations, we solve for Ec<sub>4</sub>(t) in Equation (3.66) and substitute into Equation (3.65) to obtain

<table>

 <tbody>

  <tr>

   <td rowspan="3" width="150">since <em>M </em>&gt;&gt; <em>m. </em>Substituting haveTherefore, the four first-order<em>i<sub>i</sub>(t)</em><em>_i</em><em><sub>3</sub></em><em>(t)</em>Thus, the system matricesA=</td>

   <td rowspan="3" width="147"><em>Mi2(t)             </em><em>mgx</em><em><sub>3</sub></em><em>(t)</em>.i<sub>2</sub>(t) from Equation<em>ML5c<sub>4</sub>(t) </em>— <em>Mgx<sub>3</sub>(t)</em>differential equations <em>= x<sub>2</sub>(t),          i<sub>2</sub> (t) =</em><em>=</em><em> x</em><em><sub>4</sub></em><em>(t),     </em>and    <em>x<sub>4</sub>(t)</em>are<em>0       1         0            0</em><em>0       0      –mg/ Al      0</em><em>0       0         0            1</em><em>_O     0         g /1          0_</em></td>

   <td width="71"><em>= u(t),</em>(3.65) <em>u(t) </em>=can<em>rng</em></td>

   <td rowspan="2" width="77">into Equation0.be written<em>+</em><em><sup> 1</sup></em><em> —u(t),</em><em>1</em></td>

   <td rowspan="3" width="119">(3.67) (3.66). we(168)as(3.69)(3.70) ■</td>

   <td width="0"></td>

  </tr>

  <tr>

   <td rowspan="2" width="71"><em>.</em><em>—      x<sub>3</sub>(t)</em>=       x<sub>3</sub>(t)B</td>

  </tr>

  <tr>

   <td width="77">—<em> —</em><em><sub>mi</sub></em><em>u(t).</em>01/M0<em>–1/(MO_</em></td>

  </tr>

 </tbody>

</table>







<strong>FIGURE </strong><strong>3.18</strong>

An inverted pendulum balanced on a person’s hand by moving the hand to reduce <em>6 (t) . </em>Assume, for ease, that the pendulum rotates in the x—y plane.

<strong>FIGURE 3.19</strong>

A cart and an in­verted pendulum. The pendulum is constrained to pivot in the vertical plane.