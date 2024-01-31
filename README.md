How to put an icon on points that are in folders without having to do it one by one, in a KML?
I have this code that is correct as an example:

<?xml version="1.0" encoding="UTF-8"?>
<kml xmlns="http://www.opengis.net/kml/2.2" xmlns:gx="http://www.google.com/kml/ext/2.2" xmlns:kml="http://www.opengis.net/kml/2.2" xmlns:atom="http://www.w3.org/2005/Atom">
<Document>
	<name>ALL POINT.kmz</name>

	<open>1</open>
	<Schema name="latitd and longitud new Point Google Earth" id="S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
		<SimpleField type="int" name="Point_Number"><displayName>&lt;b&gt;Point Number&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="int" name="Northing"><displayName>&lt;b&gt;Northing&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="int" name="Easting"><displayName>&lt;b&gt;Easting&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="double" name="Latitude"><displayName>&lt;b&gt;Latitude&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="double" name="Longitude"><displayName>&lt;b&gt;Longitude&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="double" name="Elevation"><displayName>&lt;b&gt;Elevation&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="string" name="Full_Description"><displayName>&lt;b&gt;Full Description&lt;/b&gt;</displayName>
</SimpleField>
	</Schema>
	<Schema name="latitd and longitud new Point Google Earth" id="S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS0">
		<SimpleField type="int" name="Point_Number"><displayName>&lt;b&gt;Point Number&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="int" name="Northing"><displayName>&lt;b&gt;Northing&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="int" name="Easting"><displayName>&lt;b&gt;Easting&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="double" name="Latitude"><displayName>&lt;b&gt;Latitude&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="double" name="Longitude"><displayName>&lt;b&gt;Longitude&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="double" name="Elevation"><displayName>&lt;b&gt;Elevation&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="string" name="Full_Description"><displayName>&lt;b&gt;Full Description&lt;/b&gt;</displayName>
</SimpleField>
	</Schema>
	<Schema name="latitd and longitud new Point Google Earth" id="S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
		<SimpleField type="int" name="Point_Number"><displayName>&lt;b&gt;Point Number&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="int" name="Northing"><displayName>&lt;b&gt;Northing&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="int" name="Easting"><displayName>&lt;b&gt;Easting&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="double" name="Latitude"><displayName>&lt;b&gt;Latitude&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="double" name="Longitude"><displayName>&lt;b&gt;Longitude&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="double" name="Elevation"><displayName>&lt;b&gt;Elevation&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="string" name="Full_Description"><displayName>&lt;b&gt;Full Description&lt;/b&gt;</displayName>
