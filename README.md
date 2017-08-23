# test
testing features

send grote oef (boodschappen) op github

wat ik heb:

$(document).ready(function () {

    var voornaam = $('#txtVoornaam').val();
    var achternaam = $('#txtAchternaam').val();
    var info = [];

    $('btnToevoegen').on('click', function () {
        if(voornaam !== '' && achternaam !== ''){
            info.push(voornaam, achternaam, $('#ddlModule').option.val())
            var row = $('<tr />');
            for(i=0; i<3; i++){
                // var kolom = $('<th />');
                // kolom.append(info[i]);
                row.append($('<td />').append(info[i]));
            }
            row.append($('<td />').append('<a />').attr('href', '#').text('Uitschrijven'));
            $('tbody').append(row);


        } else{
            window.alert("Voer de Voornaam en achternaam velden in.")
            // image?

        }
    })
    // TODO link verwijderen


});
grote oef (boodschappen) op github zetten a.u.b
