# Asset Function
    function asset($path, $secure = null){
            if ($_SERVER['HTTP_HOST']=='127.0.0.1:8000')
                return app('url')->asset($path, $secure);
            if ($_SERVER['HTTP_HOST']=='localhost:8000')
                return app('url')->asset($path, $secure);
            else
                return app('url')->asset('public/'.$path, $secure);
      }
    
# Route Group with Prefix
    Route::prefix('admin')->group(function() {
        Route::get('/', 'AdminController');
    });
    
# Api with additional data
    return TransactionLineResource::collection($result)->additional(['extra' => [
        'balance' => $debit-$credit,
        'debit' => $debit,
        'credit' => $credit,
    ]]);
    
# Foreign Key
    $table->foreign('attendance_id')->references('id')->on('attendances');
          
# Hide .env file
Use this code in .htaccess file

    <Files ~ "^.*\.([Ee][Nn][Vv])">
     order allow,deny
     deny from all
     satisfy all
    </Files>
    
# Directory Permission
    sudo chgrp -R www-data storage bootstrap/cache public/uploads
    sudo chmod -R ug+rwx storage bootstrap/cache public/uploads