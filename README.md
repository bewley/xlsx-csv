# xlsx-csv

1. Install xlsx2csv via sudo:

  sudo easy_install xlsx2csv
  
2. Navigate to folder containing xlsx files using cd

3. Run snippet:

  for i in *.xlsx;
   do
    filename=$(basename "$i" .xlsx);
    outext=".csv" 
    xlsx2csv $i $filename$outext
  done

4. Run csv concat:

  grep '' *.csv > heya.csv
