#卡券效果
.coupon{
  width: 300px;
  height: 100px;
  position: relative;
  background: radial-gradient(circle at right bottom, transparent 10px, #ffffff 0) top right /50% 51px no-repeat,
    radial-gradient(circle at left bottom, transparent 10px, #ffffff 0) top left / 50% 51px no-repeat,
    radial-gradient(circle at right top, transparent 10px, #ffffff 0) bottom right / 50% 51px no-repeat,
    radial-gradient(circle at left top, transparent 10px, #ffffff 0) bottom left / 50% 51px no-repeat;
  filter: drop-shadow(2px 2px 2px rgba(0,0,0,.2));
}
#气泡阴影
.tip {
    width: 100px;
    height: 30px;
    line-height: 30px;
    border: 1px solid rgb(245, 129, 127);
    border-radius: 4px;
    position: relative;
    background-color: #fff;
    filter: drop-shadow(0px 2px 4px rgba(245, 129, 127, 0.9));
    &::before {
      content: "";
      width: 0;
      height: 0;
      border-style: solid;
      border-width: 0 10px 10px 10px;
      border-color: transparent transparent #fff transparent;
      position: absolute;
      top: -10px;
      left: 0;
      right: 0;
      margin: auto;
      z-index: 2;
    }
    &::after {
      content: "";
      width: 0;
      height: 0;
      border-style: solid;
      border-width: 0 10px 10px 10px;
      border-color: transparent transparent rgb(245, 129, 127) transparent;
      position: absolute;
      top: -11px;
      left: 0;
      right: 0;
      margin: auto;
      z-index: 1;
    }
}