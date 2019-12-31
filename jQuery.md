# Map Function

    let ids = $('.trackingItems').map(function () {
                return $(this).val();
            });
            
# Loop
    $.each(items.value, function (index, item) {
        output += '<option value="'+ item.id +'">'+ item.name +'</option>';
    });