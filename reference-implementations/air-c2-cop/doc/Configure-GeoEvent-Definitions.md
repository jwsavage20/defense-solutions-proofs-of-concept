<p>To run the simulations and configure services GeoEvent must have a number of event definitions created or imported from feature classes.</p>
<ol class="steps">
  <li>Create a new GeoEvent Definition named Airc2-CivilianAirtracksIn. Use the following table as a guide to create the fields.</li>
<table class="bordered stripe lined-columns lined-rows">
  <thead>
    <tr>
      <td>Name</td>
      <td>Type</td>
      <td>Cardinality</td>
      <td>Tags</td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>OID</td>
      <td>Integer</td>
      <td>1</td>
      <td> </td>
    </tr>
    <tr>
      <td>ident</td>
      <td>Integer</td>
      <td>1</td>
      <td> </td>
    </tr>
    <tr>
      <td>lat</td>
      <td>Double</td>
      <td>1</td>
      <td> </td>
    </tr>
    <tr>
      <td>lon</td>
      <td>Double</td>
      <td>1</td>
      <td> </td>
    </tr>
    <tr>
      <td>id</td>
      <td>String</td>
      <td>1</td>
      <td>TRACK_ID</td>
    </tr>
    <tr>
						<td>alt</td>
						<td>Double</td>
						<td>1</td>
						<td> </td>
					</tr>
					<tr>
						<td>gs</td>
						<td>Integer</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>time</td>
						<td>Date</td>
						<td>1</td>
						<td>TIME_START</td>
					</tr>
					<tr>
						<td>heading</td>
						<td>Integer</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>geometry</td>
						<td>Geometry</td>
						<td>1</td>
						<td>GEOMETRY</td>
					</tr>
				</tbody>
			</table>
			<li>Create a new GeoEvent Definition named Airc2-MilitaryAirtracksIn. Use the following table as a guide to create the fields.</li>
			<table class="bordered stripe lined-columns lined-rows">
				<thead>
					<tr>
						<td>Name</td>
						<td>Type</td>
						<td>Cardinality</td>
						<td>Tags</td>
					</tr>
				</thead>
				<tbody>
					<tr>
						<td>OID</td>
						<td>Integer</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>ident</td>
						<td>Integer</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>lat</td>
						<td>Double</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>lon</td>
						<td>Double</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>id</td>
						<td>String</td>
						<td>1</td>
						<td>TRACK_ID</td>
					</tr>
					<tr>
						<td>alt</td>
						<td>Double</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>heading</td>
						<td>Integer</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>time</td>
						<td>Date</td>
						<td>1</td>
						<td>TIME_START</td>
					</tr>
					<tr>
						<td>SIDC_2525D</td>
						<td>String</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>geometry</td>
						<td>Geometry</td>
						<td>1</td>
						<td>GEOMETRY</td>
					</tr>
				</tbody>
			</table>
			<li>Create a new GeoEvent Definition named Airc2-Update_ACO_Status. Use the following table as a guide to create the fields.</li>
			<table class="bordered stripe lined-columns lined-rows">
				<thead>
					<tr>
						<td>Name</td>
						<td>Type</td>
						<td>Cardinality</td>
						<td>Tags</td>
					</tr>
				</thead>
				<tbody>
					<tr>
						<td>name</td>
						<td>String</td>
						<td>1</td>
						<td>TRACK_ID</td>
					</tr>
					<tr>
						<td>status</td>
						<td>String</td>
						<td>1</td>
						<td></td>
					</tr>
				</tbody>
			</table>
			<li>Create a new GeoEvent Definition named Airc2-Update_Airspace_Alert. Use the following table as a guide to create the fields.</li>
			<table class="bordered stripe lined-columns lined-rows">
				<thead>
					<tr>
						<td>Name</td>
						<td>Type</td>
						<td>Cardinality</td>
						<td>Tags</td>
					</tr>
				</thead>
				<tbody>
					<tr>
						<td>callsign</td>
						<td>String</td>
						<td>1</td>
						<td>TRACK_ID</td>
					</tr>
					<tr>
						<td>lat</td>
						<td>Double</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>long</td>
						<td>Double</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>alt</td>
						<td>Double</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>alerttime</td>
						<td>DATE</td>
						<td>1</td>
						<td>TIME_START</td>
					</tr>
					<tr>
						<td>geometry</td>
						<td>Geometry</td>
						<td>1</td>
						<td>GEOMETRY</td>
					</tr>
				</tbody>
			</table>
			<li>Create a new GeoEvent Definition named Airc2-UpdateFeature-MilitaryAirTracks-FieldMapper. Use the following table as a guide to create the fields.</li>
			<table class="bordered stripe lined-columns lined-rows">
				<thead>
					<tr>
						<td>Name</td>
						<td>Type</td>
						<td>Cardinality</td>
						<td>Tags</td>
					</tr>
				</thead>
				<tbody>
					<tr>
						<td>uniquedesignation</td>
						<td>String</td>
						<td>1</td>
						<td>TRACK_ID</td>
					</tr>
					<tr>
						<td>x</td>
						<td>Double</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>y</td>
						<td>Double</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>z</td>
						<td>Double</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>datetimevalid</td>
						<td>DATE</td>
						<td>1</td>
						<td>TIME_START</td>
					</tr>
					<tr>
						<td>symbolid_2525d</td>
						<td>String</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>geometry</td>
						<td>Geometry</td>
						<td>1</td>
						<td>GEOMETRY</td>
					</tr>
				</tbody>
			</table>
						<li>Create a new GeoEvent Definition named Airc2-UpdateFeatureService-CivilianAirTracks-FieldMapper. Use the following table as a guide to create the fields.</li>
			<table class="bordered stripe lined-columns lined-rows">
				<thead>
					<tr>
						<td>Name</td>
						<td>Type</td>
						<td>Cardinality</td>
						<td>Tags</td>
					</tr>
				</thead>
				<tbody>
					<tr>
						<td>OID</td>
						<td>Integer</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>ident</td>
						<td>Integer</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>lat</td>
						<td>Double</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>lon</td>
						<td>Double</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>id</td>
						<td>String</td>
						<td>1</td>
						<td>TRACK_ID</td>
					</tr>
					<tr>
						<td>alt</td>
						<td>Double</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>gs</td>
						<td>Integer</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>time</td>
						<td>DATE</td>
						<td>1</td>
						<td>TIME_START</td>
					</tr>
					<tr>
						<td>heading</td>
						<td>Integer</td>
						<td>1</td>
						<td></td>
					</tr>
					<tr>
						<td>geometry</td>
						<td>Geometry</td>
						<td>1</td>
						<td>GEOMETRY</td>
					</tr>
				</tbody>
			</table>
		</ol>