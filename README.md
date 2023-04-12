<!doctype html>
<html lang="english">
<head>

    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <meta name="description" content="">



    <title>Platform Library</title>


    <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/1.10.24/css/jquery.dataTables.min.css">
    <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/responsive/2.2.7/css/responsive.dataTables.min.css">
    <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/searchbuilder/1.0.1/css/searchBuilder.dataTables.min.css">
    <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/searchpanes/1.2.1/css/searchPanes.dataTables.min.css">
    <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/datetime/1.0.2/css/dataTables.dateTime.min.css">

    <script type="text/javascript" language="javascript" src="https://code.jquery.com/jquery-3.5.1.js"></script>
    <script type="text/javascript" language="javascript" src="https://cdn.datatables.net/1.10.24/js/jquery.dataTables.min.js"></script>
    <script type="text/javascript" language="javascript" src="https://cdn.datatables.net/searchpanes/1.2.1/js/dataTables.searchPanes.min.js"></script>
    <script type="text/javascript" language="javascript" src="https://cdn.datatables.net/select/1.3.3/js/dataTables.select.min.js"></script>
    <script type="text/javascript" language="javascript" src="https://cdn.datatables.net/searchbuilder/1.0.1/js/dataTables.searchBuilder.min.js"></script>
    <script type="text/javascript" language="javascript" src="https://cdn.datatables.net/searchpanes/1.2.1/js/dataTables.searchPanes.min.js"></script>


    <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/buttons/1.7.0/css/buttons.dataTables.min.css">
    <script type="text/javascript" language="javascript" src="https://cdn.datatables.net/buttons/1.7.0/js/dataTables.buttons.min.js"></script>
    <script type="text/javascript" language="javascript" src="https://cdn.datatables.net/buttons/1.7.0/js/buttons.html5.min.js"></script>
    <script type="text/javascript" language="javascript" src="https://cdn.datatables.net/buttons/1.7.1/js/buttons.colVis.min.js"></script>

    <script type="text/javascript" language="javascript" src="https://cdn.datatables.net/plug-ins/1.13.2/dataRender/hyperLink.js"></script>
    <!-- Bootstrap core CSS -->
    <link href="http://modulelibrary.otis.com/site/assets/css/bootstrap.min.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css?family=Poppins:400,600&display=swap" rel="stylesheet">
    <link rel='stylesheet' href='https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.1.3/css/bootstrap.min.css'>

    <style>

        .stars-container {
            position: relative;
            display: inline-block;
            color: transparent;
        }

            .stars-container:before {
                position: absolute;
                top: 0;
                left: 0;
                color: lightblue;
            }

            .stars-container:after {
                position: absolute;
                top: 0;
                left: 0;
                color: gold;
                overflow: hidden;
            }

        .stars-:after {
            width: 0%;
        }

        .stars-0:after {
            width: 0%;
        }

        .stars-1:after {
            width: 20%;
        }

        .stars-2:after {
            width: 40%;
        }

        .stars-3:after {
            width: 60%;
        }

        .stars-4:after {
            width: 80%;
        }

        .stars-5:after {
            width: 100%;
        }


        .bd-placeholder-img {
            font-size: 1.125rem;
            text-anchor: middle;
            -webkit-user-select: none;
            -moz-user-select: none;
            user-select: none;
        }

        @media (min-width: 1200px) {
            .bd-placeholder-img-lg {
                font-size: 3.8rem;
            }
        }

        td.details-control {
            cursor: pointer;
            height: 60px;
        }

        td {
            border-right: 1px solid #f2f2f2;
            border-top: 10px solid white;
            border-bottom: 10px solid white;
            /*border-radius:5px;*/
        }

        table.dataTable tbody tr td:first-child {
            border-left: 3px solid rgb(55, 86, 130);
        }

        table.dataTable tbody tr td:last-child {
            border-right: 2px solid rgb(55, 86, 130);
        }

        table.dataTable tbody tr td {
            cursor: pointer;
            border-bottom: 1px solid transparent;
            border-top: #ebe6e6 1px solid;
            border-bottom: #ebe6e6 1px solid;
        }


        table.dataTable tbody tr:hover td {
            background-color: #c6cccf;
            border-top: rgb(198, 204, 207) 1px solid;
            border-bottom: rgb(198, 204, 207) 1px solid;
            box-shadow: 5px 5px 5px #c6cccf;
        }

        tr.shown td.details-control {
        }

        table.dataTable thead th {
            border-bottom: 0;
        }

        table.dataTable tfoot th {
            border-top: 0;
        }


        div.dtsp-panesContainer div.dtsp-searchPanes {
            display: flex;
            flex-direction: column;
            flex-wrap: wrap;
            justify-content: flex-start;
            align-content: flex-start;
            align-items: normal;
            clear: both;
            text-align: start;
        }

        div.dtsp-columns-3 {
            min-width: 100%;
            max-width: 100%;
            padding-left: 1%;
            padding-right: 1%;
            margin: 0px !important;
        }

        .dataTables_wrapper .dataTables_filter input {
            position: relative;
            border: 1px solid #aaa;
            border-radius: 5px;
            padding: 5px;
            background-color: white;
            margin-left: 3px;
        }

        .dataTables_wrapper .dataTables_filter {
            margin-top: 15px;
            float: left;
            text-align: right;
        }

        div.dtsp-panesContainer button.dtsp-clearAll {
            float: left;
            margin: 5px;
            border: 1px solid transparent;
            background-color: transparent;
            margin-bottom: 0px;
            margin-top: 3px;
        }
        /* Keyword search */
        div.dtsp-panesContainer div.dtsp-searchPanes div.dtsp-searchPane div.dtsp-topRow div.dtsp-searchCont input.dtsp-search {
            flex-direction: row;
            flex-wrap: nowrap;
            flex-grow: 1;
            flex-shrink: 0;
            flex-basis: 100px;
            min-height: 20px;
            max-width: auto;
            min-width: auto;
            border-top: rgb(222, 220, 213) 1px solid;
            border-bottom: rgb(222, 220, 213) 1px solid;
            border-left: rgb(222, 220, 213) 1px solid;
            border-right: rgb(222, 220, 213) 5px solid;
            padding-left: 12px;
        }

        div.dtsp-panesContainer div.dtsp-searchPanes div.dtsp-searchPane div.dataTables_scrollBody {
            border-bottom: black;
            height: auto !important;
        }

        div.dtsp-panesContainer div.dtsp-searchPanes div.dtsp-searchPane button.dtsp-paneButton {
            opacity: 1;
        }

        div.dtsp-panesContainer div.dtsp-searchPanes div.dtsp-searchPane {
            flex-direction: row;
            flex-wrap: nowrap;
            flex-grow: 1;
            flex-shrink: 0;
            flex-basis: auto;
            justify-content: space-around;
            align-content: flex-start;
            align-items: stretch;
            padding-top: 0px;
            padding-bottom: 0px;
            margin: 5px;
            margin-top: 0px;
            margin-bottom: 0px;
            font-size: 0.9em;
        }

        table.dataTable thead .sorting {
        }
        /* Filter block Style */
        div.dtsp-panesContainer {
            background-color: #DDFFE5;
            font-family: 'Open Sans', sans-serif;
            padding: 2px;
            border: 1px solid #ccc;
            border-radius: 6px;
            margin: 5px 0;
            clear: both;
            text-align: center;
            font-size: 12px;
        }
        /* Nav bar shadow */
        .navbar {
            -webkit-box-shadow: 0 8px 6px -6px #999;
            -moz-box-shadow: 0 8px 6px -6px #999;
            border-bottom: rgb(168, 194, 134) 3px solid;
            box-shadow: 0 8px 6px -6px #999;
            /* the rest of your styling */
        }
        /* footer btn styling */
        .dataTables_wrapper .dataTables_paginate .paginate_button.current, .dataTables_wrapper .dataTables_paginate .paginate_button.current:hover {
            color: #000000 !important;
            border: 1px solid #979797;
            background-color: white;
            background: -webkit-gradient(linear, left top, left bottom, color-stop(0%, white), color-stop(100%, rgb(4, 30, 66)));
            background: -webkit-linear-gradient(top, white 0%, rgb(4, 30, 66) 100%);
            background: -moz-linear-gradient(top, white 0%, rgb(4, 30, 66) 100%);
            background: -o-linear-gradient(top, white 0%, rgb(4, 30, 66) 100%);
            background: linear-gradient(to bottom, #ffefef 0%, rgb(4, 30, 66) 100%);
        }
        /* EXPORT BTNS */
        button.dt-button, div.dt-button, a.dt-button, input.dt-button {
            position: relative;
            top: 14px;
            left: 8px;
            display: inline-block;
            box-sizing: border-box;
            margin-right: .333em;
            margin-bottom: .333em;
            padding: .5em 1em;
            border: 1px solid rgba(0, 0, 0, 0.3);
            border-radius: 5px;
            cursor: pointer;
            font-size: .88em;
            line-height: 1.6em;
            color: black;
            white-space: nowrap;
            overflow: hidden;
            background-color: white !important;
            background: -webkit-linear-gradient(top, rgba(230, 230, 230, 0.1) 0%, rgba(0, 0, 0, 0.1) 100%);
            background: -moz-linear-gradient(top, rgba(230, 230, 230, 0.1) 0%, rgba(0, 0, 0, 0.1) 100%);
            background: -o-linear-gradient(top, rgba(230, 230, 230, 0.1) 0%, rgba(0, 0, 0, 0.1) 100%);
            background: linear-gradient(to bottom, rgba(230, 230, 230, 0.1) 0%, rgba(0, 0, 0, 0.1) 100%);
            -webkit-user-select: none;
            -moz-user-select: none;
            -ms-user-select: none;
            user-select: none;
            text-decoration: none;
            outline: none;
            text-overflow: ellipsis;
        }
        /* Pill Color */
        div.dtsp-panesContainer div.dtsp-searchPanes div.dtsp-searchPane div.dataTables_scrollBody div.dtsp-nameCont span.dtsp-pill {
            display: inline-block;
            background-color: transparent;
            text-align: center;
            border: 1px solid rgb(214, 213, 126);
            border-radius: 10px;
            width: auto;
            min-width: 30px;
            color: black;
            font-size: 0.9em;
            padding: 0 4px;
        }

        div.dtsp-panesContainer div.dtsp-searchPanes div.dtsp-searchPane div.dataTables_scrollBody div.dtsp-nameCont {
            width: 100%;
            display: flex;
            flex-direction: row;
            justify-content: space-evenly;
            align-content: stretch;
            align-items: center;
            flex-wrap: nowrap;
        }

            div.dtsp-panesContainer div.dtsp-searchPanes div.dtsp-searchPane div.dataTables_scrollBody div.dtsp-nameCont span.dtsp-name {
                text-overflow: ellipsis;
                overflow: hidden;
                display: inline-block;
                vertical-align: middle;
                white-space: nowrap;
                flex-grow: 2;
                width: 50px;
            }

        /* filter td property */
        div.dtsp-panesContainer div.dtsp-searchPanes div.dtsp-searchPane tr > th, div.dtsp-panesContainer div.dtsp-searchPanes div.dtsp-searchPane tr > td {
            padding: 10px 10px;
            border-top: #d9d3ca 1px solid;
            border-left: #d9d3ca 1px solid;
            border-right: #d9d3ca 1px solid;
            border-bottom: transparent 1px solid;
            background-color: #d9d3ca;
        }

        a {
            text-decoration: none;
            font-variant: revert;
            padding-left: 5px;
            padding-right: 5px;
            border-top: 3px solid transparent;
        }

            a:hover, a:focus {
                text-align: center;
            }

        .active {
            color: rgb(4, 30, 66);
            text-align: center;
        }


        .dataTables_wrapper .dataTables_length select {
            border: 1px solid #aaa;
            border-radius: 3px;
            padding: 5px;
            background-color: rgb(227, 222, 222);
            padding: 4px;
        }

        /* iNFO ROW*/   
        .dataTables_wrapper .dataTables_info {
            clear: both;
            position: absolute;
            right: 3.2%;
            top: -2px;
            color: rgb(203, 160, 82);
        }

        /*set page length*/
        .dataTables_wrapper .dataTables_length {
            position: absolute;
            right: 10%;
            top: 35px;
            color: rgb(145, 131, 106);
        }
        /*Table filter pan */
        div.dtsp-panesContainer div.dtsp-searchPanes div.dtsp-searchPane div.dataTables_wrapper {
            flex: 1;
            margin: 1em 0.5%;
            margin-top: 0px;
            border-bottom: 2px solid #bd1c1c;
            border: 2px solid rgb(203, 160, 82);
            border-radius: 4px;
        }
        /*Filter pan selected*/
        table.dataTable tbody >
        tr.selected {
            background-color: blue;
        }

        /* Search Banner */
        .nfilter {
            width: 90%;
            position: relative;
            left: 5%;
            height: 65px;
            padding-top: 0px;
            padding-right: 7px;
            padding-left: 7px;
            background: #02050C;
            color: black;
            border-radius: 5px;
            box-shadow: 2px 3px 5px rgb(203, 160, 82);
        }
        /* toggle */
        .sidenav {
            height: 100%;
            width: 0px;
            position: fixed;
            z-index: 1;
            top: 0;
            left: 0;
            background-color: white;
            border-right: gray 2px solid;
            overflow-x: hidden;
            transition: 0.5s;
            padding-top: 60px;
            box-shadow: 2px 2px 5px gray;
        }

            .sidenav a {
                padding: 8px 8px 8px 32px;
                text-decoration: none;
                font-size: 25px;
                color: #818181;
                display: block;
                transition: 0.3s;
            }

                .sidenav a:hover {
                    color: #0c1042;
                }

            .sidenav .closebtn {
                position: absolute;
                top: 0;
                right: 25px;
                font-size: 36px;
                margin-left: 50px;
            }

        #main {
            transition: margin-left .5s;
            padding: 16px;
        }
        g1
        @media screen and (max-height: 450px) {
            .sidenav {
                padding-top: 15px;
            }

                .sidenav a {
                    font-size: 18px;
                }
        }
        /* Scrollbar */
        ::-webkit-scrollbar {
            width: 10px;
        }

        /* Track */
        ::-webkit-scrollbar-track {
            background: #ebeeff;
        }

        /* Handle color */
        ::-webkit-scrollbar-thumb {
            background: transparent;
            border: rgb(191, 152, 80) 1px solid;
            border-radius: 5px;
        }

            /* Handle on hover */
            ::-webkit-scrollbar-thumb:hover {
                background: #d1c3ae;
                width: 20px;
            }



        /* Arrow animation */

        .arrow {
            position: absolute;
            top: 10%;
            left: 25%;
            transform: translate(-50%,-50%);
        }

            .arrow span {
                display: block;
                width: 10px;
                height: 10px;
                border-bottom: 5px solid rgb(138, 133, 125);
                border-right: 5px solid rgb(138, 133, 125);
                transform: rotate(45deg);
                margin: -10px;
                animation: animate 2s infinite;
            }

                .arrow span:nth-child(2) {
                    animation-delay: -0.2s;
                }

                .arrow span:nth-child(3) {
                    animation-delay: -0.4s;
                }

        @keyframes animate {
            0% {
                opacity: 0;
                transform: rotate(45deg) translate(-20px,-20px);
            }

            50% {
                opacity: 1;
            }

            100% {
                opacity: 0;
                transform: rotate(45deg) translate(20px,20px);
            }
        }
        /* Hide search sort */
        div.dtsp-panesContainer div.dtsp-searchPanes div.dtsp-searchPane input.dtsp-paneInputButton, div.dtsp-panesContainer div.dtsp-searchPanes div.dtsp-searchPane button.dtsp-paneButton {
            height: 35px;
            width: 35px;
            max-width: 35px;
            min-width: 0;
            display: inline-block;
            margin: 2px;
            border: 0px solid transparent;
            background-color: ghostwhite;
            font-size: 16px;
            margin-bottom: 0px;
            flex-grow: 0;
            flex-shrink: 0;
            flex-basis: 35px;
            font-family: sans-serif;
        }

        .text-wrap {
            white-space: normal;
        }

        table.dataTable tbody tr.selected {
            color: #75131b !important;
            font-weight: 600;
        }
    </style>

    <script type="text/javascript">

        var dataSet = [
            ["P0011A", "Light Duty", "Gen3 Edge", "GB7588+A1_2015", "1, 1.6, 1.75", "680 - 1050", 75, "China", "HAA21310BS", "ACD", "BLMRLPASBIBI_SEB_ZH"],
            ["P0011B", "Light Duty", "Gen2 Prime Phase I", "IS14665", 0.7, "340 - 408", 20, "India", "   -", "ACD", "WAA29100A"],
            ["P0011C", "Light Duty", "Gen2 Prime Phase II&III", "EN81-20/50", 1, "320 - 630", 30, "India", "   -", "ACD", "WAA29100B"],
            ["P0011D", "Light Duty", "Gen2 Core", "IS14665", 0.7, "340 - 544", 25, "India", "   -", "ACD", "NAA29100S_SEB"],
            ["P0011E", "Light Duty", "GU1 QTO", "EN81-20/50", 1, "550 - 1000", 45, "Korea", "   -", "ACD", "   -"],
            ["P0011F", "Light Duty", "Gen2 Premier Residential", "JIS", "0.75, 1, 1.5, 1.75", "450 - 850", 50, "Japan", "   -", "ACD", "   -"],
            ["P0012A", "Light Duty", "Genesis", "EN81-20/50", 1, "320 - 1000", 45, "Madrid", "   -", "LVA", "   -"],
            ["P0012B", "Light Duty", "Gen2 Life", "EN81-20/50", "1,1.6,1.75", "320 - 1000", 75, "Madrid", "   -", "LVA", "   -"],
            ["P0012C", "Light Duty", "GeN2 Variable", "EN81-20/50", "1,1.6,1.75", "225 - 1000", 75, "Madrid", "   -", "LVA", "   -"],
            ["P0012D", "Light Duty", "GeN2 Flex+", "EN81-20/50", 1, "225 - 1000", 45, "Madrid", "   -", "LVA", "   -"],
            ["P0012E", "Light Duty", "GeN2 16-21P", "EN81-20/50", "1,1.6,1.75", "1250 - 1600", 75, "Madrid", "   -", "LVA", "   -"],
            ["P0012F", "Light Duty", "GeN2 Switch", "EN81-20/50", 1, "225 - 630", 27, "Madrid", "   -", "LVA", "   -"],
            ["P0012G", "Light Duty", "Gen2 Home", "EN81-20/50", 0.15, "250 - 385", 15, "Madrid", "   -", "LVA", "   -"],
            ["P0012H", "Light Duty", "Genesis", "EN81-20/50", 1, "450 - 1020", 30, "Gien", "   -", "LVA", "   -"],
            ["P0012I", "Light Duty", "Gen2 Life", "EN81-20/50", "1 - 1.6", "320 - 1020", 50, "Gien", "   -", "LVA", "   -"],
            ["P0012K", "Light Duty", "Gen2 Nova", "IS14665", 1, "340 - 1020", 60, "India", "   -", "LVA", "NAA29100P_SEB"],
            ["P0012L", "Light Duty", "Gen2 Life", "IS14665", "1.5, 1.75", "544 - 1020", 96, "India", "   -", "LVA", "NAA29100AB_SEB"],
            ["P0012M", "Light Duty", "Gen2 Light", "EN81-1", "1, 1.5, 1.6, 1.75", "450 - 1000", 90, "Brazil", "   -", "LVA", "   -"],
            ["P0012N", "Light Duty", "Gen2 Comfort", "EN81-1", 1, "300 - 1125", 54, "Brazil", "   -", "LVA", "   -"],
            ["P0013A", "Light Duty", "Gen2 Core", "IS14665", 0.7, "340 - 408", "   -", "India", "   -", "LVA", "NAA29100R_SEB"],
            ["P0013B", "Light Duty", "Gen2 Nova", "IS14665", 1, "340 - 1020", "   -", "India", "   -", "ACD", "NAA29100E_SEB"],
            ["P0013C", "Light Duty", "Gen2 Life", "IS14665", "1.5,1.75", "544 - 1020", "   -", "India", "   -", "ACD", "NAA29100AB_SEB"],
            ["P0014A", "Light Duty", "GeN2 Fit", "EN81-20/50", 1, "100 - 300", 35, "Madrid", "   -", "ACD", "   -"],
            ["P0015A", "Light Duty", "Gen2 Premier Passenger & Bed", "JIS", "0.75, 1, 1.5, 1.75", "450 - 1000", 50, "Japan", "   -", "LVA", "   -"],
            ["P0021A", "Mid Rise ", "Gen2 Comfort Pro MR", "GB7588+A1_2015", "1,1.5,1.6,1.75,2.0,2.5", "630 - 1600", 140, "China", "HAA21310S", "ACD", "BLMRPASNABI_SEB_ZH"],
            ["P0021B", "Mid Rise ", "Gen2 Comfort Pro MR SE", "GB7588+A1_2015", "1, 1.5, 1.6, 1.75,2.0,2.5", "630 - 1600", 140, "China", "HAA21310S", "ACD", "BLMRPASNASO_SEB_ZH"],
            ["P0021C", "Mid Rise ", "Gen2 Premier Pro MR", "GB7588+A1_2015", "1, 1.5, 1.6, 1.75,2.0, 2.5", "800 - 2000", 140, "China", "HAA21310S", "ACD", "BLMRPASNATE_SEB_ZH"],
            ["P0021D", "Mid Rise ", "GeN2MR_TEDA", "EN81_20_2014,GB7588+A1_2015", "1, 1.6, 1.75, 2.0, 2.5", "630 - 2000", 125, "China", "HAA21310S", "ACD", "GEN2MR_TEDA_SEB_EN"],
            ["P0021E", "Mid Rise ", "Gen2-MR (2021)", "GB7588+A1_2015", "1, 1.5, 1.6, 1.75, 2.0, 2.5", "630 - 2000", 140, "China", "HAA21310S", "ACD", "BLMRPASNANU_SEB_ZH"],
            ["P0021F", "Mid Rise ", "Gen2-MR (2021) SE", "GB7588+A1_2015", "1, 1.5, 1.6, 1.75, 2.0, 2.5", "630 - 2000", 140, "China", "HAA21310S", "ACD", "BLMRPASNAKA_SEB_ZH"],
            ["P0021G", "Mid Rise ", "GeN2MR_HZ", "GB7588+A1_2015,EN81_20_2014", "1, 1.5, 1.6, 1.75, 2.0, 2.5", "630 - 2000", 140, "China", "HAA21310S", "ACD", "GEN2MR_HZ_SEB_EN"],
            ["P0021H", "Mid Rise ", "Gen3 Peak MR", "GB7588+A1_2015", "1,1.5,1.6,1.75,2.0,2.5", "630 - 2000", 140, "China", "HAA21310S", "ACD", "BLMRPASNAOK_SEB_ZH"],
            ["P0021I", "Mid Rise ", "Gen3 Peak MR SE", "GB7588+A1_2015", "1,1.5,1.6,1.75,2.0,2.5", "630 - 2000", 140, "China", "HAA21310S", "ACD", "BLMRPASNUBI_SEB_ZH"],
            ["P0021J", "Mid Rise ", "GEN3MR_HZ", "EN81_20_2014", "1,1.5,1.6,1.75,2.0,2.5", "630 - 2000", 140, "China", "HAA21310S", "ACD", "GEN3MR_HZ_SEB_EN"],
            ["P0022A", "Mid Rise ", "Gen2 Stream", "EN81-20/50", "1,1.6,1.75,2,2.5", "630 - 2500", 120, "Gien", "   -", "ACD", "   -"],
            ["P0023A", "Mid Rise ", "Gen2 Comfort Pro MRL", "GB7588+A1_2015", "1,1.6,1.75", "630 - 1600", 96, "China", "HAA21310AW", "LVA", "BLMRLPASNABI_SEB_ZH"],
            ["P0023B", "Mid Rise ", "Gen2 Comfort Pro MRL SE", "GB7588+A1_2015", "1,1.6,1.75", "630 - 1600", 96, "China", "HAA21310AW", "ACD", "BLMRLPASNASO_SEB_ZH"],
            ["P0023C", "Mid Rise ", "Gen2 Premier Pro MRL", "GB7588+A1_2015", "1,1.6,1.75,2.0,2.5", "800 - 2000", 120, "China", "HAA21310AW", "ACD", "BLMRLPASNATE_SEB_ZH"],
            ["P0023D", "Mid Rise ", "GeN2MRL_TEDA", "EN81-20/50 & GB7588+A1_2015", "1,1.6,1.75,2.0,2.5", "630 - 2000", 120, "China", "HAA21310AW", "ACD", "GEN2MRL_TEDA_SEB_EN"],
            ["P0023E", "Mid Rise ", "Gen2 (2021)", "GB7588+A1_2015", "1,1.5,1.6,1.75,2.0,2.5", "630 - 2000", 120, "China", "HAA21310AW", "ACD", "BLMRLPASNANU_SEB_ZH"],
            ["P0023F", "Mid Rise ", "Gen2 FLEX", "GB7588+A1_2015", "1,1.5,1.6,1.75", "630 - 1000", 96, "China", "HAA21310AW", "ACD", "BLMRLPASNAKA_SEB_ZH"],
            ["P0023G", "Mid Rise ", "Gen2 (2021) SE", "GB7588+A1_2015", "1,1.5,1.6,1.75,2.0,2.5", "630 - 2000", 120, "China", "HAA21310AW", "ACD", "BLMRLPASNAPA_SEB_ZH"],
            ["P0023H", "Mid Rise ", "GeN2MRL_HZ", "EN81_20 & GB7588+A1_2015", "1,1.5,1.6,1.75,2.0,2.5", "630 - 2000", 120, "China", "HAA21310AW", "ACD", "GEN2MRL_HZ_SEB_EN"],
            ["P0023I", "Mid Rise ", "Gen3 Peak MRL", "GB7588+A1_2015", "1,1.6,1.75,2.0,2.5", "630 - 2000", 120, "China", "HAA21310AW", "ACD", "BLMRLPASNAOK_SEB_ZH"],
            ["P0023J", "Mid Rise ", "Gen3 Peak MRL SE", "GB7588+A1_2015", "1,1.6,1.75,2.0,2.5", "630 - 2000", 120, "China", "HAA21310AW", "ACD", "BLMRLPASNUBI_SEB_ZH"],
            ["P0023K", "Mid Rise ", "Gen3MRL_TEDA", "EN81-20/50", "1,1.6,1.75,2.0,2.5", "630 - 2000", 120, "China", "HAA21310AW", "ACD", "GEN3MRL_TEDA_SEB_EN"],
            ["P0023L", "Mid Rise ", "Gen3MRL_HZ", "EN81-20/50", "1,1.5,1.6,1.75,2.0,2.5", "630 - 2000", 120, "China", "HAA21310AW ,", "ACD", "GEN3MRL_HZ_SEB_EN"],
            ["P0023N", "Mid Rise ", "GeN2 MRL(GR1)", "EN81-20/50", "1,1.6,1.75", "550 - 1600", "   -", "Korea", "   -", "ACD", "   -"],
            ["P0024A", "Mid Rise", "Gen3 Core", "ASME A17.1", "0.76-1.02 ", "953-1588", 18, "Florence", "   -", "ACD5", "   -"],
            ["P0025A", "Mid Rise ", "Arise", "GB7588+A1_2015", "1,1.5,1.75,2.0,2.5", "630 - 1600", 130, "China", "HAA21310L", "ACD", "RPMRPASNATE_SEB_ZH"],
            ["P0025B", "Mid Rise ", "OH6000 (2021)", "GB7588+A1_2015", "1,1.5,1.75,2.0,2.5", "800 - 1150", 130, "China", "HAA21310L", "ACD", "RPMRPASNANU_SEB_ZH"],
            ["P0025C", "Mid Rise ", "OH6000 (2021) SE", "GB7588+A1_2015", "1,1.5,1.75,2.0,2.5", "800 - 1150", 130, "China", "HAA21310L", , "RPMRPASNUNU_SEB_ZH"],
            ["P0025D", "Mid Rise ", "Regen-M", "GB7588+A1_2015", "1,1.5,1.75,2.0,2.5", "550 - 1600", 130, "China", "HAA21310L", "G3C", "RPMRPASNAPA_SEB_ZH"],
            ["P0025E", "Mid Rise ", "Regen-M (2021 SE)", "GB7588+A1_2015", "1,1.5,1.75,2.0,2.5", "550 - 1600", 130, "China", "HAA21310L", "OH_CON, ACD4MR", "RPMRPASNUKA_SEB_ZH"],
            ["P0025F", "Mid Rise ", "Arise", "EN81_20_2014,GB7588+A1_2015", "1,1.5,1.75,2.0,2.5", "550 - 1600", 130, "China", "HAA21310L", "OH_CON, ACD4MR,ACD5MR", "ARISE_CP_SEB_EN"],
            ["P0025G", "Mid Rise ", "Arise", "IS14665", 2.5, "1156 - 1632", "   -", "India", "   -", "OH_CON, ACD4MR,ACD5MR", "WAA29100C_SEB"],
            ["P0026A", "Mid Rise ", "OH6000 MRL", "GB7588+A1_2015", "1,1.5,1.6,1.75", "630 - 1050", 75, "China", "HAA21310BX", "ACD4MR,ACD5MR", "RPMRLPASNANU_SEB_ZH"],
            ["P0026B", "Mid Rise ", "OH6000 MRL(SE)", "GB7588+A1_2015", "1,1.5,1.6,1.75", "630 - 1050", 75, "China", "HAA21310BX", "ACD4MR,ACD5MR", "RPMRLPASNUNU_SEB_ZH"],
            ["P0031A", "High Rise", "Skyrise Prime", "GB7588+A1_2015", "3,3.5,4.0", "900 - 1600", 230, "China", "HAA21310BK", "OH_CON, ACD4MR", "RPMRPASNASO_SEB_ZH"],
            ["P0031B", "High Rise", "OE8000", "GB7588+A1_2015", "3,3.5,4.0", "900 - 1600", 230, "China", "HAA21310BK", "ACD", "RPMRPASNASE_SEB_ZH"],
            ["P0031C", "High Rise", "SkyrisePrime_EN", "GB7588+A1_2015", "3,3.5,4.0", "900 - 1600", 230, "China", "HAA21310BK", "ACD", "SKYRISEPRIME_EN_SEB_EN"],
            ["P0041A", "Heavy Duty", "G2S", "ASME A17.1", "952 - 2267", 1.75, 45, "Florence", "   -", "ACD", "   -"],
            ["P0041B", "Heavy Duty", "G2O", "ASME A17.1", "1133 - 2267", 2.5, 90, "Florence", "   -", "ACD", "   -"],
            ["P0051A", "Gen360", "Gen360", "EN81-20/50", "225 - 1000", "1,1.6,1.75", 75, "Gien", "   -", "ACD", "   -"],
           

        ]

        $(document).ready(function () {
            var table = $('#container').DataTable({

                data: dataSet,
                columns: [

                    //{ "width": "20%", "targets": 0 },


                    {
                        "title": "Number",
                        "render": function (data, type, row, meta) {
                            if (type === 'display') {
                                data = '<a href="https://windchill.otis.com/Windchill/netmarkets/jsp/ext/otis/wc/querypart/queryPart.jsp?number=' + data + '">' + data + '</a>';
                            }
                            return data;
                        }
                    },

                    { title: 'Platform Group ' },
                    { title: 'Product Name' },
                    { title: ' Code ' },
                  
                    { title: 'Speed (m/s)' },
                    { title: 'Duty Load(kg)' },
                    { title: 'Rise (m) ' },
                    { title: 'Region' },
                    {
                        "title": 'Master Wiring Drawing',
                        "render": function (data, type, row, meta) {
                            if (type === 'display') {
                                data = '<a href="https://windchill.otis.com/Windchill/netmarkets/jsp/ext/otis/wc/querydoc/queryDocument.jsp?number=' + data + '">' + data + '</a>';
                            }
                            return data;
                        }


                    },
                    { title: 'Controller' },
                    {
                        title: 'SEB',
                        "render": function (data, type, row, meta) {
                            if (type === 'display') {
                                data = '<a href="https://windchill.otis.com/Windchill/netmarkets/jsp/ext/otis/wc/querydoc/queryDocument.jsp?number=' + data + '">' + data + '</a>';
                            }
                            return data;
                        }
                    },
                ],



                "responsive": true,
                "targets": 'no-sort',
                "bSort": true,
                "order": [[2, 'asc']],

                "lengthMenu": [[10, 25, 50, , -1], [10, 25, 50, 100, "All"]],
                "language": {
                    "search": "_INPUT_",
                    "searchPlaceholder": "Search your required product library ",
                    "zeroRecords": "Nothing found - sorry",
                    "info": "Number of Platfrom Variants : _MAX_",
                    "infoEmpty": "No records availa	ble",
                    "infoFiltered": "(Filtered: _TOTAL_ )"
                },
                "search": {
                    "addClass": 'form-control input-lg col-xs-12'
                },
                "fnDrawCallback": function () {
                    $("input[type='search']").attr("id", "searchBox");
                    $('#dialPlanListTable').css("float", "right;");
                    $("select[name='dialPlanListTable_length'], #searchBox").removeClass("input-sm");
                    $('#searchBox').css("width", "28vw");
                },
                //export btns
                buttons: {
                    //buttons: [  'colvis', 'copy', 'pdf', 'excel' ],
                    buttons: [

                        //  {
                        //    extend: 'pdf',
                        //    text: 'PDF',
                        //    title: 'Export visible rows to PDF',
                        //    exportOptions: {
                        //          columns: ':visible'
                        //      },
                        //  },

                        {
                            extend: 'excel',
                            text: 'Excel',
                            title: 'Export visible rows to excel',
                            exportOptions: {
                                columns: ':visible'
                            },
                        },

                        {
                            extend: 'copy',
                            text: 'Copy',
                            title: 'Copy to clipboard',
                            exportOptions: {
                                columns: ':visible'
                            },
                        },


                        {

                            extend: 'colvis',

                            text: 'Column Display',
                            exportOptions: {
                                columns: ':visible'
                            },
                        }

                    ],
                    //buttons: [  'colvis' ]
                },
                //resonsive
                responsive: {
                    breakpoints: [
                        { name: 'bigdesktop', width: Infinity },
                        { name: 'meddesktop', width: 1480 },
                        { name: 'smalldesktop', width: 1280 },
                        { name: 'medium', width: 1188 },
                        { name: 'tabletl', width: 1024 },
                        { name: 'btwtabllandp', width: 848 },
                        { name: 'tabletp', width: 800 },
                        { name: 'mobilel', width: 480 },
                        { name: 'mobilep', width: 320 }
                    ]
                },
                //searchpans
                searchPanes: {
                    layout: `columns-1`,
                    //columns: [0,1,4,5,6],


                    cascadePanes: true,
                    viewTotal: true, //to show pill total & filtered for custom panels
                },

                //sidenav "dom": '<"myCustomClass1"fP>t<"bottom"ilp><"clear">',
                "dom": '<"sidenav"P><"nfilter"fBli>t<"bottom"p><"clear">',


                //buttons: [ 'copy', 'pdf', 'excel' ],
                columnDefs: [
                    { "targets": [3], "visible": false, "searchable": true },
                    { "targets": [], "visible": false, "searchable": true },

                    { searchPanes: { show: false }, targets: [0] },
                    { searchPanes: { show: true }, targets: [1] },
                    { searchPanes: { show: true }, targets: [2] },
                    { searchPanes: { show: false }, targets: [3] },
                    { searchPanes: { show: false }, targets: [4] },
                    { searchPanes: { show: false }, targets: [5] },
                    { searchPanes: { show: false }, targets: [6] },
                    { searchPanes: { show: true }, targets: [7] },
                    { searchPanes: { show: false }, targets: [8] },
                    { searchPanes: { show: false }, targets: [9] },
                    { searchPanes: { show: false }, targets: [10] },

                ]
            });


            //adding column dropdown

            // Add event listener for opening and closing details
            $('#container tbody').on('click', 'td.details-control', function () {

                //table highlight

                //child row show / hide
                var tr = $(this).closest('tr');
                var row = table.row(tr);

                if (row.child.isShown()) {
                    // This row is already open - close it
                    row.child.hide();
                    tr.removeClass('shown');
                }
                else {
                    // Open this row
                    row.child(format(row.data())).show();
                    tr.addClass('shown');
                }

            });
            //add element id for filter
            $('.sidenav').attr('id', 'mySidenav')
            document.getElementById("mySidenav").style.width = "250px";
            document.getElementById("main").style.marginLeft = "250px";
            document.getElementById("newbtn").style.left = "225px";
            $("button").remove(".dtsp-countButton, .dtsp-nameButton");
            $('.dtsp-topRow').removeClass("dtsp-subRowsContainer")

        });


        function openNav() {
            var x = document.getElementById("mySidenav").style.width;
            if (x === "0px") {
                document.getElementById("mySidenav").style.width = "250px";
                document.getElementById("main").style.marginLeft = "250px";
                document.getElementById("newbtn").style.left = "225px";
                document.getElementById("rarrow").style.transform = "rotate(0deg)";
                document.getElementById("rarrow").style.top = "0px";
                document.getElementById("rarrow").style.left = "20px";
            } else {
                document.getElementById("mySidenav").style.width = "0px";
                document.getElementById("main").style.marginLeft = "0px";
                document.getElementById("newbtn").style.left = "-22px";
                document.getElementById("rarrow").style.transform = "rotate(180deg)";
                document.getElementById("rarrow").style.top = "30px";
                document.getElementById("rarrow").style.left = "10px";

            }
        }
    </script>
    <!-- Custom styles for this template -->
    <link href="http://modulelibrary.otis.com/site/assets/css/navbar-top-fixed.css" rel="stylesheet">
    <link href="http://modulelibrary.otis.com/site/assets/css/navbar.css" rel="stylesheet">
