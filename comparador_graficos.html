<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.7.1/jquery.min.js"></script>
    <title>Gráfico de línea con Highcharts</title>
    <!-- Incluye la biblioteca Highcharts -->
    <script src="https://code.highcharts.com/highcharts.js"></script>
    <style>
        h1 {
            text-align: center;
        }
        
        #crecimiento {
            background: #d3cece;
            width: 30%;
            height: 1.5rem;
            font-size: 1.2rem;
            padding: 10px;
            box-shadow: 5px 5px 10px 1px rgba(0,0,0,0.75);
            -webkit-box-shadow: 5px 5px 10px 1px rgba(0,0,0,0.75);
            -moz-box-shadow: 5px 5px 10px 1px rgba(0,0,0,0.75);
            text-align: center;
            /* margin-left: 50%; */
            margin-right: 1rem;
            float: right;
            border-radius: 5px;
        }
    </style>
</head>

<body>
    <h1>Comparador de Crecimiento</h1>

    <!-- Contenedor del primer gráfico -->
    <div id="grafico-linea-1" style="height: 300px;"></div>

    <!-- Contenedor del segundo gráfico -->
    <div id="grafico-linea-2" style="height: 300px;"></div>

    <div id = "crecimiento"></div>

    <!-- Código JavaScript para crear los gráficos de línea -->
    <script>
        // Datos para el primer gráfico
        var datos1 = {
        title: {
            text: 'Crecimiento de Trabajadores en Intel',
            align: 'left'
        },
        xAxis: {
            categories: ['Enero', 'Febrero', 'Marzo', 'Abril', 'Mayo']
        },
        yAxis: {
            title: {
            text: ''
            }
        },
        series: [{
            data: [130, 67, 109, 255, 177],
            dataLabels: {
            enabled: true,
            formatter: function () {
                return this.y;
            }
            }
        }],
        plotOptions: {
            series: {
            point: {
                events: {
                mouseOver: function () {
                    cambiacolor(chart1, chart2)
                }
                }
            },
            }
        },
        credits: {
            enabled: false
        },
        exporting: {
            enabled: false
        },
        legend: {
            enabled: false
        },
        tooltip: {
            // Mostrar el valor del punto al lado del punto
            formatter: function () {
            return '<b>' + this.x + '</b>: ' + this.y;
            }
        },
        };

        // Datos para el segundo gráfico
        var datos2 = {
        title: {
            text: 'Crecimiento de Trabajadores en IBM',
            align: 'left'
        },
        xAxis: {
            categories: ['Enero', 'Febrero', 'Marzo', 'Abril', 'Mayo']
        },
        yAxis: {
            title: {
            text: ''
            }
        },
        series: [{
            data: [115, 465, 223, 155, 99],
            dataLabels: {
            enabled: true,
            formatter: function () {
                return this.y;
            }
            }
        }],
        plotOptions: {
            series: {
            point: {
                events: {
                mouseOver: function () {
                    cambiacolor(chart2, chart1)
                }
                },
            },
            }
        },
        credits: {
            enabled: false
        },
        exporting: {
            enabled: false
        },
        legend: {
            enabled: false
        },
        tooltip: {
            // Mostrar el valor del punto al lado del punto
            formatter: function () {
            return '<b>' + this.x + '</b>: ' + this.y;
            }
        },
        };

    // Crea los gráficos
    var chart1 = new Highcharts.Chart('grafico-linea-1', datos1);
    var chart2 = new Highcharts.Chart('grafico-linea-2', datos2);
    //funcion para obtener el index del punto al que se le hace hover
    function cambiacolor(grafico_param_1, grafico_param_2){

        //poner el color rojo al punto que se le hace hover
        grafico_param_1.series[0].data[grafico_param_1.hoverPoint.index].update({
            marker: {
                fillColor: 'red'
            }
        });
        //remover el colro de los demas puntos
        for (let i = 0; i < grafico_param_1.series[0].data.length; i++) {
            if(i!=grafico_param_1.hoverPoint.index){
                grafico_param_1.series[0].data[i].update({
                    marker: {
                        fillColor: null
                    }
                });
            }
            
        }
        //poner el color rojo al punto que se le hace hover
        var index = grafico_param_1.hoverPoint.index;
        grafico_param_2.series[0].data[index].update({
            marker: {
                fillColor: 'red'
            }
        });
        //remover el colro de los demas puntos
        for (let i = 0; i < grafico_param_2.series[0].data.length; i++) {
            if(i!=index){
                grafico_param_2.series[0].data[i].update({
                    marker: {
                        fillColor: null
                    }
                });
            }
            
        }

        //activar el tooltip del grafico_param_2
        grafico_param_2.tooltip.refresh(grafico_param_2.series[0].data[index]);
        //desactivar el tooltip del grafico_param_1
        grafico_param_1.tooltip.hide();
    }
    //funcion que sume todos los valores de los puntos del grafico uno y dos 
    function sumarValores(obtener_total_de_cual_grafico){
        if (obtener_total_de_cual_grafico == "grafico_1")
        {
            var suma = 0;
            for (let i = 0; i < chart1.series[0].data.length; i++) {
                suma += chart1.series[0].data[i].y;
            }
        }
        else{
            var suma = 0;
            for (let i = 0; i < chart2.series[0].data.length; i++) {
                suma += chart2.series[0].data[i].y;
            }
        }
            
        return suma;
    }
    var total_grafico_1 = sumarValores("grafico_1");
    var total_grafico_2 = sumarValores("grafico_2");

    //funcion que tome en cuenta los dos valores y saque un porcentaje de cual crecio mas y cuanto porcentaje crecio con respecto al otro
        function empresa_ganadora (){
            var porcentaje_grafico_1 = (total_grafico_1*100)/(total_grafico_1+total_grafico_2);
            var porcentaje_grafico_2 = (total_grafico_2*100)/(total_grafico_1+total_grafico_2);
            var crecimiento = 0;
            if (porcentaje_grafico_1 > porcentaje_grafico_2){
                crecimiento = porcentaje_grafico_1 - porcentaje_grafico_2;
                //pasar crecimiento a dos decimales
                crecimiento = crecimiento.toFixed(2);
                $("#crecimiento").text("Intel creció en trabajadores "+crecimiento+"% mas que IBM")
            }
            else{
                crecimiento = porcentaje_grafico_2 - porcentaje_grafico_1;
                crecimiento = crecimiento.toFixed(2);
                $("#crecimiento").text("IMB creció en trabajadores "+crecimiento+"% mas que Intel") 
            }
        }
        empresa_ganadora ()

</script>

</body>
</html>
