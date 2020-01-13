<head>
<script
  src="https://code.jquery.com/jquery-3.4.1.min.js"
  integrity="sha256-CSXorXvZcTkaix6Yvo6HppcZGetbYMGWSFlBw8HfCJo="
  crossorigin="anonymous"></script>
  <link rel="stylesheet" type="text/css" href="//cdn.datatables.net/1.10.13/css/jquery.dataTables.css">
  <script type="text/javascript" charset="utf8" src="//cdn.datatables.net/1.10.20/js/jquery.dataTables.min.js"></script>
  <script>
  $(document).ready(function() {
      $('#dogs').DataTable( {
          "ajax": "dogs.json"
      } );
  } );
  </script>
  <script>
  $(document).ready(function() {
      $('#cats').DataTable( {
          "ajax": "cats.json"
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
		<th>Drug Class</th>
                <th>ASTAG Rating</th>
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

