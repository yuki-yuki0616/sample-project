# sample-project

�ۑ�2�Ŋ��������\�[�X�R�[�h�ł��B

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
 zoom: 15,      //�n�}�̏k�ڒl
 center: MyLatLng,    //�n�}�̒��S���W
 mapTypeId: 'roadmap'   //�n�}�̎��
};
var map = new google.maps.Map(document.getElementById('map'), Options);
marker = new google.maps.Marker({ // �}�[�J�[�̒ǉ�
        position: MyLatLng, // �}�[�J�[�𗧂Ă�ʒu���w��
      map: map // �}�[�J�[�𗧂Ă�n�}���w��
   });
</script>

</body>
</html>
