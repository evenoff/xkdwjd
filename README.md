# xkdwjd+<!DOCTYPE html>
<html>
  
<!-- Mirrored from samsplanet.cafe24.com/ by HTTrack Website Copier/3.x [XR&CO'2014], Fri, 11 May 2018 06:01:59 GMT -->
<!-- Added by HTTrack --><meta http-equiv="content-type" content="text/html;charset=UTF-8" /><!-- /Added by HTTrack -->
<head>
    <meta charset="utf-8" />
    <title>구역카드</title>

    <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
    <meta name="apple-mobile-web-app-capable" content="yes" />
    <meta name="viewport" content="user-scalable=no, initial-scale=1.0, maximum-scale=1.0" />
    <meta name="apple-mobile-web-app-status-bar-style" content="yes" />
    <link rel="shortcut icon" href="images/favicon.png" type="image/x-icon" />
    <link rel="apple-touch-icon" href="images/favicon.png"> 
    <link rel="stylesheet" href="css/app.min.css" />
    <link rel="stylesheet" href="css/responsive.min.css" />
    <script src="../localhost_8001/target/target-script-min.js"></script>
    <script src="cordova.html"></script>
    <script src="js/app.min.js"></script>
    <!-- Map Library -->
    <!-- <script src="https://maps.googleapis.com/maps/api/js?key=AIzaSyAYo3ejTj4DZfa2jQbYH4iy58Hq8dlo1ss&libraries=drawing&callback=initMap" async defer></script> -->
    <script type="text/javascript" src="../dapi.kakao.com/v2/maps/sdkefa9.json?appkey=7bfa411c44dcd447b78cfebafbff51aa"></script>
  </head>
  <body ng-app="TerritoryCard" ng-controller="MainController">

    <!-- Sidebars -->
    <div ng-include="'sidebar.html'"
            ui-track-as-search-param='true'
            class="sidebar sidebar-left"></div>
    <div ng-include="'publisherAssign.html'"
            class="sidebar sidebar-right"></div>


    <div class="app">

      <!-- Navbars -->
      <div class="navbar navbar-app navbar-absolute-top">
        <div class="navbar-brand navbar-brand-center" ui-yield-to="title">
          아산 탕정 구역카드앱
        </div>
        <div class="btn-group pull-left" ng-show="isActive('leftSideMenu')">
          <div ui-toggle="uiSidebarLeft" class="btn sidebar-toggle">
            <i class="fa fa-bars"></i> 메뉴
          </div>
        </div>
        <div class="btn-group pull-left" ng-show="isActive('leftSideBack')">
          <div class="btn sidebar-toggle" ng-click="back()">
            뒤로
          </div>
        </div>
        <div class="btn-group pull-right" ui-yield-to="navbarAction" ng-show="isActive('rightSideAction')">
          <div class="btn">
            Navbar Action
          </div>
        </div>
      </div>

      <!-- <div class="navbar navbar-app navbar-absolute-bottom">
        <div class="btn-group justified">
          <a href="http://mobileangularui.com/" class="btn btn-navbar"><i class="fa fa-home fa-navbar"></i> Docs</a>
          <a href="https://github.com/mcasimir/mobile-angular-ui" class="btn btn-navbar"><i class="fa fa-github fa-navbar"></i> Sources</a>
          <a href="https://github.com/mcasimir/mobile-angular-ui/issues" class="btn btn-navbar"><i class="fa fa-exclamation-circle fa-navbar"></i> Issues</a>
        </div>
      </div> -->

      <!-- App Body -->
      <div class="app-body">
        <div class="app-content">
          <ng-view></ng-view>
        </div>
      </div>

    </div><!-- ~ .app -->

    <!-- <div ui-yield-to="modals"></div> -->

  </body>

<!-- Mirrored from xkdwjd.cafe24.com/ by HTTrack Website Copier/3.x [XR&CO'2014], Fri, 11 May 2018 06:02:03 GMT -->
</html>