</SimpleField>
	</Schema>
	<Style id="hlightPointStyle">
		<IconStyle>
			<scale>1.3</scale>
			<Icon>
				http://maps.google.com/mapfiles/kml/pushpin/ylw-pushpin.png
			</Icon>
			<hotSpot x="20" y="2" xunits="pixels" yunits="pixels"/>
		</IconStyle>
		<BalloonStyle>
			<text><![CDATA[<table border="0">
  <tr><td><b>Point Number</b></td><td>$[latitd and longitud new Point Google Earth/Point_Number]</td></tr>
  <tr><td><b>Northing</b></td><td>$[latitd and longitud new Point Google Earth/Northing]</td></tr>
  <tr><td><b>Easting</b></td><td>$[latitd and longitud new Point Google Earth/Easting]</td></tr>
  <tr><td><b>Latitude</b></td><td>$[latitd and longitud new Point Google Earth/Latitude]</td></tr>
  <tr><td><b>Longitude</b></td><td>$[latitd and longitud new Point Google Earth/Longitude]</td></tr>
  <tr><td><b>Elevation</b></td><td>$[latitd and longitud new Point Google Earth/Elevation]</td></tr>
  <tr><td><b>Full Description</b></td><td>$[latitd and longitud new Point Google Earth/Full_Description]</td></tr>
</table>]]></text>
		</BalloonStyle>
		<gx:IconStackStyle>
		</gx:IconStackStyle>
	</Style>
	<StyleMap id="msn_grn-pushpin">
		<Pair>
			<key>normal</key>
			<styleUrl>#sn_grn-pushpin</styleUrl>
		</Pair>
		<Pair>
			<key>highlight</key>
			<styleUrl>#sh_grn-pushpin</styleUrl>
		</Pair>
	</StyleMap>
	<StyleMap id="msn_pink-pushpin">
		<Pair>
			<key>normal</key>
			<styleUrl>#sn_pink-pushpin</styleUrl>
		</Pair>
		<Pair>
			<key>highlight</key>
			<styleUrl>#sh_pink-pushpin</styleUrl>
		</Pair>
	</StyleMap>
	<StyleMap id="msn_ylw-pushpin">
		<Pair>
			<key>normal</key>
			<styleUrl>#sn_ylw-pushpin</styleUrl>
		</Pair>
		<Pair>
			<key>highlight</key>
			<styleUrl>#sh_ylw-pushpin</styleUrl>
		</Pair>
	</StyleMap>
	<Style id="normPointStyle">
		<IconStyle>
			<scale>1.1</scale>
			<Icon>
				http://maps.google.com/mapfiles/kml/pushpin/ylw-pushpin.png
			</Icon>
			<hotSpot x="20" y="2" xunits="pixels" yunits="pixels"/>
		</IconStyle>
		<BalloonStyle>
			<text><![CDATA[<table border="0">
  <tr><td><b>Point Number</b></td><td>$[latitd and longitud new Point Google Earth/Point_Number]</td></tr>
  <tr><td><b>Northing</b></td><td>$[latitd and longitud new Point Google Earth/Northing]</td></tr>
  <tr><td><b>Easting</b></td><td>$[latitd and longitud new Point Google Earth/Easting]</td></tr>
  <tr><td><b>Latitude</b></td><td>$[latitd and longitud new Point Google Earth/Latitude]</td></tr>
  <tr><td><b>Longitude</b></td><td>$[latitd and longitud new Point Google Earth/Longitude]</td></tr>
  <tr><td><b>Elevation</b></td><td>$[latitd and longitud new Point Google Earth/Elevation]</td></tr>
  <tr><td><b>Full Description</b></td><td>$[latitd and longitud new Point Google Earth/Full_Description]</td></tr>
</table>]]></text>
		</BalloonStyle>
	</Style>
	<StyleMap id="pointStyleMap">
		<Pair>
			<key>normal</key>
			<styleUrl>#normPointStyle</styleUrl>
		</Pair>
		<Pair>
			<key>highlight</key>
			<styleUrl>#hlightPointStyle</styleUrl>
		</Pair>
	</StyleMap>
	
		<Style id="sn_grn-pushpin">
		<IconStyle>
			<scale>1.1</scale>
			<Icon>
				http://maps.google.com/mapfiles/kml/pushpin/grn-pushpin.png
			</Icon>
			<hotSpot x="20" y="2" xunits="pixels" yunits="pixels"/>
		</IconStyle>
	</Style>
	<Style id="sn_pink-pushpin">
		<IconStyle>
			<scale>1.1</scale>
			<Icon>
				http://maps.google.com/mapfiles/kml/pushpin/pink-pushpin.png
			</Icon>
			<hotSpot x="20" y="2" xunits="pixels" yunits="pixels"/>
		</IconStyle>
	 </Style>
	 <Folder>
		<name>Austing Dam embankment</name>
                       	<Placemark>
			<name>CPTU01</name>
			<styleUrl>#pointStyleMap</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">1</SimpleData>
					<SimpleData name="Northing">6252713</SimpleData>
					<SimpleData name="Easting">411958</SimpleData>
					<SimpleData name="Latitude">-33.8622</SimpleData>
					<SimpleData name="Longitude">116.048</SimpleData>
					<SimpleData name="Elevation">1256.8</SimpleData>
					<SimpleData name="Full_Description">CPTU01</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0481769702016,-33.86222112888441,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU01A</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">2</SimpleData>
					<SimpleData name="Northing">6252713</SimpleData>
					<SimpleData name="Easting">411958</SimpleData>
					<SimpleData name="Latitude">-33.8622</SimpleData>
					<SimpleData name="Longitude">116.048</SimpleData>
					<SimpleData name="Elevation">1256.8</SimpleData>
					<SimpleData name="Full_Description">CPTU01A</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0481769702016,-33.86222112888441,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU01B</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">3</SimpleData>
					<SimpleData name="Northing">6252713</SimpleData>
					<SimpleData name="Easting">411958</SimpleData>
					<SimpleData name="Latitude">-33.8622</SimpleData>
					<SimpleData name="Longitude">116.048</SimpleData>
					<SimpleData name="Elevation">1256.8</SimpleData>
					<SimpleData name="Full_Description">CPTU01B</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0481769702016,-33.86222112888441,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU01C</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">4</SimpleData>
					<SimpleData name="Northing">6252713</SimpleData>
					<SimpleData name="Easting">411958</SimpleData>
					<SimpleData name="Latitude">-33.8622</SimpleData>
					<SimpleData name="Longitude">116.048</SimpleData>
					<SimpleData name="Elevation">1256.8</SimpleData>
					<SimpleData name="Full_Description">CPTU01C</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0481769702016,-33.86222112888441,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU02</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">5</SimpleData>
					<SimpleData name="Northing">6252746</SimpleData>
					<SimpleData name="Easting">411865</SimpleData>
					<SimpleData name="Latitude">-33.8619</SimpleData>
					<SimpleData name="Longitude">116.047</SimpleData>
					<SimpleData name="Elevation">1256.7</SimpleData>
					<SimpleData name="Full_Description">CPTU02</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0471748734214,-33.86192478916671,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU03</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">6</SimpleData>
					<SimpleData name="Northing">6252783</SimpleData>
					<SimpleData name="Easting">411772</SimpleData>
					<SimpleData name="Latitude">-33.8616</SimpleData>
					<SimpleData name="Longitude">116.046</SimpleData>
					<SimpleData name="Elevation">1256.9</SimpleData>
					<SimpleData name="Full_Description">CPTU03</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0461625757863,-33.8615742505324,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU04</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">7</SimpleData>
					<SimpleData name="Northing">6252823</SimpleData>
					<SimpleData name="Easting">411660</SimpleData>
					<SimpleData name="Latitude">-33.8612</SimpleData>
					<SimpleData name="Longitude">116.045</SimpleData>
					<SimpleData name="Elevation">1256.9</SimpleData>
					<SimpleData name="Full_Description">CPTU04</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0449667247289,-33.8612042441832,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU05</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">8</SimpleData>
					<SimpleData name="Northing">6252855</SimpleData>
					<SimpleData name="Easting">411568</SimpleData>
					<SimpleData name="Latitude">-33.8609</SimpleData>
					<SimpleData name="Longitude">116.044</SimpleData>
					<SimpleData name="Elevation">1256.8</SimpleData>
					<SimpleData name="Full_Description">CPTU05</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0439646514822,-33.86090787871036,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU06</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">9</SimpleData>
					<SimpleData name="Northing">6252883</SimpleData>
					<SimpleData name="Easting">411490</SimpleData>
					<SimpleData name="Latitude">-33.8606</SimpleData>
					<SimpleData name="Longitude">116.043</SimpleData>
					<SimpleData name="Elevation">1256.5</SimpleData>
					<SimpleData name="Full_Description">CPTU06</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0431242246537,-33.86065785342509,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU07</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">10</SimpleData>
					<SimpleData name="Northing">6252702</SimpleData>
					<SimpleData name="Easting">411892</SimpleData>
					<SimpleData name="Latitude">-33.8623</SimpleData>
					<SimpleData name="Longitude">116.047</SimpleData>
					<SimpleData name="Elevation">1248</SimpleData>
					<SimpleData name="Full_Description">CPTU07</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.047451518361,-33.86232374799732,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU08</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">11</SimpleData>
					<SimpleData name="Northing">6252732</SimpleData>
					<SimpleData name="Easting">411836</SimpleData>
					<SimpleData name="Latitude">-33.862</SimpleData>
					<SimpleData name="Longitude">116.047</SimpleData>
					<SimpleData name="Elevation">1249.5</SimpleData>
					<SimpleData name="Full_Description">CPTU08</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0468491806221,-33.86204853188617,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU08A</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">12</SimpleData>
					<SimpleData name="Northing">6252732</SimpleData>
					<SimpleData name="Easting">411836</SimpleData>
					<SimpleData name="Latitude">-33.862</SimpleData>
					<SimpleData name="Longitude">116.047</SimpleData>
					<SimpleData name="Elevation">1249.5</SimpleData>
					<SimpleData name="Full_Description">CPTU08A</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0468491806221,-33.86204853188617,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU09</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">13</SimpleData>
					<SimpleData name="Northing">6252751</SimpleData>
					<SimpleData name="Easting">411784</SimpleData>
					<SimpleData name="Latitude">-33.8619</SimpleData>
					<SimpleData name="Longitude">116.046</SimpleData>
					<SimpleData name="Elevation">1250.1</SimpleData>
					<SimpleData name="Full_Description">CPTU09</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0462997921043,-33.86187292768602,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU09A</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">14</SimpleData>
					<SimpleData name="Northing">6252751</SimpleData>
					<SimpleData name="Easting">411784</SimpleData>
					<SimpleData name="Latitude">-33.8619</SimpleData>
					<SimpleData name="Longitude">116.046</SimpleData>
					<SimpleData name="Elevation">1250.1</SimpleData>
					<SimpleData name="Full_Description">CPTU09A</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0462997921043,-33.86187292768602,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU10</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">15</SimpleData>
					<SimpleData name="Northing">6252786</SimpleData>
					<SimpleData name="Easting">411704</SimpleData>
					<SimpleData name="Latitude">-33.8615</SimpleData>
					<SimpleData name="Longitude">116.045</SimpleData>
					<SimpleData name="Elevation">1250</SimpleData>
					<SimpleData name="Full_Description">CPTU10</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0454385322774,-33.86155060770329,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU10A</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">16</SimpleData>
					<SimpleData name="Northing">6252786</SimpleData>
					<SimpleData name="Easting">411704</SimpleData>
					<SimpleData name="Latitude">-33.8615</SimpleData>
					<SimpleData name="Longitude">116.045</SimpleData>
					<SimpleData name="Elevation">1250</SimpleData>
					<SimpleData name="Full_Description">CPTU10A</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0454385322774,-33.86155060770329,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU11</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">17</SimpleData>
					<SimpleData name="Northing">6252812</SimpleData>
					<SimpleData name="Easting">411622</SimpleData>
					<SimpleData name="Latitude">-33.8613</SimpleData>
					<SimpleData name="Longitude">116.045</SimpleData>
					<SimpleData name="Elevation">1250.8</SimpleData>
					<SimpleData name="Full_Description">CPTU11</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0445548563427,-33.86130025713284,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU12</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">18</SimpleData>
					<SimpleData name="Northing">6252855</SimpleData>
					<SimpleData name="Easting">411527</SimpleData>
					<SimpleData name="Latitude">-33.8609</SimpleData>
					<SimpleData name="Longitude">116.044</SimpleData>
					<SimpleData name="Elevation">1253</SimpleData>
					<SimpleData name="Full_Description">CPTU12</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0435213604105,-33.86091345802912,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU12A</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">19</SimpleData>
					<SimpleData name="Northing">6252855</SimpleData>
					<SimpleData name="Easting">411527</SimpleData>
					<SimpleData name="Latitude">-33.8609</SimpleData>
					<SimpleData name="Longitude">116.044</SimpleData>
					<SimpleData name="Elevation">1253</SimpleData>
					<SimpleData name="Full_Description">CPTU12A</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0435213604105,-33.86091345802912,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU13</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">20</SimpleData>
					<SimpleData name="Northing">6252920</SimpleData>
					<SimpleData name="Easting">411417</SimpleData>
					<SimpleData name="Latitude">-33.8603</SimpleData>
					<SimpleData name="Longitude">116.042</SimpleData>
					<SimpleData name="Elevation">1256.6</SimpleData>
					<SimpleData name="Full_Description">CPTU13</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0423497670089,-33.86030912995422,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU13A</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">21</SimpleData>
					<SimpleData name="Northing">6252920</SimpleData>
					<SimpleData name="Easting">411417</SimpleData>
					<SimpleData name="Latitude">-33.8603</SimpleData>
					<SimpleData name="Longitude">116.042</SimpleData>
					<SimpleData name="Elevation">1256.6</SimpleData>
					<SimpleData name="Full_Description">CPTU13A</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0423497670089,-33.86030912995422,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU14</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">22</SimpleData>
					<SimpleData name="Northing">6252968</SimpleData>
					<SimpleData name="Easting">411340</SimpleData>
					<SimpleData name="Latitude">-33.8599</SimpleData>
					<SimpleData name="Longitude">116.042</SimpleData>
					<SimpleData name="Elevation">1256.4</SimpleData>
					<SimpleData name="Full_Description">CPTU14</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0415113661992,-33.85987873662096,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU14A</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">23</SimpleData>
					<SimpleData name="Northing">6252968</SimpleData>
					<SimpleData name="Easting">411340</SimpleData>
					<SimpleData name="Latitude">-33.8599</SimpleData>
					<SimpleData name="Longitude">116.042</SimpleData>
					<SimpleData name="Elevation">1256.4</SimpleData>
					<SimpleData name="Full_Description">CPTU14A</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0415113661992,-33.85987873662096,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU15</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">24</SimpleData>
					<SimpleData name="Northing">6253046</SimpleData>
					<SimpleData name="Easting">411326</SimpleData>
					<SimpleData name="Latitude">-33.8592</SimpleData>
					<SimpleData name="Longitude">116.041</SimpleData>
					<SimpleData name="Elevation">1258.5</SimpleData>
					<SimpleData name="Full_Description">CPTU15</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0413788052408,-33.85916523281293,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU15A</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">25</SimpleData>
					<SimpleData name="Northing">6253046</SimpleData>
					<SimpleData name="Easting">411326</SimpleData>
					<SimpleData name="Latitude">-33.8592</SimpleData>
					<SimpleData name="Longitude">116.041</SimpleData>
					<SimpleData name="Elevation">1258.5</SimpleData>
					<SimpleData name="Full_Description">CPTU15A</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0413788052408,-33.85916523281293,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU15B</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">26</SimpleData>
					<SimpleData name="Northing">6253046</SimpleData>
					<SimpleData name="Easting">411326</SimpleData>
					<SimpleData name="Latitude">-33.8592</SimpleData>
					<SimpleData name="Longitude">116.041</SimpleData>
					<SimpleData name="Elevation">1258.5</SimpleData>
					<SimpleData name="Full_Description">CPTU15B</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0413788052408,-33.85916523281293,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU37A</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">28</SimpleData>
					<SimpleData name="Northing">6252718</SimpleData>
					<SimpleData name="Easting">411676</SimpleData>
					<SimpleData name="Latitude">-33.8622</SimpleData>
					<SimpleData name="Longitude">116.045</SimpleData>
					<SimpleData name="Elevation">1246.5</SimpleData>
					<SimpleData name="Full_Description">CPTU37A</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0451183275557,-33.86215237649003,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU38</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">29</SimpleData>
					<SimpleData name="Northing">6252685</SimpleData>
					<SimpleData name="Easting">411749</SimpleData>
					<SimpleData name="Latitude">-33.8625</SimpleData>
					<SimpleData name="Longitude">116.046</SimpleData>
					<SimpleData name="Elevation">1246.5</SimpleData>
					<SimpleData name="Full_Description">CPTU38</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0459149343483,-33.86245616096537,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU38A</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">30</SimpleData>
					<SimpleData name="Northing">6252685</SimpleData>
					<SimpleData name="Easting">411749</SimpleData>
					<SimpleData name="Latitude">-33.8625</SimpleData>
					<SimpleData name="Longitude">116.046</SimpleData>
					<SimpleData name="Elevation">1246.5</SimpleData>
					<SimpleData name="Full_Description">CPTU38A</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0459149343483,-33.86245616096537,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU39</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">31</SimpleData>
					<SimpleData name="Northing">6252660</SimpleData>
					<SimpleData name="Easting">411816</SimpleData>
					<SimpleData name="Latitude">-33.8627</SimpleData>
					<SimpleData name="Longitude">116.047</SimpleData>
					<SimpleData name="Elevation">1247.3</SimpleData>
					<SimpleData name="Full_Description">CPTU39</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0466366803698,-33.86268721212274,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>CPTU39A</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">32</SimpleData>
					<SimpleData name="Northing">6252660</SimpleData>
					<SimpleData name="Easting">411816</SimpleData>
					<SimpleData name="Latitude">-33.8627</SimpleData>
					<SimpleData name="Longitude">116.047</SimpleData>
					<SimpleData name="Elevation">1247.3</SimpleData>
					<SimpleData name="Full_Description">CPTU39A</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0466366803698,-33.86268721212274,0</coordinates>
			</Point>
		</Placemark>
		<Placemark>
			<name>SCPTU04A</name>
			<styleUrl>#msn_ylw-pushpin</styleUrl>
			<ExtendedData>
				<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS">
					<SimpleData name="Point_Number">33</SimpleData>
					<SimpleData name="Northing">6252826</SimpleData>
					<SimpleData name="Easting">411659</SimpleData>
					<SimpleData name="Latitude">-33.8612</SimpleData>
					<SimpleData name="Longitude">116.045</SimpleData>
					<SimpleData name="Elevation">1256.69</SimpleData>
					<SimpleData name="Full_Description">SCPTU04A</SimpleData>
				</SchemaData>
			</ExtendedData>
			<Point>
				<coordinates>116.0449454068092,-33.86117702305973,0</coordinates>
			</Point>
		</Placemark>
		<Folder>
			<name>GREEN</name>
			<Placemark>
				<name>CPTU16</name>
				<styleUrl>#msn_grn-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS0">
						<SimpleData name="Point_Number">34</SimpleData>
						<SimpleData name="Northing">6253122</SimpleData>
						<SimpleData name="Easting">411290</SimpleData>
						<SimpleData name="Latitude">-33.8585</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1259.6</SimpleData>
						<SimpleData name="Full_Description">CPTU16</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.040986422131,-33.85848578205454,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU16A</name>
				<styleUrl>#msn_grn-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS0">
						<SimpleData name="Point_Number">35</SimpleData>
						<SimpleData name="Northing">6253122</SimpleData>
						<SimpleData name="Easting">411290</SimpleData>
						<SimpleData name="Latitude">-33.8585</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1259.6</SimpleData>
						<SimpleData name="Full_Description">CPTU16A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.040986422131,-33.85848578205454,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU30A</name>
				<styleUrl>#msn_grn-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS0">
						<SimpleData name="Point_Number">36</SimpleData>
						<SimpleData name="Northing">6253388</SimpleData>
						<SimpleData name="Easting">411627</SimpleData>
						<SimpleData name="Latitude">-33.8561</SimpleData>
						<SimpleData name="Longitude">116.045</SimpleData>
						<SimpleData name="Elevation">1255.2</SimpleData>
						<SimpleData name="Full_Description">CPTU30A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0446667502751,-33.85610638307886,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU31</name>
				<styleUrl>#msn_grn-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS0">
						<SimpleData name="Point_Number">37</SimpleData>
						<SimpleData name="Northing">6253154</SimpleData>
						<SimpleData name="Easting">411390</SimpleData>
						<SimpleData name="Latitude">-33.8582</SimpleData>
						<SimpleData name="Longitude">116.042</SimpleData>
						<SimpleData name="Elevation">1257.4</SimpleData>
						<SimpleData name="Full_Description">CPTU31</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.042070565739,-33.85820561602463,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU31A</name>
				<styleUrl>#msn_grn-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS0">
						<SimpleData name="Point_Number">38</SimpleData>
						<SimpleData name="Northing">6253154</SimpleData>
						<SimpleData name="Easting">411390</SimpleData>
						<SimpleData name="Latitude">-33.8582</SimpleData>
						<SimpleData name="Longitude">116.042</SimpleData>
						<SimpleData name="Elevation">1257.4</SimpleData>
						<SimpleData name="Full_Description">CPTU31A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.042070565739,-33.85820561602463,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU32</name>
				<styleUrl>#msn_grn-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS0">
						<SimpleData name="Point_Number">39</SimpleData>
						<SimpleData name="Northing">6253190</SimpleData>
						<SimpleData name="Easting">411512</SimpleData>
						<SimpleData name="Latitude">-33.8579</SimpleData>
						<SimpleData name="Longitude">116.043</SimpleData>
						<SimpleData name="Elevation">1257.4</SimpleData>
						<SimpleData name="Full_Description">CPTU32</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0434038156521,-33.85788228071081,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU33</name>
				<styleUrl>#msn_grn-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS0">
						<SimpleData name="Point_Number">40</SimpleData>
						<SimpleData name="Northing">6253225</SimpleData>
						<SimpleData name="Easting">411568</SimpleData>
						<SimpleData name="Latitude">-33.8576</SimpleData>
						<SimpleData name="Longitude">116.044</SimpleData>
						<SimpleData name="Elevation">1257.8</SimpleData>
						<SimpleData name="Full_Description">CPTU33</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0440126448464,-33.85757135163637,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU33A</name>
				<styleUrl>#msn_grn-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS0">
						<SimpleData name="Point_Number">41</SimpleData>
						<SimpleData name="Northing">6253225</SimpleData>
						<SimpleData name="Easting">411568</SimpleData>
						<SimpleData name="Latitude">-33.8576</SimpleData>
						<SimpleData name="Longitude">116.044</SimpleData>
						<SimpleData name="Elevation">1257.8</SimpleData>
						<SimpleData name="Full_Description">CPTU33A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0440126448464,-33.85757135163637,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU36</name>
				<styleUrl>#msn_grn-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS0">
						<SimpleData name="Point_Number">42</SimpleData>
						<SimpleData name="Northing">6253414</SimpleData>
						<SimpleData name="Easting">412029</SimpleData>
						<SimpleData name="Latitude">-33.8559</SimpleData>
						<SimpleData name="Longitude">116.049</SimpleData>
						<SimpleData name="Elevation">1258.6</SimpleData>
						<SimpleData name="Full_Description">CPTU36</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0490144398745,-33.85591453715104,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU36A</name>
				<styleUrl>#msn_grn-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS0">
						<SimpleData name="Point_Number">43</SimpleData>
						<SimpleData name="Northing">6253414</SimpleData>
						<SimpleData name="Easting">412029</SimpleData>
						<SimpleData name="Latitude">-33.8559</SimpleData>
						<SimpleData name="Longitude">116.049</SimpleData>
						<SimpleData name="Elevation">1258.6</SimpleData>
						<SimpleData name="Full_Description">CPTU36A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0490144398745,-33.85591453715104,0</coordinates>
				</Point>
			</Placemark>
		</Folder>
		<Folder>
			<name>PURPLE</name>
			<Placemark>
				<name>CPTU17</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">44</SimpleData>
						<SimpleData name="Northing">6253152</SimpleData>
						<SimpleData name="Easting">411194</SimpleData>
						<SimpleData name="Latitude">-33.8582</SimpleData>
						<SimpleData name="Longitude">116.04</SimpleData>
						<SimpleData name="Elevation">1262.1</SimpleData>
						<SimpleData name="Full_Description">CPTU17</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0399626757098,-33.85819823435342,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU18</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">45</SimpleData>
						<SimpleData name="Northing">6253236</SimpleData>
						<SimpleData name="Easting">411244</SimpleData>
						<SimpleData name="Latitude">-33.8574</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1256.8</SimpleData>
						<SimpleData name="Full_Description">CPTU18</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0405115055645,-33.85745396039952,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU19</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">46</SimpleData>
						<SimpleData name="Northing">6253337</SimpleData>
						<SimpleData name="Easting">411264</SimpleData>
						<SimpleData name="Latitude">-33.8565</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1254.8</SimpleData>
						<SimpleData name="Full_Description">CPTU19</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0407378711133,-33.85654483900178,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU19A</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">47</SimpleData>
						<SimpleData name="Northing">6253337</SimpleData>
						<SimpleData name="Easting">411264</SimpleData>
						<SimpleData name="Latitude">-33.8565</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1254.8</SimpleData>
						<SimpleData name="Full_Description">CPTU19A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0407378711133,-33.85654483900178,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU20</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">48</SimpleData>
						<SimpleData name="Northing">6253389</SimpleData>
						<SimpleData name="Easting">411235</SimpleData>
						<SimpleData name="Latitude">-33.8561</SimpleData>
						<SimpleData name="Longitude">116.04</SimpleData>
						<SimpleData name="Elevation">1256</SimpleData>
						<SimpleData name="Full_Description">CPTU20</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0404297567359,-33.85606445239543,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU21</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">49</SimpleData>
						<SimpleData name="Northing">6253470</SimpleData>
						<SimpleData name="Easting">411242</SimpleData>
						<SimpleData name="Latitude">-33.8553</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1254.5</SimpleData>
						<SimpleData name="Full_Description">CPTU21</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0405134870437,-33.85534361233413,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU22</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">50</SimpleData>
						<SimpleData name="Northing">6253511</SimpleData>
						<SimpleData name="Easting">411299</SimpleData>
						<SimpleData name="Latitude">-33.855</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1254.5</SimpleData>
						<SimpleData name="Full_Description">CPTU22</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0411337215772,-33.8549786741679,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU23</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">51</SimpleData>
						<SimpleData name="Northing">6253540</SimpleData>
						<SimpleData name="Easting">411375</SimpleData>
						<SimpleData name="Latitude">-33.8547</SimpleData>
						<SimpleData name="Longitude">116.042</SimpleData>
						<SimpleData name="Elevation">1254.3</SimpleData>
						<SimpleData name="Full_Description">CPTU23</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0419472996098,-33.8547234595367,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU24</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">52</SimpleData>
						<SimpleData name="Northing">6253512</SimpleData>
						<SimpleData name="Easting">411482</SimpleData>
						<SimpleData name="Latitude">-33.855</SimpleData>
						<SimpleData name="Longitude">116.043</SimpleData>
						<SimpleData name="Elevation">1254.4</SimpleData>
						<SimpleData name="Full_Description">CPTU24</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0431119283517,-33.85497600972793,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU25</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">53</SimpleData>
						<SimpleData name="Northing">6253499</SimpleData>
						<SimpleData name="Easting">411256</SimpleData>
						<SimpleData name="Latitude">-33.8551</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1248.9</SimpleData>
						<SimpleData name="Full_Description">CPTU25</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0406678353817,-33.85507425423992,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU25A</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">54</SimpleData>
						<SimpleData name="Northing">6253499</SimpleData>
						<SimpleData name="Easting">411256</SimpleData>
						<SimpleData name="Latitude">-33.8551</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1248.9</SimpleData>
						<SimpleData name="Full_Description">CPTU25A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0406678353817,-33.85507425423992,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU26</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">55</SimpleData>
						<SimpleData name="Northing">6253529</SimpleData>
						<SimpleData name="Easting">411289</SimpleData>
						<SimpleData name="Latitude">-33.8548</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1247.5</SimpleData>
						<SimpleData name="Full_Description">CPTU26</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0410275489343,-33.85480649383967,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU27</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">56</SimpleData>
						<SimpleData name="Northing">6253552</SimpleData>
						<SimpleData name="Easting">411435</SimpleData>
						<SimpleData name="Latitude">-33.8546</SimpleData>
						<SimpleData name="Longitude">116.043</SimpleData>
						<SimpleData name="Elevation">1247.5</SimpleData>
						<SimpleData name="Full_Description">CPTU27</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0426079409773,-33.85461135012964,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU28</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">57</SimpleData>
						<SimpleData name="Northing">6253513</SimpleData>
						<SimpleData name="Easting">411543</SimpleData>
						<SimpleData name="Latitude">-33.855</SimpleData>
						<SimpleData name="Longitude">116.044</SimpleData>
						<SimpleData name="Elevation">1251.6</SimpleData>
						<SimpleData name="Full_Description">CPTU28</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0437605554822,-33.85497202471524,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU29</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">58</SimpleData>
						<SimpleData name="Northing">6253483</SimpleData>
						<SimpleData name="Easting">411609</SimpleData>
						<SimpleData name="Latitude">-33.8552</SimpleData>
						<SimpleData name="Longitude">116.044</SimpleData>
						<SimpleData name="Elevation">1255.2</SimpleData>
						<SimpleData name="Full_Description">CPTU29</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0444817307663,-33.85524817694997,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU29A</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">59</SimpleData>
						<SimpleData name="Northing">6253483</SimpleData>
						<SimpleData name="Easting">411609</SimpleData>
						<SimpleData name="Latitude">-33.8552</SimpleData>
						<SimpleData name="Longitude">116.044</SimpleData>
						<SimpleData name="Elevation">1255.2</SimpleData>
						<SimpleData name="Full_Description">CPTU29A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0444817307663,-33.85524817694997,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU30</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">60</SimpleData>
						<SimpleData name="Northing">6253388</SimpleData>
						<SimpleData name="Easting">411627</SimpleData>
						<SimpleData name="Latitude">-33.8561</SimpleData>
						<SimpleData name="Longitude">116.045</SimpleData>
						<SimpleData name="Elevation">1255.2</SimpleData>
						<SimpleData name="Full_Description">CPTU30</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0446667502751,-33.85610638307886,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU42</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">61</SimpleData>
						<SimpleData name="Northing">6253483</SimpleData>
						<SimpleData name="Easting">411653</SimpleData>
						<SimpleData name="Latitude">-33.8552</SimpleData>
						<SimpleData name="Longitude">116.045</SimpleData>
						<SimpleData name="Elevation">1255.8</SimpleData>
						<SimpleData name="Full_Description">CPTU42</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0449573186413,-33.85525186278894,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU43</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">62</SimpleData>
						<SimpleData name="Northing">6253486</SimpleData>
						<SimpleData name="Easting">411719</SimpleData>
						<SimpleData name="Latitude">-33.8552</SimpleData>
						<SimpleData name="Longitude">116.046</SimpleData>
						<SimpleData name="Elevation">1257.98</SimpleData>
						<SimpleData name="Full_Description">CPTU43</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0456710015323,-33.85523033447488,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU44</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">63</SimpleData>
						<SimpleData name="Northing">6253486</SimpleData>
						<SimpleData name="Easting">411789</SimpleData>
						<SimpleData name="Latitude">-33.8552</SimpleData>
						<SimpleData name="Longitude">116.046</SimpleData>
						<SimpleData name="Elevation">1257.4</SimpleData>
						<SimpleData name="Full_Description">CPTU44</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0464276187518,-33.85523619014514,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU44A</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">64</SimpleData>
						<SimpleData name="Northing">6253486</SimpleData>
						<SimpleData name="Easting">411789</SimpleData>
						<SimpleData name="Latitude">-33.8552</SimpleData>
						<SimpleData name="Longitude">116.046</SimpleData>
						<SimpleData name="Elevation">1257.4</SimpleData>
						<SimpleData name="Full_Description">CPTU44A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0464276187518,-33.85523619014514,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>SCPTU40</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">65</SimpleData>
						<SimpleData name="Northing">6253537</SimpleData>
						<SimpleData name="Easting">411355</SimpleData>
						<SimpleData name="Latitude">-33.8547</SimpleData>
						<SimpleData name="Longitude">116.042</SimpleData>
						<SimpleData name="Elevation">1254.05</SimpleData>
						<SimpleData name="Full_Description">SCPTU40</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0417417321202,-33.85473989889272,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>SCPTU41</name>
				<styleUrl>#msn_pink-pushpin</styleUrl>
				<ExtendedData>
					<SchemaData schemaUrl="#S_latitd_and_longitud_new_Point_Google_Earth_IIIDDDS1">
						<SimpleData name="Point_Number">66</SimpleData>
						<SimpleData name="Northing">6253516</SimpleData>
						<SimpleData name="Easting">411468</SimpleData>
						<SimpleData name="Latitude">-33.8549</SimpleData>
						<SimpleData name="Longitude">116.043</SimpleData>
						<SimpleData name="Elevation">1254.14</SimpleData>
						<SimpleData name="Full_Description">SCPTU41</SimpleData>
					</SchemaData>
				</ExtendedData>
				<gx:balloonVisibility>1</gx:balloonVisibility>
				<Point>
					<coordinates>116.0429610078526,-33.85493876341941,0</coordinates>
				</Point>
			</Placemark>
		</Folder>
	</Folder>
