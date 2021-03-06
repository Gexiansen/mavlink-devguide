<!-- THIS FILE IS AUTO-GENERATED: https://github.com/mavlink/mavlink/blob/master/doc/mavlink_gitbook.py -->

# MAVLINK Message Set: minimal.xml

*This is a human-readable form of the XML definition file: [minimal.xml](https://github.com/mavlink/mavlink/blob/master/message_definitions/v1.0/minimal.xml).*

<span></span>

> **Note** MAVLink 2 messages have an ID > 255 and are marked up using **(MAVLink 2)** in their description.

<span id="mav2_extension_field"></span>

> **Note** MAVLink 2 extension fields that have been added to MAVLink 1 messages are displayed in blue. 

<style>
td {
    vertical-align:top;
}
</style>

 <html>
 <body></p>

<h2>MAVLink Protocol Version</h2>

<p>The current MAVLink version is 2.2. The minor version numbers (after the dot) range from 1-255.</p>

<h2>MAVLink Type Enumerations</h2>

<h3 id="MAV_AUTOPILOT">
   <a href="#MAV_AUTOPILOT">MAV_AUTOPILOT</a>
  </h3>

<p>Micro air vehicle / autopilot classes. This identifies the individual model.</p>

<table class="sortable">
   <thead>
    <tr>
     <th>Value</th>
     <th>Field Name</th>
     <th>Description</th>
    </tr>
   </thead>
   <tbody>
    <tr id="MAV_AUTOPILOT_GENERIC">
     <td>0</td>
     <td>
      <a href="#MAV_AUTOPILOT_GENERIC">MAV_AUTOPILOT_GENERIC</a>
     </td>
     <td>Generic autopilot, full support for everything</td>
    </tr>
    <tr id="MAV_AUTOPILOT_PIXHAWK">
     <td>1</td>
     <td>
      <a href="#MAV_AUTOPILOT_PIXHAWK">MAV_AUTOPILOT_PIXHAWK</a>
     </td>
     <td>PIXHAWK autopilot, http://pixhawk.ethz.ch</td>
    </tr>
    <tr id="MAV_AUTOPILOT_SLUGS">
     <td>2</td>
     <td>
      <a href="#MAV_AUTOPILOT_SLUGS">MAV_AUTOPILOT_SLUGS</a>
     </td>
     <td>SLUGS autopilot, http://slugsuav.soe.ucsc.edu</td>
    </tr>
    <tr id="MAV_AUTOPILOT_ARDUPILOTMEGA">
     <td>3</td>
     <td>
      <a href="#MAV_AUTOPILOT_ARDUPILOTMEGA">MAV_AUTOPILOT_ARDUPILOTMEGA</a>
     </td>
     <td>ArduPilotMega / ArduCopter, http://diydrones.com</td>
    </tr>
    <tr id="MAV_AUTOPILOT_OPENPILOT">
     <td>4</td>
     <td>
      <a href="#MAV_AUTOPILOT_OPENPILOT">MAV_AUTOPILOT_OPENPILOT</a>
     </td>
     <td>OpenPilot, http://openpilot.org</td>
    </tr>
    <tr id="MAV_AUTOPILOT_GENERIC_WAYPOINTS_ONLY">
     <td>5</td>
     <td>
      <a href="#MAV_AUTOPILOT_GENERIC_WAYPOINTS_ONLY">MAV_AUTOPILOT_GENERIC_WAYPOINTS_ONLY</a>
     </td>
     <td>Generic autopilot only supporting simple waypoints</td>
    </tr>
    <tr id="MAV_AUTOPILOT_GENERIC_WAYPOINTS_AND_SIMPLE_NAVIGATION_ONLY">
     <td>6</td>
     <td>
      <a href="#MAV_AUTOPILOT_GENERIC_WAYPOINTS_AND_SIMPLE_NAVIGATION_ONLY">MAV_AUTOPILOT_GENERIC_WAYPOINTS_AND_SIMPLE_NAVIGATION_ONLY</a>
     </td>
     <td>Generic autopilot supporting waypoints and other simple navigation commands</td>
    </tr>
    <tr id="MAV_AUTOPILOT_GENERIC_MISSION_FULL">
     <td>7</td>
     <td>
      <a href="#MAV_AUTOPILOT_GENERIC_MISSION_FULL">MAV_AUTOPILOT_GENERIC_MISSION_FULL</a>
     </td>
     <td>Generic autopilot supporting the full mission command set</td>
    </tr>
    <tr id="MAV_AUTOPILOT_INVALID">
     <td>8</td>
     <td>
      <a href="#MAV_AUTOPILOT_INVALID">MAV_AUTOPILOT_INVALID</a>
     </td>
     <td>No valid autopilot, e.g. a GCS or other MAVLink component</td>
    </tr>
    <tr id="MAV_AUTOPILOT_PPZ">
     <td>9</td>
     <td>
      <a href="#MAV_AUTOPILOT_PPZ">MAV_AUTOPILOT_PPZ</a>
     </td>
     <td>PPZ UAV - http://nongnu.org/paparazzi</td>
    </tr>
    <tr id="MAV_AUTOPILOT_UDB">
     <td>10</td>
     <td>
      <a href="#MAV_AUTOPILOT_UDB">MAV_AUTOPILOT_UDB</a>
     </td>
     <td>UAV Dev Board</td>
    </tr>
    <tr id="MAV_AUTOPILOT_FP">
     <td>11</td>
     <td>
      <a href="#MAV_AUTOPILOT_FP">MAV_AUTOPILOT_FP</a>
     </td>
     <td>FlexiPilot</td>
    </tr>
   </tbody>
  </table>

<h3 id="MAV_TYPE">
   <a href="#MAV_TYPE">MAV_TYPE</a>
  </h3>

<p>
  </p>

<table class="sortable">
   <thead>
    <tr>
     <th>Value</th>
     <th>Field Name</th>
     <th>Description</th>
    </tr>
   </thead>
   <tbody>
    <tr id="MAV_TYPE_GENERIC">
     <td>0</td>
     <td>
      <a href="#MAV_TYPE_GENERIC">MAV_TYPE_GENERIC</a>
     </td>
     <td>Generic micro air vehicle.</td>
    </tr>
    <tr id="MAV_TYPE_FIXED_WING">
     <td>1</td>
     <td>
      <a href="#MAV_TYPE_FIXED_WING">MAV_TYPE_FIXED_WING</a>
     </td>
     <td>Fixed wing aircraft.</td>
    </tr>
    <tr id="MAV_TYPE_QUADROTOR">
     <td>2</td>
     <td>
      <a href="#MAV_TYPE_QUADROTOR">MAV_TYPE_QUADROTOR</a>
     </td>
     <td>Quadrotor</td>
    </tr>
    <tr id="MAV_TYPE_COAXIAL">
     <td>3</td>
     <td>
      <a href="#MAV_TYPE_COAXIAL">MAV_TYPE_COAXIAL</a>
     </td>
     <td>Coaxial helicopter</td>
    </tr>
    <tr id="MAV_TYPE_HELICOPTER">
     <td>4</td>
     <td>
      <a href="#MAV_TYPE_HELICOPTER">MAV_TYPE_HELICOPTER</a>
     </td>
     <td>Normal helicopter with tail rotor.</td>
    </tr>
    <tr id="MAV_TYPE_ANTENNA_TRACKER">
     <td>5</td>
     <td>
      <a href="#MAV_TYPE_ANTENNA_TRACKER">MAV_TYPE_ANTENNA_TRACKER</a>
     </td>
     <td>Ground installation</td>
    </tr>
    <tr id="MAV_TYPE_GCS">
     <td>6</td>
     <td>
      <a href="#MAV_TYPE_GCS">MAV_TYPE_GCS</a>
     </td>
     <td>Operator control unit / ground control station</td>
    </tr>
    <tr id="MAV_TYPE_AIRSHIP">
     <td>7</td>
     <td>
      <a href="#MAV_TYPE_AIRSHIP">MAV_TYPE_AIRSHIP</a>
     </td>
     <td>Airship, controlled</td>
    </tr>
    <tr id="MAV_TYPE_FREE_BALLOON">
     <td>8</td>
     <td>
      <a href="#MAV_TYPE_FREE_BALLOON">MAV_TYPE_FREE_BALLOON</a>
     </td>
     <td>Free balloon, uncontrolled</td>
    </tr>
    <tr id="MAV_TYPE_ROCKET">
     <td>9</td>
     <td>
      <a href="#MAV_TYPE_ROCKET">MAV_TYPE_ROCKET</a>
     </td>
     <td>Rocket</td>
    </tr>
    <tr id="MAV_TYPE_GROUND_ROVER">
     <td>10</td>
     <td>
      <a href="#MAV_TYPE_GROUND_ROVER">MAV_TYPE_GROUND_ROVER</a>
     </td>
     <td>Ground rover</td>
    </tr>
    <tr id="MAV_TYPE_SURFACE_BOAT">
     <td>11</td>
     <td>
      <a href="#MAV_TYPE_SURFACE_BOAT">MAV_TYPE_SURFACE_BOAT</a>
     </td>
     <td>Surface vessel, boat, ship</td>
    </tr>
    <tr id="MAV_TYPE_SUBMARINE">
     <td>12</td>
     <td>
      <a href="#MAV_TYPE_SUBMARINE">MAV_TYPE_SUBMARINE</a>
     </td>
     <td>Submarine</td>
    </tr>
    <tr id="MAV_TYPE_HEXAROTOR">
     <td>13</td>
     <td>
      <a href="#MAV_TYPE_HEXAROTOR">MAV_TYPE_HEXAROTOR</a>
     </td>
     <td>Hexarotor</td>
    </tr>
    <tr id="MAV_TYPE_OCTOROTOR">
     <td>14</td>
     <td>
      <a href="#MAV_TYPE_OCTOROTOR">MAV_TYPE_OCTOROTOR</a>
     </td>
     <td>Octorotor</td>
    </tr>
    <tr id="MAV_TYPE_TRICOPTER">
     <td>15</td>
     <td>
      <a href="#MAV_TYPE_TRICOPTER">MAV_TYPE_TRICOPTER</a>
     </td>
     <td>Octorotor</td>
    </tr>
    <tr id="MAV_TYPE_FLAPPING_WING">
     <td>16</td>
     <td>
      <a href="#MAV_TYPE_FLAPPING_WING">MAV_TYPE_FLAPPING_WING</a>
     </td>
     <td>Flapping wing</td>
    </tr>
   </tbody>
  </table>

<h3 id="MAV_MODE_FLAG">
   <a href="#MAV_MODE_FLAG">MAV_MODE_FLAG</a>
  </h3>

<p>These flags encode the MAV mode.</p>

<table class="sortable">
   <thead>
    <tr>
     <th>Value</th>
     <th>Field Name</th>
     <th>Description</th>
    </tr>
   </thead>
   <tbody>
    <tr id="MAV_MODE_FLAG_SAFETY_ARMED">
     <td>128</td>
     <td>
      <a href="#MAV_MODE_FLAG_SAFETY_ARMED">MAV_MODE_FLAG_SAFETY_ARMED</a>
     </td>
     <td>0b10000000 MAV safety set to armed. Motors are enabled / running / can start. Ready to fly.</td>
    </tr>
    <tr id="MAV_MODE_FLAG_MANUAL_INPUT_ENABLED">
     <td>64</td>
     <td>
      <a href="#MAV_MODE_FLAG_MANUAL_INPUT_ENABLED">MAV_MODE_FLAG_MANUAL_INPUT_ENABLED</a>
     </td>
     <td>0b01000000 remote control input is enabled.</td>
    </tr>
    <tr id="MAV_MODE_FLAG_HIL_ENABLED">
     <td>32</td>
     <td>
      <a href="#MAV_MODE_FLAG_HIL_ENABLED">MAV_MODE_FLAG_HIL_ENABLED</a>
     </td>
     <td>0b00100000 hardware in the loop simulation. All motors / actuators are blocked, but internal software is full operational.</td>
    </tr>
    <tr id="MAV_MODE_FLAG_STABILIZE_ENABLED">
     <td>16</td>
     <td>
      <a href="#MAV_MODE_FLAG_STABILIZE_ENABLED">MAV_MODE_FLAG_STABILIZE_ENABLED</a>
     </td>
     <td>0b00010000 system stabilizes electronically its attitude (and optionally position). It needs however further control inputs to move around.</td>
    </tr>
    <tr id="MAV_MODE_FLAG_GUIDED_ENABLED">
     <td>8</td>
     <td>
      <a href="#MAV_MODE_FLAG_GUIDED_ENABLED">MAV_MODE_FLAG_GUIDED_ENABLED</a>
     </td>
     <td>0b00001000 guided mode enabled, system flies waypoints / mission items.</td>
    </tr>
    <tr id="MAV_MODE_FLAG_AUTO_ENABLED">
     <td>4</td>
     <td>
      <a href="#MAV_MODE_FLAG_AUTO_ENABLED">MAV_MODE_FLAG_AUTO_ENABLED</a>
     </td>
     <td>0b00000100 autonomous mode enabled, system finds its own goal positions. Guided flag can be set or not, depends on the actual implementation.</td>
    </tr>
    <tr id="MAV_MODE_FLAG_TEST_ENABLED">
     <td>2</td>
     <td>
      <a href="#MAV_MODE_FLAG_TEST_ENABLED">MAV_MODE_FLAG_TEST_ENABLED</a>
     </td>
     <td>0b00000010 system has a test mode enabled. This flag is intended for temporary system tests and should not be used for stable implementations.</td>
    </tr>
    <tr id="MAV_MODE_FLAG_CUSTOM_MODE_ENABLED">
     <td>1</td>
     <td>
      <a href="#MAV_MODE_FLAG_CUSTOM_MODE_ENABLED">MAV_MODE_FLAG_CUSTOM_MODE_ENABLED</a>
     </td>
     <td>0b00000001 Reserved for future use.</td>
    </tr>
   </tbody>
  </table>

<h3 id="MAV_MODE_FLAG_DECODE_POSITION">
   <a href="#MAV_MODE_FLAG_DECODE_POSITION">MAV_MODE_FLAG_DECODE_POSITION</a>
  </h3>

<p>These values encode the bit positions of the decode position. These values can be used to read the value of a flag bit by combining the base_mode variable with AND with the flag position value. The result will be either 0 or 1, depending on if the flag is set or not.</p>

<table class="sortable">
   <thead>
    <tr>
     <th>Value</th>
     <th>Field Name</th>
     <th>Description</th>
    </tr>
   </thead>
   <tbody>
    <tr id="MAV_MODE_FLAG_DECODE_POSITION_SAFETY">
     <td>128</td>
     <td>
      <a href="#MAV_MODE_FLAG_DECODE_POSITION_SAFETY">MAV_MODE_FLAG_DECODE_POSITION_SAFETY</a>
     </td>
     <td>First bit:  10000000</td>
    </tr>
    <tr id="MAV_MODE_FLAG_DECODE_POSITION_MANUAL">
     <td>64</td>
     <td>
      <a href="#MAV_MODE_FLAG_DECODE_POSITION_MANUAL">MAV_MODE_FLAG_DECODE_POSITION_MANUAL</a>
     </td>
     <td>Second bit: 01000000</td>
    </tr>
    <tr id="MAV_MODE_FLAG_DECODE_POSITION_HIL">
     <td>32</td>
     <td>
      <a href="#MAV_MODE_FLAG_DECODE_POSITION_HIL">MAV_MODE_FLAG_DECODE_POSITION_HIL</a>
     </td>
     <td>Third bit:  00100000</td>
    </tr>
    <tr id="MAV_MODE_FLAG_DECODE_POSITION_STABILIZE">
     <td>16</td>
     <td>
      <a href="#MAV_MODE_FLAG_DECODE_POSITION_STABILIZE">MAV_MODE_FLAG_DECODE_POSITION_STABILIZE</a>
     </td>
     <td>Fourth bit: 00010000</td>
    </tr>
    <tr id="MAV_MODE_FLAG_DECODE_POSITION_GUIDED">
     <td>8</td>
     <td>
      <a href="#MAV_MODE_FLAG_DECODE_POSITION_GUIDED">MAV_MODE_FLAG_DECODE_POSITION_GUIDED</a>
     </td>
     <td>Fifth bit:  00001000</td>
    </tr>
    <tr id="MAV_MODE_FLAG_DECODE_POSITION_AUTO">
     <td>4</td>
     <td>
      <a href="#MAV_MODE_FLAG_DECODE_POSITION_AUTO">MAV_MODE_FLAG_DECODE_POSITION_AUTO</a>
     </td>
     <td>Sixt bit:   00000100</td>
    </tr>
    <tr id="MAV_MODE_FLAG_DECODE_POSITION_TEST">
     <td>2</td>
     <td>
      <a href="#MAV_MODE_FLAG_DECODE_POSITION_TEST">MAV_MODE_FLAG_DECODE_POSITION_TEST</a>
     </td>
     <td>Seventh bit: 00000010</td>
    </tr>
    <tr id="MAV_MODE_FLAG_DECODE_POSITION_CUSTOM_MODE">
     <td>1</td>
     <td>
      <a href="#MAV_MODE_FLAG_DECODE_POSITION_CUSTOM_MODE">MAV_MODE_FLAG_DECODE_POSITION_CUSTOM_MODE</a>
     </td>
     <td>Eighth bit: 00000001</td>
    </tr>
   </tbody>
  </table>

<h3 id="MAV_STATE">
   <a href="#MAV_STATE">MAV_STATE</a>
  </h3>

<p>
  </p>

<table class="sortable">
   <thead>
    <tr>
     <th>Value</th>
     <th>Field Name</th>
     <th>Description</th>
    </tr>
   </thead>
   <tbody>
    <tr id="MAV_STATE_UNINIT">
     <td>0</td>
     <td>
      <a href="#MAV_STATE_UNINIT">MAV_STATE_UNINIT</a>
     </td>
     <td>Uninitialized system, state is unknown.</td>
    </tr>
    <tr id="MAV_STATE_BOOT">
     <td>
     </td>
     <td>
      <a href="#MAV_STATE_BOOT">MAV_STATE_BOOT</a>
     </td>
     <td>System is booting up.</td>
    </tr>
    <tr id="MAV_STATE_CALIBRATING">
     <td>
     </td>
     <td>
      <a href="#MAV_STATE_CALIBRATING">MAV_STATE_CALIBRATING</a>
     </td>
     <td>System is calibrating and not flight-ready.</td>
    </tr>
    <tr id="MAV_STATE_STANDBY">
     <td>
     </td>
     <td>
      <a href="#MAV_STATE_STANDBY">MAV_STATE_STANDBY</a>
     </td>
     <td>System is grounded and on standby. It can be launched any time.</td>
    </tr>
    <tr id="MAV_STATE_ACTIVE">
     <td>
     </td>
     <td>
      <a href="#MAV_STATE_ACTIVE">MAV_STATE_ACTIVE</a>
     </td>
     <td>System is active and might be already airborne. Motors are engaged.</td>
    </tr>
    <tr id="MAV_STATE_CRITICAL">
     <td>
     </td>
     <td>
      <a href="#MAV_STATE_CRITICAL">MAV_STATE_CRITICAL</a>
     </td>
     <td>System is in a non-normal flight mode. It can however still navigate.</td>
    </tr>
    <tr id="MAV_STATE_EMERGENCY">
     <td>
     </td>
     <td>
      <a href="#MAV_STATE_EMERGENCY">MAV_STATE_EMERGENCY</a>
     </td>
     <td>System is in a non-normal flight mode. It lost control over parts or over the whole airframe. It is in mayday and going down.</td>
    </tr>
    <tr id="MAV_STATE_POWEROFF">
     <td>
     </td>
     <td>
      <a href="#MAV_STATE_POWEROFF">MAV_STATE_POWEROFF</a>
     </td>
     <td>System just initialized its power-down sequence, will shut down now.</td>
    </tr>
   </tbody>
  </table>

<h2>MAVLink Messages</h2>

<h3 id="HEARTBEAT">HEARTBEAT (<a href="#HEARTBEAT">
    #0
   </a>
   )
  </h3>

<p>The heartbeat message shows that a system is present and responding. The type of the MAV and Autopilot hardware allow the receiving system to treat further messages from this system appropriate (e.g. by laying out the user interface based on the autopilot).</p>

<table class="sortable">
   <thead>
    <tr>
     <th>Field Name</th>
     <th>Type</th>
     <th>Values</th>
     <th>Description</th>
    </tr>
   </thead>
   <tbody>
    <tr>
     <td>type</td>
     <td>uint8_t</td>
     <td>
      <a href="#MAV_TYPE">MAV_TYPE</a>
     </td>
     <td>Type of the MAV (quadrotor, helicopter, etc., up to 15 types, defined in MAV_TYPE ENUM)</td>
    </tr>
    <tr>
     <td>autopilot</td>
     <td>uint8_t</td>
     <td>
      <a href="#MAV_AUTOPILOT">MAV_AUTOPILOT</a>
     </td>
     <td>Autopilot type / class. defined in MAV_AUTOPILOT ENUM</td>
    </tr>
    <tr>
     <td>base_mode</td>
     <td>uint8_t</td>
     <td>
      <a href="#">
      </a>
     </td>
     <td>System mode bitfield, see MAV_MODE_FLAGS ENUM in mavlink/include/mavlink_types.h</td>
    </tr>
    <tr>
     <td>custom_mode</td>
     <td>uint32_t</td>
     <td>
      <a href="#">
      </a>
     </td>
     <td>A bitfield for use for autopilot-specific flags.</td>
    </tr>
    <tr>
     <td>system_status</td>
     <td>uint8_t</td>
     <td>
      <a href="#MAV_STATE">MAV_STATE</a>
     </td>
     <td>System status flag, see MAV_STATE ENUM</td>
    </tr>
    <tr>
     <td>mavlink_version</td>
     <td>uint8_t_mavlink_version</td>
     <td>
      <a href="#">
      </a>
     </td>
     <td>MAVLink version</td>
    </tr>
   </tbody>
  </table>

<p></body>
</html>
