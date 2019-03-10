# sample-project

課題2で完了したソースコードです。

<!DOCTYPE html>
<html lang="ja">

<head>
<meta charset="UTF-8">
<title>Sample_GoogleMap</title>

<script src="http://maps.google.com/maps/api/js?key=AIzaSyAJv5SqWLDtQlKU43uwqbqyBk_nH7YkTkQ&language=ja"></script>

<style>
html { height: 100% }
body { height: 100% }
#map { height: 100%; width: 100%}
</style>
</head>

<body>
<div id="map"></div>

<script>
var MyLatLng = new google.maps.LatLng( 35.649591, 139.709098);
var Options = {
 zoom: 15,      //地図の縮尺値
 center: MyLatLng,    //地図の中心座標
 mapTypeId: 'roadmap'   //地図の種類
};
var map = new google.maps.Map(document.getElementById('map'), Options);
marker = new google.maps.Marker({ // マーカーの追加
        position: MyLatLng, // マーカーを立てる位置を指定
      map: map // マーカーを立てる地図を指定
   });
</script>

</body>
</html>