</head>
  <body style="max-height:500px; overflow:scroll;">


   <nav class="navbar navbar-expand-sm navbar-dark fixed-top" style="background-color: rgb(28, 59, 102);">
    <div class="container-fluid">
	          <h1 class="d-flex align-items-center fs-4 text-white mb-0">
			   <a class="navbar-brand" href="https://otiselevator.sharepoint.com/sites/PlatformDevelopment/sitepages/home.aspx" style="color: rgb(4, 30, 66) !important;"><img src="http://modulelibrary.otis.com/site/assets/img/logop.png" alt="" width="420px" height="65px" class="d-inline-block align-text-top" style="transparent !important;position:absolute;  left: 0px; top: 0px" ></a>
			        
    </h1>
      <button class="navbar-toggler" 
	  type="button" 
	 
	  data-bs-target="#navbarsExample03" 
	  aria-controls="navbarsExample03" 
	  aria-expanded="false" 
	  aria-label="Toggle navigation">
	  
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="navbarsExample03">

          <ul class="navbar-nav me-auto mb-2 mb-sm-0">
              <li class="nav-item"><a class="nav-link active" aria-current="page" href="index.html" style="transparent  !important;padding-left:350px; border-top:transparent 1px solid;">&nbsp;</a></li>

              <li class="nav-item">
                  <a class="nav-link active" aria-current="page" href="index.html" style="color: rgb(203, 160, 82) !important;border-top:transparent 1px solid; padding:10px;">Product Library</a>
              </li>

              <li class="nav-item">
                  <a class="nav-link" href="about.html" style="color: white !important; padding-left: 5px; padding-right: 5px; border-top: transparent 1px solid; padding:10px;">About</a>
              </li>

          </ul>
      </div>
    </div>
  </nav>

   <div id="main" style="margin-left: 4px;">
       <!-- class="alert alert-success" (place in div to get the notification of updated day )  -->
       <div id="success-alert" style="left:5%; width:90%;">
       </div>
       <table  id="container"  style="position:relative; left:0%;width:100%;border-collapse:separate;border-spacing: 0 10px;">
           <thead>
               <tr>
                   <!-- <th align= "center" style="width:5%"><img src="mg.png"></th> -->
                   <th align="left" style="width: 10%; text-align: left; background-color: #DDFFE5; ">Number</th>
                   <th align="left" style="width: 10%; text-align: left; background-color: #DDFFE5; ">
                       platform Group
                   </th>
                   <th align="left" style="width: 35%;  background-color: #DDFFE5;text-decoration:underline; ">Product Name </th>
                   <th align="center" style="width: 10%; text-align: center; background-color: #DDFFE5; ">Code </th>
                   
                   <th align="left" style="width: 15%;  background-color: #DDFFE5; ">
                       Speed
                   </th>
                   <th align="left" style="width: 10%;  background-color: #DDFFE5; ">
                       Duty Load(kg)
                   </th>
                   <th align="left" style="width: 8%;  background-color: #DDFFE5; ">
                       Rise (m)
                   </th>
                   <th align="left" style="width: 5%;  background-color: #DDFFE5; ">
                       Region
                   </th>
                   <th align="center" style="width: 15%; text-align: center; background-color: #DDFFE5; ">
                       Master Wiring Drawing
                   </th>
                   <th align="left" style="width: 10%;  background-color: #DDFFE5; ">
                      Controller
                   </th>
                   <th align="left" style="width: 10%;  background-color: #DDFFE5; ">
                       SEB
                   </th>


               </tr>
           </thead>
          
       </table>

       <!-- Toggle Button -->
       <!-- (symbols in the filter table )
           <span id="newbtn" style="

         background-color:rgb(4, 30, 66);
         padding:0px;
         border-top: rgb(203, 160, 82) 2px solid;
         border-bottom: transparent 2px solid;
         border-left: rgb(203, 160, 82) 2px solid;
         border-right: rgb(203, 160, 82) 2px solid;
         border-radius:5px 5px 0% 0%;
         cursor:pointer;
         Position: absolute;
         top: 100px;
         left:-200px;
         background-color: none;
         -ms-transform: rotate(90deg);
         transform: rotate(90deg);
         font-size:20px;
         color:rgb(203, 160, 82);
         transition: left .5s;
         " onclick="openNav()">
                &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Filter&nbsp;

    </span>-->
       <!-- panes: [
             {
                 cascadePanes: 'true',
                 name: 'Product', header: 'Product',options: [

                     { label: 'P001-Light Duty', value: function (rowData, rowIdx) { return rowData['Product'].includes('P001-Light Duty');}},
                     { label: 'P002-Mid Rise', value: function (rowData, rowIdx) { return rowData['Product'].includes('P002-Mid Rise');}},
                     { label: 'P003-High Rise', value: function (rowData, rowIdx) { return rowData['Product'].includes('P003-High Rise');}},
                     { label: 'P004-Heavy Duty', value: function (rowData, rowIdx) { return rowData['Product'].includes('P004-Heavy Duty');}},
                     { label: 'P005-Gen360', value: function (rowData, rowIdx) { return rowData['Product'].includes('P005-Gen360');}},
                 ],

             }
         ],-->
    <span id= "newbtn" style=" padding:0px;border-top: rgb(4, 30, 66) 1px solid; border-bottom: rgb(4, 30, 66) 1px solid; transition: left .5s; border-left: rgb(4, 30, 66) 1px solid;border-radius:100% 100% 0% 0%;	border-right: rgb(4, 30, 66) 2px solid;cursor:pointer;Position: fixed;top: 50%;left: 0px;background-color: none;font-size:20px;color:white;" onclick="openNav()">
    </span>
   </div>
	

   
	<!-- Bookmark Script-->




	<!-- Bookmark Script ends-->
  </body>
</html>