</Document>
</kml>

and I have mine, which always shows all the points with the same color of the icon, which is yellow, and I don't understand why the colors of the points are not changed as the correct example has.
<?xml version="1.0" encoding="UTF-8"?>
<kml xmlns="http://www.opengis.net/kml/2.2" xmlns:gx="http://www.google.com/kml/ext/2.2" xmlns:kml="http://www.opengis.net/kml/2.2" xmlns:atom="http://www.w3.org/2005/Atom">
<Document>
	<name>AGREGAMOS DESDE GOOGLE  EARTH CAPAS.kmz</name>
	<Schema name="all point Australia" id="S_all_point_Australia_IIIDDDS">
		<SimpleField type="int" name="Point_Number"><displayName>&lt;b&gt;Point Number&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="int" name="Northing"><displayName>&lt;b&gt;Northing&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="int" name="Easting"><displayName>&lt;b&gt;Easting&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="double" name="Latitude"><displayName>&lt;b&gt;Latitude&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="double" name="Longitude"><displayName>&lt;b&gt;Longitude&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="double" name="Elevation"><displayName>&lt;b&gt;Elevation&lt;/b&gt;</displayName>
</SimpleField>
		<SimpleField type="string" name="Full_Description"><displayName>&lt;b&gt;Full Description&lt;/b&gt;</displayName>
