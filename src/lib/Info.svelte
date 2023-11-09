<script>
let data = {
  ip: '192,212,174,101',
  location: 'Brookelyn,Ny 10001',
  timeZone: 'UTC-05:00',
  isp: 'SpaceX Starlink'
};
</script>
<div class="d-flex justify-content-center">
    <div class="info bg-white pt-3 px-4 row rounded-3 position-absolute">
        <div class="ip col-sm-6 col-xl-3">
            <h5>IP ADDRESS</h5>
            <p>{data.ip}</p>
        </div>
        <div class="location col-sm-6 col-xl-3">
            <h5>LOCATION</h5>
            <p>{data.location}</p>
        </div>
        <div class="time-zone col-sm-6 col-xl-3">
            <h5>TIMEZONE</h5>
            <p>{data.timeZone}</p>
        </div>
        <div class="isp col-sm-6 col-xl-3">
            <h5>ISP</h5>
            <p>{data.isp}</p>
        </div>
    </div>
</div>

<style>
.info {
  max-width: 90%;
  box-shadow: 0px 5px 8px 0 rgb(0 0 0 / 32%);
}

.info h5 {
  padding-top: 0.5em;
  color: hsl(0, 0%, 59%);
  text-align: center;
  font-size: clamp(0.9em, 4vw, 1.2em);
}

.info p {
  font-weight: 500;
  text-align: center;
  font-size: clamp(1.3em, 5vw, 1.7em);
}

@media (max-width : 576px) {
  .info {
    max-width: 90%;
    box-shadow: 0px 5px 8px 0 rgb(0 0 0 / 32%);
  }
}

@media (min-width : 577px) {
  .info {
    width: clamp(40em, 90vw, 80em);
  }
}

@media (min-width : 1201px) {
  .info p {
    max-width: 10ch;
    text-align: left;
  }

  .info h5 {
    text-align: left;
  }

  .ip,
  .location,
  .time-zone {
    position: relative;
  }

  .ip::after,
  .location::after,
  .time-zone::after {
    content: '';
    width: 2px;
    height: 50%;
    top : 25%;
    right : 3em ;
    position: absolute;
    background-color: hsla(0, 0%, 59%, 0.458);
  }
}
</style>
