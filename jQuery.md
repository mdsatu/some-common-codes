# Map Function

    let ids = $('.trackingItems').map(function () {
                return $(this).val();
            });
            
# Loop
    $.each(items.value, function (index, item) {
        output += '<option value="'+ item.id +'">'+ item.name +'</option>';
    });

# Select 2
    $('.select_picker').select2({
        theme: 'classic',
        dropdownParent: $("#textStyleModal"),
        containerCssClass: 'custom-select2-container',
        dropdownCssClass: 'custom-select2-dropdown',
        templateResult: function(data) {
            return $('<span>').text(data.text).css('font-family', data.id);
        }
    });