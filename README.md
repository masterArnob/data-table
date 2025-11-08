# data-table
## data table
```php
      <div class="table-responsive">
                    <table id="dataTableExample" class="table table-striped table-bordered">
                        <thead>
                            <tr>
                                <th>Name</th>
                                <th>Thumb Image</th>
                                <th>Admin ID</th>
                                <th>Action</th>
                            </tr>
                        </thead>
                        <tbody>
                           
                            @forelse ($products as $item)
                                <tr>
                                    <td>{{ $item->name }}</td>
                                    <td>{{ $item->thumb_image }}</td>
                                    <td>{{ $item->admin_id }}</td>
                                    <td>
                                        <a href="{{ route('admin.products.edit', $item->id) }}" class="btn btn-sm btn-primary">Edit</a>
                                        <form action="{{ route('admin.products.destroy', $item->id) }}" method="POST" class="d-inline">
                                            @csrf
                                            @method('DELETE')
                                            <button type="submit" class="btn btn-sm btn-danger">Delete</button>
                                        </form>
                                    </td>
                                </tr>
                            @empty
                                No Data Found
                            @endforelse
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


