# Map Function

    let ids = $('.trackingItems').map(function () {
                return $(this).val();
            });
            
# Loop
    $.each(value.value, function (index, value) {
        attrValues += '<option value="' + attrIds + ',' + value + '">' + value + '</option>';
    });