</SimpleField>
	</Schema>
	<Style id="hlightPointStyle">
		<IconStyle>
			<Icon>
				http://maps.google.com/mapfiles/kml/pushpin/ylw-pushpin.png
			</Icon>
		</IconStyle>
		<BalloonStyle>
			<text><![CDATA[<table border="0">
  <tr><td><b>Point Number</b></td><td>$[all point Australia/Point_Number]</td></tr>
  <tr><td><b>Northing</b></td><td>$[all point Australia/Northing]</td></tr>
  <tr><td><b>Easting</b></td><td>$[all point Australia/Easting]</td></tr>
  <tr><td><b>Latitude</b></td><td>$[all point Australia/Latitude]</td></tr>
  <tr><td><b>Longitude</b></td><td>$[all point Australia/Longitude]</td></tr>
  <tr><td><b>Elevation</b></td><td>$[all point Australia/Elevation]</td></tr>
  <tr><td><b>Full Description</b></td><td>$[all point Australia/Full_Description]</td></tr>
</table>]]></text>
		</BalloonStyle>
                <gx:IconStackStyle>
		</gx:IconStackStyle>
	</Style>
	<Style id="msn_grn-pushpin">
		<Pair>
			<key>normal</key>
			<styleUrl>#sn_grn-pushpin</styleUrl>
		</Pair>
		<Pair>
			<key>highlight</key>
			<styleUrl>#sh_grn-pushpin</styleUrl>
		</Pair>
	</Style>
	<Style id="msn_pink-pushpin">
		<Pair>
			<key>normal</key>
			<styleUrl>#sn_pink-pushpin</styleUrl>
		</Pair>
		<Pair>
			<key>highlight</key>
			<styleUrl>#sh_pink-pushpin</styleUrl>
		</Pair>
	</Style>
	<Style id="msn_ylw-pushpin">
		<Pair>
			<key>normal</key>
			<styleUrl>#sn_ylw-pushpin</styleUrl>
		</Pair>
		<Pair>
			<key>highlight</key>
			<styleUrl>#sh_ylw-pushpin</styleUrl>
		</Pair>
	</Style>
	<Style id="normPointStyle">
		<IconStyle>
			<scale>1.1</scale>
			<Icon>
				http://maps.google.com/mapfiles/kml/pushpin/ylw-pushpin.png
			</Icon>
			<hotSpot x="20" y="2" xunits="pixels" yunits="pixels"/>
		</IconStyle>
