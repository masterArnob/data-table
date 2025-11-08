# data-table
## data table
```php
     <div class="table-responsive">
                    <table id="dataTableExample" class="table table-striped table-bordered">
                        <thead>
                            <tr>
                                <th>Name</th>
                                <th>Position</th>
                                <th>Office</th>
                                <th>Age</th>
                                <th>Start date</th>
                                <th>Salary</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td>{{ $loop->iteration }}</td>
                                <td>Accountant</td>
                                <td>Tokyo</td>
                                <td>33</td>
                                <td>2008/11/28</td>
                                <td>$162,700</td>
                            </tr>
                          
                          
                           
                         
                          
                     
                        </tbody>
                    </table>
                </div>
```




css link
```php
  <link rel="stylesheet" href="{{ asset('assets/datatable/datatables.net-bs5/dataTables.bootstrap5.css') }}">
```



script
```php
  <script src="{{ asset('assets/datatable/datatables.net/jquery.dataTables.js') }}"></script>
  <script src="{{ asset('assets/datatable/datatables.net-bs5/dataTables.bootstrap5.js') }}"></script>
  <script src="{{ asset('assets/datatable/data-table.js') }}"></script>
```


