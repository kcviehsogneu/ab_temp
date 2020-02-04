<head>
<script
  src="https://code.jquery.com/jquery-3.4.1.min.js"
  integrity="sha256-CSXorXvZcTkaix6Yvo6HppcZGetbYMGWSFlBw8HfCJo="
  crossorigin="anonymous"></script>
<link rel="stylesheet" type="text/css" href="//cdn.datatables.net/1.10.13/css/jquery.dataTables.css">
<script type="text/javascript" language="javascript" src="https://code.jquery.com/jquery-3.3.1.js"></script>
<script type="text/javascript" language="javascript" src="https://cdn.datatables.net/1.10.20/js/jquery.dataTables.min.js"></script>
<script type="text/javascript" language="javascript" src="https://cdn.datatables.net/buttons/1.6.1/js/dataTables.buttons.min.js"></script>
<script type="text/javascript" language="javascript" src="https://cdnjs.cloudflare.com/ajax/libs/jszip/3.1.3/jszip.min.js"></script>
<script type="text/javascript" language="javascript" src="https://cdnjs.cloudflare.com/ajax/libs/pdfmake/0.1.53/pdfmake.min.js"></script>
<script type="text/javascript" language="javascript" src="https://cdnjs.cloudflare.com/ajax/libs/pdfmake/0.1.53/vfs_fonts.js"></script>
<script type="text/javascript" language="javascript" src="https://cdn.datatables.net/buttons/1.6.1/js/buttons.html5.min.js"></script>
<script type="text/javascript" charset="utf8" src="//cdn.datatables.net/1.10.20/js/jquery.dataTables.min.js"></script>
<script>

  $(document).ready(function() {
      $('#dogs').DataTable( {
      	"dom": 'Bfrtip',
        "buttons": ['copyHtml5',
            'excelHtml5',
            'csvHtml5',
            'pdfHtml5'],
  	"ajax": "dogs.json",
  	"columnDefs": [ {
		"type": "ratings",
      		"targets": -4
        } ]
      } );
  } );
  </script>
  <script>
  $.fn.dataTable.ext.type.order['ratings-pre'] = function ( d ) {
    switch ( d ) {
        case 'Low':    return 1;
        case 'Medium': return 2;
        case 'High':   return 3;
    }
    return 0;
  };
  $(document).ready(function() {
      $('#cats').DataTable( {
          "ajax": "cats.json",
	  "columnDefs": [ {
	      "type": "ratings",
	      "targets": -5
        } ]
      } );
  } );
  </script>
</head>



<h2>Antimicrobial Usage for Dogs in Australia</h2>


<table id="dogs" class="display" style="width:100%">
        <thead>
            <tr>
		<th>Rank</th>
                <th>Ingredient</th>
		<th>Drug Class</th>
		<th>ASTAG Rating</th>
                <th>WHO Rating</th>
                <th>System Antimicrobial Consults (%)</th>
                <th>Topical Antimicrobial Consults (%)</th>
            </tr>
        </thead>
        <tfoot>
            <tr>
		<th>Rank</th>
                <th>Ingredient</th>
		<th>ASTAG Rating</th>
                <th>Drug Class</th>
                <th>WHO Rating</th>
                <th>System Antimicrobial Consults (%)</th>
                <th>Topical Antimicrobial Consults (%)</th>
            </tr>
        </tfoot>
 </table>
 
 <h2>Antimicrobial Usage for Cats in Australia</h2>
 
 <table id="cats" class="display" style="width:100%">
        <thead>
            <tr>
		<th>Rank</th>
                <th>Ingredient</th>
		<th>Drug Class</th>
		<th>ASTAG Rating</th>
                <th>WHO Rating</th>
                <th>System Antimicrobial Consults (%)</th>
                <th>Topical Antimicrobial Consults (%)</th>
            </tr>
        </thead>
        <tfoot>
            <tr>
		<th>Rank</th>
                <th>Ingredient</th>
		<th>Drug Class</th>
                <th>ASTAG Rating</th>
                <th>WHO Rating</th>
                <th>System Antimicrobial Consults (%)</th>
                <th>Topical Antimicrobial Consults (%)</th>
            </tr>
        </tfoot>
 </table>