</Style>
	<Style id="sn_pink-pushpin">
		<IconStyle>
			<scale>1.1</scale>
			<Icon>
				http://maps.google.com/mapfiles/kml/pushpin/pink-pushpin.png
			</Icon>
			<hotSpot x="20" y="2" xunits="pixels" yunits="pixels"/>
		</IconStyle>
</Style>
<Style id="sn_grn-pushpin">
		<IconStyle>
			<scale>1.1</scale>
			<Icon>
				http://maps.google.com/mapfiles/kml/pushpin/grn-pushpin.png
			</Icon>
			<hotSpot x="20" y="2" xunits="pixels" yunits="pixels"/>
		</IconStyle>
		<BalloonStyle>
			<text><![CDATA[<table border="0">
  <tr><td><b>Point Number</b></td><td>$[all point Australia/Point_Number]</td></tr>
  <tr><td><b>Northing</b></td><td>$[all point Australia/Northing]</td></tr>
  <tr><td><b>Easting</b></td><td>$[all point Australia/Easting]</td></tr>
  <tr><td><b>Latitude</b></td><td>$[all point Australia/Latitude]</td></tr>
  <tr><td><b>Longitude</b></td><td>$[all point Australia/Longitude]</td></tr>
  <tr><td><b>Elevation</b></td><td>$[all point Australia/Elevation]</td></tr>
  <tr><td><b>Full Description</b></td><td>$[all point Australia/Full_Description]</td></tr>
</table>]]></text>
		</BalloonStyle>
	</Style>
	<StyleMap id="pointStyleMap">
		<Pair>
			<key>normal</key>
			<styleUrl>#normPointStyle</styleUrl>
		</Pair>
		<Pair>
			<key>highlight</key>
			<styleUrl>#hlightPointStyle</styleUrl>
		</Pair>
	</StyleMap>
        <Style id="sn_grn-pushpin">
		<IconStyle>
			<scale>1.1</scale>
			<Icon>
				http://maps.google.com/mapfiles/kml/pushpin/grn-pushpin.png
			</Icon>
			<hotSpot x="20" y="2" xunits="pixels" yunits="pixels"/>
		</IconStyle>
	</Style>
	<Style id="sn_pink-pushpin">
		<IconStyle>
			<scale>1.1</scale>
			<Icon>
				http://maps.google.com/mapfiles/kml/pushpin/pink-pushpin.png
			</Icon>
			<hotSpot x="20" y="2" xunits="pixels" yunits="pixels"/>
		</IconStyle>
	 </Style>
		<Folder>
		<name>Temporary Places</name>
		<open>1</open>
		<Folder>
			<name>Temporary Places</name>
			<open>1</open>
			<Document>
				<name>all point Australia.txt</name>
				<open>1</open>
				<Folder id="layer 0">
					<name>all point Australia</name>
					<open>1</open>
				</Folder>
			</Document>
		</Folder>
	        <Style id="sn_grn-pushpin">
		<IconStyle>
			<scale>1.1</scale>
			<Icon>
				http://maps.google.com/mapfiles/kml/pushpin/grn-pushpin.png
			</Icon>
			<hotSpot x="20" y="2" xunits="pixels" yunits="pixels"/>
		</IconStyle>
	</Style>
	<Style id="sn_pink-pushpin">
		<IconStyle>
			<scale>1.1</scale>
			<Icon>
				http://maps.google.com/mapfiles/kml/pushpin/pink-pushpin.png
			</Icon>
			<hotSpot x="20" y="2" xunits="pixels" yunits="pixels"/>
		</IconStyle>
	 </Style>
		<Folder>
			<name>GRUPO 1</name>
			<Placemark>
				<name>CPTU01</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">1</SimpleData>
						<SimpleData name="Northing">6252713</SimpleData>
						<SimpleData name="Easting">411958</SimpleData>
						<SimpleData name="Latitude">-33.8622</SimpleData>
						<SimpleData name="Longitude">116.048</SimpleData>
						<SimpleData name="Elevation">1256.8</SimpleData>
						<SimpleData name="Full_Description">CPTU01</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.048177,-33.86222100000001,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU01A</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">2</SimpleData>
						<SimpleData name="Northing">6252713</SimpleData>
						<SimpleData name="Easting">411958</SimpleData>
						<SimpleData name="Latitude">-33.8622</SimpleData>
						<SimpleData name="Longitude">116.048</SimpleData>
						<SimpleData name="Elevation">1256.8</SimpleData>
						<SimpleData name="Full_Description">CPTU01A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.048177,-33.86222100000001,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU01B</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">3</SimpleData>
						<SimpleData name="Northing">6252713</SimpleData>
						<SimpleData name="Easting">411958</SimpleData>
						<SimpleData name="Latitude">-33.8622</SimpleData>
						<SimpleData name="Longitude">116.048</SimpleData>
						<SimpleData name="Elevation">1256.8</SimpleData>
						<SimpleData name="Full_Description">CPTU01B</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.048177,-33.86222100000001,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU01C</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">4</SimpleData>
						<SimpleData name="Northing">6252713</SimpleData>
						<SimpleData name="Easting">411958</SimpleData>
						<SimpleData name="Latitude">-33.8622</SimpleData>
						<SimpleData name="Longitude">116.048</SimpleData>
						<SimpleData name="Elevation">1256.8</SimpleData>
						<SimpleData name="Full_Description">CPTU01C</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.048177,-33.86222100000001,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU02</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">5</SimpleData>
						<SimpleData name="Northing">6252746</SimpleData>
						<SimpleData name="Easting">411865</SimpleData>
						<SimpleData name="Latitude">-33.8619</SimpleData>
						<SimpleData name="Longitude">116.047</SimpleData>
						<SimpleData name="Elevation">1256.7</SimpleData>
						<SimpleData name="Full_Description">CPTU02</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.047175,-33.861916,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU03</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">6</SimpleData>
						<SimpleData name="Northing">6252783</SimpleData>
						<SimpleData name="Easting">411772</SimpleData>
						<SimpleData name="Latitude">-33.8616</SimpleData>
						<SimpleData name="Longitude">116.046</SimpleData>
						<SimpleData name="Elevation">1256.9</SimpleData>
						<SimpleData name="Full_Description">CPTU03</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.046173,-33.861574,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU04</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">7</SimpleData>
						<SimpleData name="Northing">6252823</SimpleData>
						<SimpleData name="Easting">411660</SimpleData>
						<SimpleData name="Latitude">-33.8612</SimpleData>
						<SimpleData name="Longitude">116.045</SimpleData>
						<SimpleData name="Elevation">1256.9</SimpleData>
						<SimpleData name="Full_Description">CPTU04</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.044967,-33.86120399999998,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU05</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">8</SimpleData>
						<SimpleData name="Northing">6252855</SimpleData>
						<SimpleData name="Easting">411568</SimpleData>
						<SimpleData name="Latitude">-33.8609</SimpleData>
						<SimpleData name="Longitude">116.044</SimpleData>
						<SimpleData name="Elevation">1256.8</SimpleData>
						<SimpleData name="Full_Description">CPTU05</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.043975,-33.86090799999999,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU06</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">9</SimpleData>
						<SimpleData name="Northing">6252883</SimpleData>
						<SimpleData name="Easting">411490</SimpleData>
						<SimpleData name="Latitude">-33.8606</SimpleData>
						<SimpleData name="Longitude">116.043</SimpleData>
						<SimpleData name="Elevation">1256.5</SimpleData>
						<SimpleData name="Full_Description">CPTU06</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.043135,-33.860649,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU07</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">10</SimpleData>
						<SimpleData name="Northing">6252702</SimpleData>
						<SimpleData name="Easting">411892</SimpleData>
						<SimpleData name="Latitude">-33.8623</SimpleData>
						<SimpleData name="Longitude">116.047</SimpleData>
						<SimpleData name="Elevation">1248</SimpleData>
						<SimpleData name="Full_Description">CPTU07</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.047462,-33.862315,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU08</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">11</SimpleData>
						<SimpleData name="Northing">6252732</SimpleData>
						<SimpleData name="Easting">411836</SimpleData>
						<SimpleData name="Latitude">-33.862</SimpleData>
						<SimpleData name="Longitude">116.047</SimpleData>
						<SimpleData name="Elevation">1249.5</SimpleData>
						<SimpleData name="Full_Description">CPTU08</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.04686,-33.86204000000001,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU08A</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">12</SimpleData>
						<SimpleData name="Northing">6252732</SimpleData>
						<SimpleData name="Easting">411836</SimpleData>
						<SimpleData name="Latitude">-33.862</SimpleData>
						<SimpleData name="Longitude">116.047</SimpleData>
						<SimpleData name="Elevation">1249.5</SimpleData>
						<SimpleData name="Full_Description">CPTU08A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.04686,-33.86204000000001,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU09</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">13</SimpleData>
						<SimpleData name="Northing">6252751</SimpleData>
						<SimpleData name="Easting">411784</SimpleData>
						<SimpleData name="Latitude">-33.8619</SimpleData>
						<SimpleData name="Longitude">116.046</SimpleData>
						<SimpleData name="Elevation">1250.1</SimpleData>
						<SimpleData name="Full_Description">CPTU09</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0463,-33.86186399999999,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU09A</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">14</SimpleData>
						<SimpleData name="Northing">6252751</SimpleData>
						<SimpleData name="Easting">411784</SimpleData>
						<SimpleData name="Latitude">-33.8619</SimpleData>
						<SimpleData name="Longitude">116.046</SimpleData>
						<SimpleData name="Elevation">1250.1</SimpleData>
						<SimpleData name="Full_Description">CPTU09A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.0463,-33.86186399999999,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU10</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">15</SimpleData>
						<SimpleData name="Northing">6252786</SimpleData>
						<SimpleData name="Easting">411704</SimpleData>
						<SimpleData name="Latitude">-33.8615</SimpleData>
						<SimpleData name="Longitude">116.045</SimpleData>
						<SimpleData name="Elevation">1250</SimpleData>
						<SimpleData name="Full_Description">CPTU10</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.045439,-33.86154199999999,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU10A</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">16</SimpleData>
						<SimpleData name="Northing">6252786</SimpleData>
						<SimpleData name="Easting">411704</SimpleData>
						<SimpleData name="Latitude">-33.8615</SimpleData>
						<SimpleData name="Longitude">116.045</SimpleData>
						<SimpleData name="Elevation">1250</SimpleData>
						<SimpleData name="Full_Description">CPTU10A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.045439,-33.86154199999999,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU11</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">17</SimpleData>
						<SimpleData name="Northing">6252812</SimpleData>
						<SimpleData name="Easting">411622</SimpleData>
						<SimpleData name="Latitude">-33.8613</SimpleData>
						<SimpleData name="Longitude">116.045</SimpleData>
						<SimpleData name="Elevation">1250.8</SimpleData>
						<SimpleData name="Full_Description">CPTU11</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.044555,-33.86130000000001,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU12</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">18</SimpleData>
						<SimpleData name="Northing">6252855</SimpleData>
						<SimpleData name="Easting">411527</SimpleData>
						<SimpleData name="Latitude">-33.8609</SimpleData>
						<SimpleData name="Longitude">116.044</SimpleData>
						<SimpleData name="Elevation">1253</SimpleData>
						<SimpleData name="Full_Description">CPTU12</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.043532,-33.860905,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU12A</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">19</SimpleData>
						<SimpleData name="Northing">6252855</SimpleData>
						<SimpleData name="Easting">411527</SimpleData>
						<SimpleData name="Latitude">-33.8609</SimpleData>
						<SimpleData name="Longitude">116.044</SimpleData>
						<SimpleData name="Elevation">1253</SimpleData>
						<SimpleData name="Full_Description">CPTU12A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.043532,-33.860905,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU13</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">20</SimpleData>
						<SimpleData name="Northing">6252920</SimpleData>
						<SimpleData name="Easting">411417</SimpleData>
						<SimpleData name="Latitude">-33.8603</SimpleData>
						<SimpleData name="Longitude">116.042</SimpleData>
						<SimpleData name="Elevation">1256.6</SimpleData>
						<SimpleData name="Full_Description">CPTU13</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.04235,-33.86030900000001,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU13A</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">21</SimpleData>
						<SimpleData name="Northing">6252920</SimpleData>
						<SimpleData name="Easting">411417</SimpleData>
						<SimpleData name="Latitude">-33.8603</SimpleData>
						<SimpleData name="Longitude">116.042</SimpleData>
						<SimpleData name="Elevation">1256.6</SimpleData>
						<SimpleData name="Full_Description">CPTU13A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.04235,-33.86030900000001,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU14</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">22</SimpleData>
						<SimpleData name="Northing">6252968</SimpleData>
						<SimpleData name="Easting">411340</SimpleData>
						<SimpleData name="Latitude">-33.8599</SimpleData>
						<SimpleData name="Longitude">116.042</SimpleData>
						<SimpleData name="Elevation">1256.4</SimpleData>
						<SimpleData name="Full_Description">CPTU14</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.041522,-33.85986999999999,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU14A</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">23</SimpleData>
						<SimpleData name="Northing">6252968</SimpleData>
						<SimpleData name="Easting">411340</SimpleData>
						<SimpleData name="Latitude">-33.8599</SimpleData>
						<SimpleData name="Longitude">116.042</SimpleData>
						<SimpleData name="Elevation">1256.4</SimpleData>
						<SimpleData name="Full_Description">CPTU14A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.041522,-33.85986999999999,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU15</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">24</SimpleData>
						<SimpleData name="Northing">6253046</SimpleData>
						<SimpleData name="Easting">411326</SimpleData>
						<SimpleData name="Latitude">-33.8592</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1258.5</SimpleData>
						<SimpleData name="Full_Description">CPTU15</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.041379,-33.859165,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU15A</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">25</SimpleData>
						<SimpleData name="Northing">6253046</SimpleData>
						<SimpleData name="Easting">411326</SimpleData>
						<SimpleData name="Latitude">-33.8592</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1258.5</SimpleData>
						<SimpleData name="Full_Description">CPTU15A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.041379,-33.859165,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU15B</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">26</SimpleData>
						<SimpleData name="Northing">6253046</SimpleData>
						<SimpleData name="Easting">411326</SimpleData>
						<SimpleData name="Latitude">-33.8592</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1258.5</SimpleData>
						<SimpleData name="Full_Description">CPTU15B</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.041379,-33.859165,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU37</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">27</SimpleData>
						<SimpleData name="Northing">6252718</SimpleData>
						<SimpleData name="Easting">411676</SimpleData>
						<SimpleData name="Latitude">-33.8622</SimpleData>
						<SimpleData name="Longitude">116.045</SimpleData>
						<SimpleData name="Elevation">1246.5</SimpleData>
						<SimpleData name="Full_Description">CPTU37</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.045129,-33.862152,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU37A</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">28</SimpleData>
						<SimpleData name="Northing">6252718</SimpleData>
						<SimpleData name="Easting">411676</SimpleData>
						<SimpleData name="Latitude">-33.8622</SimpleData>
						<SimpleData name="Longitude">116.045</SimpleData>
						<SimpleData name="Elevation">1246.5</SimpleData>
						<SimpleData name="Full_Description">CPTU37A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.045129,-33.862152,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU38</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">29</SimpleData>
						<SimpleData name="Northing">6252685</SimpleData>
						<SimpleData name="Easting">411749</SimpleData>
						<SimpleData name="Latitude">-33.8625</SimpleData>
						<SimpleData name="Longitude">116.046</SimpleData>
						<SimpleData name="Elevation">1246.5</SimpleData>
						<SimpleData name="Full_Description">CPTU38</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.045915,-33.86245600000002,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU38A</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">30</SimpleData>
						<SimpleData name="Northing">6252685</SimpleData>
						<SimpleData name="Easting">411749</SimpleData>
						<SimpleData name="Latitude">-33.8625</SimpleData>
						<SimpleData name="Longitude">116.046</SimpleData>
						<SimpleData name="Elevation">1246.5</SimpleData>
						<SimpleData name="Full_Description">CPTU38A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.045915,-33.86245600000002,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU39</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">31</SimpleData>
						<SimpleData name="Northing">6252660</SimpleData>
						<SimpleData name="Easting">411816</SimpleData>
						<SimpleData name="Latitude">-33.8627</SimpleData>
						<SimpleData name="Longitude">116.047</SimpleData>
						<SimpleData name="Elevation">1247.3</SimpleData>
						<SimpleData name="Full_Description">CPTU39</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.046637,-33.862687,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU39A</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">32</SimpleData>
						<SimpleData name="Northing">6252660</SimpleData>
						<SimpleData name="Easting">411816</SimpleData>
						<SimpleData name="Latitude">-33.8627</SimpleData>
						<SimpleData name="Longitude">116.047</SimpleData>
						<SimpleData name="Elevation">1247.3</SimpleData>
						<SimpleData name="Full_Description">CPTU39A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.046637,-33.862687,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>SCPTU04A</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">33</SimpleData>
						<SimpleData name="Northing">6252826</SimpleData>
						<SimpleData name="Easting">411659</SimpleData>
						<SimpleData name="Latitude">-33.8612</SimpleData>
						<SimpleData name="Longitude">116.045</SimpleData>
						<SimpleData name="Elevation">1256.69</SimpleData>
						<SimpleData name="Full_Description">SCPTU04A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.044956,-33.861177,0</coordinates>
				</Point>
			</Placemark>
		</Folder>
		<Folder>
			<name>GRUPO 2</name>
			<Placemark>
				<name>CPTU16</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">34</SimpleData>
						<SimpleData name="Northing">6253122</SimpleData>
						<SimpleData name="Easting">411290</SimpleData>
						<SimpleData name="Latitude">-33.8585</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1259.6</SimpleData>
						<SimpleData name="Full_Description">CPTU16</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.040997,-33.85847699999999,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU16A</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">35</SimpleData>
						<SimpleData name="Northing">6253122</SimpleData>
						<SimpleData name="Easting">411290</SimpleData>
						<SimpleData name="Latitude">-33.8585</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1259.6</SimpleData>
						<SimpleData name="Full_Description">CPTU16A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.040997,-33.85847699999999,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU30A</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">36</SimpleData>
						<SimpleData name="Northing">6253388</SimpleData>
						<SimpleData name="Easting">411627</SimpleData>
						<SimpleData name="Latitude">-33.8561</SimpleData>
						<SimpleData name="Longitude">116.045</SimpleData>
						<SimpleData name="Elevation">1255.2</SimpleData>
						<SimpleData name="Full_Description">CPTU30A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.044667,-33.85610600000001,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU31</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">37</SimpleData>
						<SimpleData name="Northing">6253154</SimpleData>
						<SimpleData name="Easting">411390</SimpleData>
						<SimpleData name="Latitude">-33.8582</SimpleData>
						<SimpleData name="Longitude">116.042</SimpleData>
						<SimpleData name="Elevation">1257.4</SimpleData>
						<SimpleData name="Full_Description">CPTU31</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.042081,-33.85819699999998,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU31A</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">38</SimpleData>
						<SimpleData name="Northing">6253154</SimpleData>
						<SimpleData name="Easting">411390</SimpleData>
						<SimpleData name="Latitude">-33.8582</SimpleData>
						<SimpleData name="Longitude">116.042</SimpleData>
						<SimpleData name="Elevation">1257.4</SimpleData>
						<SimpleData name="Full_Description">CPTU31A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.042081,-33.85819699999998,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU32</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">39</SimpleData>
						<SimpleData name="Northing">6253190</SimpleData>
						<SimpleData name="Easting">411512</SimpleData>
						<SimpleData name="Latitude">-33.8579</SimpleData>
						<SimpleData name="Longitude">116.043</SimpleData>
						<SimpleData name="Elevation">1257.4</SimpleData>
						<SimpleData name="Full_Description">CPTU32</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.043404,-33.857882,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU33</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">40</SimpleData>
						<SimpleData name="Northing">6253225</SimpleData>
						<SimpleData name="Easting">411568</SimpleData>
						<SimpleData name="Latitude">-33.8576</SimpleData>
						<SimpleData name="Longitude">116.044</SimpleData>
						<SimpleData name="Elevation">1257.8</SimpleData>
						<SimpleData name="Full_Description">CPTU33</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.044013,-33.85757100000001,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU33A</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">41</SimpleData>
						<SimpleData name="Northing">6253225</SimpleData>
						<SimpleData name="Easting">411568</SimpleData>
						<SimpleData name="Latitude">-33.8576</SimpleData>
						<SimpleData name="Longitude">116.044</SimpleData>
						<SimpleData name="Elevation">1257.8</SimpleData>
						<SimpleData name="Full_Description">CPTU33A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.044013,-33.85757100000001,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU36</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">42</SimpleData>
						<SimpleData name="Northing">6253414</SimpleData>
						<SimpleData name="Easting">412029</SimpleData>
						<SimpleData name="Latitude">-33.8559</SimpleData>
						<SimpleData name="Longitude">116.049</SimpleData>
						<SimpleData name="Elevation">1258.6</SimpleData>
						<SimpleData name="Full_Description">CPTU36</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.049015,-33.85590600000001,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU36A</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">43</SimpleData>
						<SimpleData name="Northing">6253414</SimpleData>
						<SimpleData name="Easting">412029</SimpleData>
						<SimpleData name="Latitude">-33.8559</SimpleData>
						<SimpleData name="Longitude">116.049</SimpleData>
						<SimpleData name="Elevation">1258.6</SimpleData>
						<SimpleData name="Full_Description">CPTU36A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.049015,-33.85590600000001,0</coordinates>
				</Point>
			</Placemark>
		</Folder>
		<Folder>
			<name>GRUPO 3</name>
			<Placemark>
				<name>CPTU17</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">44</SimpleData>
						<SimpleData name="Northing">6253152</SimpleData>
						<SimpleData name="Easting">411194</SimpleData>
						<SimpleData name="Latitude">-33.8582</SimpleData>
						<SimpleData name="Longitude">116.04</SimpleData>
						<SimpleData name="Elevation">1262.1</SimpleData>
						<SimpleData name="Full_Description">CPTU17</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.039963,-33.85819800000002,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU18</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">45</SimpleData>
						<SimpleData name="Northing">6253236</SimpleData>
						<SimpleData name="Easting">411244</SimpleData>
						<SimpleData name="Latitude">-33.8574</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1256.8</SimpleData>
						<SimpleData name="Full_Description">CPTU18</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.040512,-33.85744499999999,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU19</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">46</SimpleData>
						<SimpleData name="Northing">6253337</SimpleData>
						<SimpleData name="Easting">411264</SimpleData>
						<SimpleData name="Latitude">-33.8565</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1254.8</SimpleData>
						<SimpleData name="Full_Description">CPTU19</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.040738,-33.856536,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU19A</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">47</SimpleData>
						<SimpleData name="Northing">6253337</SimpleData>
						<SimpleData name="Easting">411264</SimpleData>
						<SimpleData name="Latitude">-33.8565</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1254.8</SimpleData>
						<SimpleData name="Full_Description">CPTU19A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.040738,-33.856536,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU20</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">48</SimpleData>
						<SimpleData name="Northing">6253389</SimpleData>
						<SimpleData name="Easting">411235</SimpleData>
						<SimpleData name="Latitude">-33.8561</SimpleData>
						<SimpleData name="Longitude">116.04</SimpleData>
						<SimpleData name="Elevation">1256</SimpleData>
						<SimpleData name="Full_Description">CPTU20</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.04043,-33.856064,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU21</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">49</SimpleData>
						<SimpleData name="Northing">6253470</SimpleData>
						<SimpleData name="Easting">411242</SimpleData>
						<SimpleData name="Latitude">-33.8553</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1254.5</SimpleData>
						<SimpleData name="Full_Description">CPTU21</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.040514,-33.85533499999999,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU22</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">50</SimpleData>
						<SimpleData name="Northing">6253511</SimpleData>
						<SimpleData name="Easting">411299</SimpleData>
						<SimpleData name="Latitude">-33.855</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1254.5</SimpleData>
						<SimpleData name="Full_Description">CPTU22</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.041134,-33.85497,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU23</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">51</SimpleData>
						<SimpleData name="Northing">6253540</SimpleData>
						<SimpleData name="Easting">411375</SimpleData>
						<SimpleData name="Latitude">-33.8547</SimpleData>
						<SimpleData name="Longitude">116.042</SimpleData>
						<SimpleData name="Elevation">1254.3</SimpleData>
						<SimpleData name="Full_Description">CPTU23</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.041958,-33.85471500000001,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU24</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">52</SimpleData>
						<SimpleData name="Northing">6253512</SimpleData>
						<SimpleData name="Easting">411482</SimpleData>
						<SimpleData name="Latitude">-33.855</SimpleData>
						<SimpleData name="Longitude">116.043</SimpleData>
						<SimpleData name="Elevation">1254.4</SimpleData>
						<SimpleData name="Full_Description">CPTU24</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.043112,-33.854976,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU25</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">53</SimpleData>
						<SimpleData name="Northing">6253499</SimpleData>
						<SimpleData name="Easting">411256</SimpleData>
						<SimpleData name="Latitude">-33.8551</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1248.9</SimpleData>
						<SimpleData name="Full_Description">CPTU25</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.040668,-33.85507399999999,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU25A</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">54</SimpleData>
						<SimpleData name="Northing">6253499</SimpleData>
						<SimpleData name="Easting">411256</SimpleData>
						<SimpleData name="Latitude">-33.8551</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1248.9</SimpleData>
						<SimpleData name="Full_Description">CPTU25A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.040668,-33.85507399999999,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU26</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">55</SimpleData>
						<SimpleData name="Northing">6253529</SimpleData>
						<SimpleData name="Easting">411289</SimpleData>
						<SimpleData name="Latitude">-33.8548</SimpleData>
						<SimpleData name="Longitude">116.041</SimpleData>
						<SimpleData name="Elevation">1247.5</SimpleData>
						<SimpleData name="Full_Description">CPTU26</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.041028,-33.854806,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU27</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">56</SimpleData>
						<SimpleData name="Northing">6253552</SimpleData>
						<SimpleData name="Easting">411435</SimpleData>
						<SimpleData name="Latitude">-33.8546</SimpleData>
						<SimpleData name="Longitude">116.043</SimpleData>
						<SimpleData name="Elevation">1247.5</SimpleData>
						<SimpleData name="Full_Description">CPTU27</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.042608,-33.854611,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU28</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">57</SimpleData>
						<SimpleData name="Northing">6253513</SimpleData>
						<SimpleData name="Easting">411543</SimpleData>
						<SimpleData name="Latitude">-33.855</SimpleData>
						<SimpleData name="Longitude">116.044</SimpleData>
						<SimpleData name="Elevation">1251.6</SimpleData>
						<SimpleData name="Full_Description">CPTU28</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.043771,-33.85497200000001,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU29</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">58</SimpleData>
						<SimpleData name="Northing">6253483</SimpleData>
						<SimpleData name="Easting">411609</SimpleData>
						<SimpleData name="Latitude">-33.8552</SimpleData>
						<SimpleData name="Longitude">116.044</SimpleData>
						<SimpleData name="Elevation">1255.2</SimpleData>
						<SimpleData name="Full_Description">CPTU29</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.044482,-33.85524800000002,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU29A</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">59</SimpleData>
						<SimpleData name="Northing">6253483</SimpleData>
						<SimpleData name="Easting">411609</SimpleData>
						<SimpleData name="Latitude">-33.8552</SimpleData>
						<SimpleData name="Longitude">116.044</SimpleData>
						<SimpleData name="Elevation">1255.2</SimpleData>
						<SimpleData name="Full_Description">CPTU29A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.044482,-33.85524800000002,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU30</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">60</SimpleData>
						<SimpleData name="Northing">6253388</SimpleData>
						<SimpleData name="Easting">411627</SimpleData>
						<SimpleData name="Latitude">-33.8561</SimpleData>
						<SimpleData name="Longitude">116.045</SimpleData>
						<SimpleData name="Elevation">1255.2</SimpleData>
						<SimpleData name="Full_Description">CPTU30</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.044667,-33.85610600000001,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU42</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">61</SimpleData>
						<SimpleData name="Northing">6253483</SimpleData>
						<SimpleData name="Easting">411653</SimpleData>
						<SimpleData name="Latitude">-33.8552</SimpleData>
						<SimpleData name="Longitude">116.045</SimpleData>
						<SimpleData name="Elevation">1255.8</SimpleData>
						<SimpleData name="Full_Description">CPTU42</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.044965,-33.85525000000001,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU43</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">62</SimpleData>
						<SimpleData name="Northing">6253486</SimpleData>
						<SimpleData name="Easting">411719</SimpleData>
						<SimpleData name="Latitude">-33.8552</SimpleData>
						<SimpleData name="Longitude">116.046</SimpleData>
						<SimpleData name="Elevation">1257.98</SimpleData>
						<SimpleData name="Full_Description">CPTU43</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.04568,-33.855224,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU44</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">63</SimpleData>
						<SimpleData name="Northing">6253486</SimpleData>
						<SimpleData name="Easting">411789</SimpleData>
						<SimpleData name="Latitude">-33.8552</SimpleData>
						<SimpleData name="Longitude">116.046</SimpleData>
						<SimpleData name="Elevation">1257.4</SimpleData>
						<SimpleData name="Full_Description">CPTU44</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.046436,-33.85523000000001,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>CPTU44A</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">64</SimpleData>
						<SimpleData name="Northing">6253486</SimpleData>
						<SimpleData name="Easting">411789</SimpleData>
						<SimpleData name="Latitude">-33.8552</SimpleData>
						<SimpleData name="Longitude">116.046</SimpleData>
						<SimpleData name="Elevation">1257.4</SimpleData>
						<SimpleData name="Full_Description">CPTU44A</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.046436,-33.85523000000001,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>SCPTU40</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">65</SimpleData>
						<SimpleData name="Northing">6253537</SimpleData>
						<SimpleData name="Easting">411355</SimpleData>
						<SimpleData name="Latitude">-33.8547</SimpleData>
						<SimpleData name="Longitude">116.042</SimpleData>
						<SimpleData name="Elevation">1254.05</SimpleData>
						<SimpleData name="Full_Description">SCPTU40</SimpleData>
					</SchemaData>
				</ExtendedData>
				<Point>
					<coordinates>116.041746,-33.85473200000001,0</coordinates>
				</Point>
			</Placemark>
			<Placemark>
				<name>SCPTU41</name>
				<styleUrl>#pointStyleMap</styleUrl>
				<Style id="inline">
					<IconStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</IconStyle>
					<LineStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</LineStyle>
					<PolyStyle>
						<color>ffffffff</color>
						<colorMode>normal</colorMode>
					</PolyStyle>
				</Style>
				<ExtendedData>
					<SchemaData schemaUrl="#S_all_point_Australia_IIIDDDS">
						<SimpleData name="Point_Number">66</SimpleData>
						<SimpleData name="Northing">6253516</SimpleData>
						<SimpleData name="Easting">411468</SimpleData>
						<SimpleData name="Latitude">-33.8549</SimpleData>
						<SimpleData name="Longitude">116.043</SimpleData>
						<SimpleData name="Elevation">1254.14</SimpleData>
						<SimpleData name="Full_Description">SCPTU41</SimpleData>
					</SchemaData>
				</ExtendedData>
				<gx:balloonVisibility>1</gx:balloonVisibility>
				<Point>
					<coordinates>116.042971,-33.85493400000002,0</coordinates>
				</Point>
			</Placemark>
		</Folder>
	</Folder>
</Document>
</kml>
Can someone help me and send me the correct code and show me where my error is, and how to put the colors to each point with its corresponding folder. I would thank you a lot.








