<template>
<!--    <div id="home" >-->

<!--         <div  class="left">-->
<!--         <div class="image-container">-->
<!--             <h2>Graph </h2>-->
<!--             <svg class="graph" viewBox="-100 -100 200 200" xmlns="http://www.w3.org/2000/svg" @click="sendPointFromSvg">-->
<!--                        <defs>-->
<!--                            <marker id='arrow-head' orient="auto"-->
<!--                                    markerWidth='2' markerHeight='4'-->
<!--                                    refX='0.1' refY='2'>-->
<!--                                <path d='M0,0 V4 L2,2 Z' fill="black"></path>-->
<!--                            </marker>-->
<!--                        </defs>-->
<!--                        <polygon class="triangle" points="0 0, 0 20, 40 0" fill="rgb(0, 160, 223)"></polygon>-->
<!--                        <rect class="rectangle" x="0" y="-40" width="20" height="40" fill="rgb(0, 160, 223)"></rect>-->
<!--                        <path class="circle" fill="rgb(0, 160, 223)" d="M 0,-40 a 40,40 0 0 0 -40,40 L 0 0 Z"></path>-->
<!--                        <path-->
<!--                                d="M -95 0, h 190"-->
<!--                                stroke="black"-->
<!--                                stroke-width="1"-->
<!--                                marker-end="url(#arrow-head)"></path>-->
<!--                        <path-->
<!--                                d="M 0 95, v -190"-->
<!--                                stroke="black"-->
<!--                                stroke-width="1"-->
<!--                                marker-end="url(#arrow-head)"></path>-->
<!--                        <text x="92" y="-3" class="graph__inscription">x</text>-->
<!--                        <text x="3" y="-92" class="graph__inscription">y</text>-->
<!--                        <text x="12" y="-3" class="graph__inscription">R/2</text>-->
<!--                        <text x="-31" y="-3" class="graph__inscription">-R/2</text>-->
<!--                        <text x="3" y="23" class="graph__inscription">-R/2</text>-->
<!--                        <text x="3" y="-17" class="graph__inscription">R/2</text>-->
<!--                        <text x="37" y="-3" class="graph__inscription">R</text>-->
<!--                        <text x="-47" y="-3" class="graph__inscription">-R</text>-->
<!--                        <text x="3" y="43" class="graph__inscription">-R</text>-->
<!--                        <text x="3" y="-37" class="graph__inscription">R</text>-->

<!--                        <circle cx="0" cy="0" r="1.5" fill="black"></circle>-->
<!--                        <circle cx="0" cy="20" r="1.5" fill="black"></circle>-->
<!--                        <circle cx="0" cy="-20" r="1.5" fill="black"></circle>-->
<!--                        <circle cx="20" cy="0" r="1.5" fill="black"></circle>-->
<!--                        <circle cx="-20" cy="0" r="1.5" fill="black"></circle>-->
<!--                        <circle cx="40" cy="0" r="1.5" fill="black"></circle>-->
<!--                        <circle cx="-40" cy="0" r="1.5" fill="black"></circle>-->
<!--                        <circle cx="0" cy="40" r="1.5" fill="black"></circle>-->
<!--                        <circle cx="0" cy="-40" r="1.5" fill="black"></circle>-->
<!--                    </svg>-->
<!--         </div>-->
<!--     </div >-->


<!--          <div  class="right">-->
<!--              <h2 style="text-align: center">Input Data From here: </h2>-->
<!--                  <div class="X-input">-->
<!--                      <label class="lable_xyr">X: </label>-->

<!--                      <input class="x-radio" id="x-radio1" type="radio" name="xval" value="-4" v-model="x">-->
<!--                      <label class="xbox-label" for="x-radio1">-4</label>-->

<!--                      <input class="x-radio" id="x-radio2" type="radio" name="xval" value="-3" v-model="x">-->
<!--                      <label class="xbox-label" for="x-radio2">-3</label>-->

<!--                      <input class="x-radio" id="x-radio3" type="radio" name="xval" value="-2" v-model="x">-->
<!--                      <label class="xbox-label" for="x-radio3">-2</label>-->

<!--                      <input class="x-radio" id="x-radio4" type="radio" name="xval" value="-1" v-model="x">-->
<!--                      <label class="xbox-label" for="x-radio4">-1</label>-->

<!--                      <input class="x-radio" id="x-radio5" type="radio" name="xval" value="0" v-model="x">-->
<!--                      <label class="xbox-label" for="x-radio5">0</label>-->

<!--                      <input class="x-radio" id="x-radio6" type="radio" name="xval" value="1" v-model="x">-->
<!--                      <label class="xbox-label" for="x-radio6">1</label>-->

<!--                      <input class="x-radio" id="x-radio7" type="radio" name="xval" value="2" v-model="x">-->
<!--                      <label class="xbox-label" for="x-radio7">2</label>-->

<!--                      <input class="x-radio" id="x-radio8" type="radio" name="xval" value="3" v-model="x">-->
<!--                      <label class="xbox-label" for="x-radio8">3</label>-->

<!--                      <input class="x-radio" id="x-radio9" type="radio" name="xval" value="4" v-model="x">-->
<!--                      <label class="xbox-label" for="x-radio9">4</label>-->
<!--                  </div>-->
<!--                  <br>-->
<!--                  <div class="Y-Input">-->
<!--                      <label class="lable_xyr label_y">Y:  </label>-->
<!--                      <input id="y-textinput" type="text" name="yval" maxlength="9" autocomplete="off" placeholder="Number from -3 to 5" v-model="y">-->
<!--                  </div>-->
<!--                  <br>-->

<!--                  <div class="R-input">-->
<!--                      <label class="lable_xyr">R: </label>-->

<!--                      <input class="x-radio" id="r-radio1" type="radio" name="rval" value="-5" v-model="r">-->
<!--                      <label class="xbox-label" for="r-radio1">-5</label>-->

<!--                      <input class="x-radio" id="r-radio2" type="radio" name="rval" value="-4" v-model="r">-->
<!--                      <label class="xbox-label" for="r-radio2">-4</label>-->

<!--                      <input class="x-radio" id="r-radio3" type="radio" name="rval" value="-3" v-model="r">-->
<!--                      <label class="xbox-label" for="r-radio3">-3</label>-->

<!--                      <input class="x-radio" id="r-radio4" type="radio" name="rval" value="-2" v-model="r">-->
<!--                      <label class="xbox-label" for="r-radio4">-2</label>-->

<!--                      <input class="x-radio" id="r-radio5" type="radio" name="rval" value="-1" v-model="r">-->
<!--                      <label class="xbox-label" for="r-radio5">-1</label>-->

<!--                      <input class="x-radio" id="r-radio6" type="radio" name="rval" value="0" v-model="r">-->
<!--                      <label class="xbox-label" for="r-radio6">0</label>-->

<!--                      <input class="x-radio" id="r-radio7" type="radio" name="rval" value="1" v-model="r">-->
<!--                      <label class="xbox-label" for="r-radio7">1</label>-->

<!--                      <input class="x-radio" id="r-radio8" type="radio" name="rval" value="2" v-model="r">-->
<!--                      <label class="xbox-label" for="r-radio8">2</label>-->

<!--                      <input class="x-radio" id="r-radio9" type="radio" name="rval" value="3" v-model="r">-->
<!--                      <label class="xbox-label" for="r-radio9">3</label>-->

<!--                      <div class="buttons">-->
<!--                          <button class="button-submit" type="submit" name="Submit" @click="submitForm">Submit</button>-->
<!--                          <button class="button-reset" type="reset" name="Reset" @click="resetPoints">Reset</button>-->
<!--                          <button class="button-logout" name="logout" @click="logout">Logout</button>-->
<!--                      </div>-->
<!--                  </div>-->
<!--          </div>-->
<!--        </div>-->

<!--        <div id="maintable">-->
<!--            <div class="table">-->
<!--               <table style="width: 100%">-->
<!--                   <br>-->
<!--                       <div class="plate-top">-->
<!--                           <h2 class="plate-top-title"> Table </h2>-->
<!--                       </div>-->

<!--                       <div class="scroll-container">-->
<!--                           <table id="result-table">-->
<!--                               <tr class="table-header">-->
<!--                                   <th class="coords-col"> X </th>-->
<!--                                   <th class="coords-col">Y</th>-->
<!--                                   <th class="coords-col">R</th>-->
<!--                                   <th class="hitres-col"> Hit result</th>-->
<!--                                   <th class="time-col"> Excution time</th>-->
<!--                               </tr>-->
<!--                                <tr v-for="point in points" :key="point">-->
<!--                                    <td class="coords-col">{{point.x.toFixed(3)}}</td>-->
<!--                                    <td class="coords-col">{{point.y.toFixed(3)}}</td>-->
<!--                                    <td class="coords-col">{{point.r}}</td>-->
<!--                                    <td class="hitres-col">{{point.hitResult}}</td>-->
<!--                                    <td class="time-col">{{point.time}}</td>-->
<!--                                </tr>-->
<!--                           </table>-->
<!--                       </div>-->
<!--               </table>-->
<!--            </div>-->
<!--        </div>-->








  <table id = "main-grid">

    <tr>
      <!--Graph-->
      <td class="content-plate" id ="graph-plate">
        <div class="plate-top">
          <h2 class="plate-top-title">Graph</h2>
        </div>
        <svg class="graph" viewBox="-200 -200 400 400" xmlns="http://www.w3.org/2000/svg" @click="sendPointFromSvg">
          <defs>
            <marker id='arrow-head' orient="auto"
                    markerWidth='2' markerHeight='4'
                    refX='0.1' refY='2'>
              <path d='M0,0 V4 L2,2 Z' fill="black"></path>
            </marker>
          </defs>
          <polygon class="triangle" points="0 0, 0 -40, 40 0" fill="rgb(139, 153, 226)"></polygon>
          <rect class="rectangle" x="-40" y="0" width="40" height="20" fill="rgb(139, 153, 226)"></rect>
          <path class="circle" fill="rgb(139, 153, 226)" d="M 0,-20 a 20,20 0 0 0 -20,20 L 0 0 Z"></path>
          <path
              d="M -195 0, h 390"
              stroke="black"
              stroke-width="1"
              marker-end="url(#arrow-head)"></path>
          <path
              d="M 0 195, v -390"
              stroke="black"
              stroke-width="1"
              marker-end="url(#arrow-head)"></path>
          <text x="192" y="-3" class="graph__inscription">x</text>
          <text x="3" y="-192" class="graph__inscription">y</text>
          <text x="12" y="-3" class="graph__inscription_r2_x">R/2</text>
          <text x="-31" y="-3" class="graph__inscription_-r2_x">-R/2</text>
          <text x="3" y="23" class="graph__inscription_-r2_y">-R/2</text>
          <text x="3" y="-17" class="graph__inscription_r2_y">R/2</text>
          <text x="37" y="-3" class="graph__inscription_r_x">R</text>
          <text x="-47" y="-3" class="graph__inscription_-r_x">-R</text>
          <text x="3" y="43" class="graph__inscription_-r_y">-R</text>
          <text x="3" y="-37" class="graph__inscription_r_y">R</text>

          <circle cx="0" cy="0" r="1.5" fill="black"></circle>
          <circle cx="0" cy="20" r="1.5" fill="black" class="dot_y"></circle>
          <circle cx="0" cy="-20" r="1.5" fill="black" class="dot_y"></circle>
          <circle cx="20" cy="0" r="1.5" fill="black" class="dot_x"></circle>
          <circle cx="-20" cy="0" r="1.5" fill="black" class="dot_x"></circle>
          <circle cx="40" cy="0" r="1.5" fill="black" class="dot_x2"></circle>
          <circle cx="-40" cy="0" r="1.5" fill="black" class="dot_x2"></circle>
          <circle cx="0" cy="40" r="1.5" fill="black" class="dot_y2"></circle>
          <circle cx="0" cy="-40" r="1.5" fill="black" class="dot_y2"></circle>
        </svg>

      </td>

      <!--Table-->
      <td class="content-plate" id = "table-plate" rowspan="2">
        <div class="plate-top">
          <h2 class="plate-top-title"> Table </h2>
        </div>

        <div class="scroll-container">
          <table id="result-table">
            <tr class="table-header">
              <th class="coords-col"> X </th>
              <th class="coords-col">Y</th>
              <th class="coords-col">R</th>
              <th class="hitres-col"> Hit result</th>
              <th class="time-col"> Excution time</th>
            </tr>

            <tr v-for="point in points" :key="point">
              <td class="coords-col">{{point.x.toFixed(3)}}</td>
              <td class="coords-col">{{point.y.toFixed(3)}}</td>
              <td class="coords-col">{{point.r}}</td>
              <td class="hitres-col">{{point.hitResult}}</td>
              <td class="time-col">{{point.time}}</td>
            </tr>



          </table>
        </div>
      </td>
    </tr>



    <tr>
      <!--Values-->
      <td class="content-plate" id="values-plate">
        <div class="plate-top">
          <h2 class="plate-top-title"> Values </h2>
        </div>

        <form id="input-form" action="" method="POST">
          <table id="input-grid">
            <!--X Values-->
            <tr>
              <td class="input-grid-label">
                <label>X: </label>
              </td>

              <td class="input-grid-value x-radio-group">

                <div class="center-labeled">
                    <select name="xval" class="r-checkbox" v-model="x"  >
                      <option value="-4" >-4</option>
                      <option value="-3" >-3</option>
                      <option value="-2" >-2</option>
                      <option value="-1" >-1</option>
                      <option value="0" >0</option>
                      <option value="1" >1</option>
                      <option value="2" >2</option>
                      <option value="3" >3</option>
                      <option value="4" >4</option>
                    </select>
                </div>
              </td>
            </tr>

            <!--Y VALUES-->

            <tr>
              <td class="input-grid-label">
                <label class="lable_xyr label_y">Y:  </label>
<!--                <label for="y-textinput">Y: </label>-->
              </td>
              <td class="input-grid-value">
                <input id="y-textinput" type="text" name="yval" maxlength="11" autocomplete="off" placeholder="Number from -5 to 5" v-model="y">
              </td>
            </tr>


            <!--R Value-->
            <tr>
              <td class="input-grid-label">
                <label>R: </label>
              </td>


              <td class="input-grid-value">
                <div class="center-labeled">
                  <select name="rval" class="r-checkbox" v-model="r"  >
                    <option value="-4" >-4</option>
                    <option value="-3" >-3</option>
                    <option value="-2" >-2</option>
                    <option value="-1" >-1</option>
                    <option value="0" >0</option>
                    <option value="1" >1</option>
                    <option value="2" >2</option>
                    <option value="3" >3</option>
                    <option value="4" >4</option>
                  </select>
                </div>
              </td>
            </tr>


            <!--Buttons-->
            <tr  >
              <td colspan="3">
                <div class="buttons">
                  <input class="button-submit" type="submit" name="Submit" @click="submitForm">
                  <input  class="button-reset" type="reset" name="Reset" @click="resetPoints">
                  <input class="button-logout" type="logout" name="Logout" @click="logout">
<!--                  <input class="button-submit" type="submit" name="Submit" @click="submitForm">-->
<!--                  <input class="button-reset" type="reset" name="Reset" @click="resetPoints">-->
<!--                  <input class="button-logout" type="" name="Logout" @click="logout">-->
                </div>
              </td>
            </tr>
          </table>
        </form>
      </td>
    </tr>
  </table>








<!--          </div>-->


</template>

<script>
export default {
    name: "Main",
    data(){
        return {
            x: "-4",
            y: "-5",
            r: "-4",
            points: new Array()
        }
    },
    watch: {
        y(value) {
            const buttonSubmit = document.querySelector(".button-submit");
            const yTextInput = document.querySelector(".label_y");
            if (!isNaN(parseFloat(value)) && isFinite(value) && value <= 5 && value >= -5) {
                buttonSubmit.disabled = false;
                buttonSubmit.style.border = "2px solid #c5e29a"
                yTextInput.style.backgroundColor = "#c5e29a"
            } else {
                buttonSubmit.disabled = true;
                buttonSubmit.style.border = "2px solid #B00020";
                yTextInput.style.backgroundColor = "#B00020"
            }
        
        },
        r(value) {
          if (value > 0) {
            const rectangle = document.querySelector('.rectangle')
            document.querySelector('.triangle').setAttribute("points", `0 0, 0 ${-40 * value}, ${40 * value} 0`);
            document.querySelector('.circle').setAttribute("d", `M 0,${-20 * value} a ${20 * value},${20 * value} 0 0 0 ${-20 * value},${20 * value} L 0 0 Z`);
            rectangle.setAttribute("x", -40 * value);
            rectangle.setAttribute("width", 40 * value);
            rectangle.setAttribute("height", 20 * value);

            document.querySelector('.graph__inscription_r2_x').setAttribute("x", 12*value);
            document.querySelector('.graph__inscription_-r2_x').setAttribute("x", -31*value);
            document.querySelector('.graph__inscription_-r2_y').setAttribute("y", 23*value);
            document.querySelector('.graph__inscription_r2_y').setAttribute("y", -17*value);
            document.querySelector('.graph__inscription_r_x').setAttribute("x", 37*value);
            document.querySelector('.graph__inscription_-r_x').setAttribute("x", -47*value);
            document.querySelector('.graph__inscription_-r_y').setAttribute("y", 43*value);
            document.querySelector('.graph__inscription_r_y').setAttribute("y", -37*value);

            document.querySelectorAll('.dot_x').forEach(dot => {
              dot.setAttribute("cx", (parseInt(dot.getAttribute("cx")) > 0 ? 20 : -20) * value);
            });
            document.querySelectorAll('.dot_y').forEach(dot => {
              dot.setAttribute("cy", (parseInt(dot.getAttribute("cy")) > 0 ? 20 : -20) * value);
            });
            document.querySelectorAll('.dot_x2').forEach(dot => {
              dot.setAttribute("cx", (parseInt(dot.getAttribute("cx")) > 0 ? 40 : -40) * value);
            });
            document.querySelectorAll('.dot_y2').forEach(dot => {
              dot.setAttribute("cy", (parseInt(dot.getAttribute("cy")) > 0 ? 40 : -40) * value);
            });
          }
        }
    },
  mounted() {
    this.getPoints();
  },
    methods: {
        submitForm(event) {
            event.preventDefault();
            const userDetails = JSON.parse(localStorage.getItem("userDetails"));
            if (userDetails) {
                this.axios.post("https://boiling-headland-85483.herokuapp.com/points ", {
                    x: this.x,
                    y: this.y,
                    r: this.r
                },
                {
                    headers: {"Authorization": "Bearer " + userDetails.accessToken}
                }).then(() => {
                    this.getPoints();
                }).catch(error => {
                    if (error.response.status === 401 || error.response.status === 403) {
                        this.invalidateTokenAndGoToAuthPage();
                    }
                })
            } else this.invalidateTokenAndGoToAuthPage();
        },
        resetPoints(event) {
            event.preventDefault();
            this.axios.delete("https://boiling-headland-85483.herokuapp.com/points/",
            {
                headers: {"Authorization": "Bearer " + JSON.parse(localStorage.getItem("userDetails")).accessToken}
            }).then(() => {
                this.getPoints();
                this.drawPoints();
            }).catch(error => {
                if (error.response.status === 401 || error.response.status === 403) {
                    this.invalidateTokenAndGoToAuthPage();
                }
            })
        },
        getPoints() {
            const userDetails = JSON.parse(localStorage.getItem("userDetails"));
            this.axios.get("https://boiling-headland-85483.herokuapp.com/points/", {
                headers: {"Authorization": "Bearer " + userDetails.accessToken}
            }).then(response => {
                this.points = this.getPointsListFromResponse(response.data)
                this.drawPoints();
            }).catch(error => {
                alert(error.message);
                if (error.response.status === 401 || error.response.status === 403) {
                    this.invalidateTokenAndGoToAuthPage();
                }
            })
        },
        getPointsListFromResponse(json) {
            let pointsUnwraped = new Array();
            if (json._embedded !== undefined) {
                for (let jsonObj of json._embedded.pointList) {
                    pointsUnwraped.push((({ x, y, r, hitResult, time }) => ({ x, y, r, hitResult, time }))(jsonObj))
                }
            }
            return pointsUnwraped;
        },
        invalidateTokenAndGoToAuthPage() {
            localStorage.removeItem("userDetails");
            this.$router.push({name: "auth"});
        },
        drawPoints() {
          const svg = document.querySelector('.graph');
          document.querySelectorAll('.circle--point').forEach(point => point.remove());

          if (this.points) {
            for (let point of this.points) {
                const circleElement = document.createElementNS("http://www.w3.org/2000/svg", "circle");
                circleElement.classList.add('circle--point');
                circleElement.setAttribute("cx", point.x*40);
                circleElement.setAttribute("cy", -point.y*40);
                circleElement.setAttribute("r", 1);
                circleElement.setAttribute("fill", point.hitResult ? "green" : "red");
                svg.appendChild(circleElement);
            }
          }
        },
        sendPointFromSvg(event) {
            event.preventDefault();
            const svg = document.querySelector('.graph');
            const pt = svg.createSVGPoint();

            pt.x = event.clientX;
            pt.y = event.clientY;
            let loc = pt.matrixTransform(svg.getScreenCTM().inverse());

            let xSvg = loc.x/40;
            let ySvg = -loc.y/40;

            this.axios.post("https://boiling-headland-85483.herokuapp.com/points", {
                x: xSvg,
                y: ySvg,
                r: this.r
            },
            {
                headers: {"Authorization": "Bearer " + JSON.parse(localStorage.getItem("userDetails")).accessToken}
            }).then(() => {
                this.getPoints();
            }).catch(error => {
                if (error.response.status === 401) {
                    this.invalidateTokenAndGoToAuthPage();
                }
            })
        },
        logout(event) {
            event.preventDefault();
            localStorage.removeItem("userDetails");
            this.$router.push({name: "auth"});
        }
    }
}

</script>

<style scoped>
body{
  font-size: 16px;
  font-family: "Open Sans", "Arial", sans-serif;
  background-color: snow;
}
#main-grid {
  width: 95%;
  margin: auto;
  border-spacing: 1em;
}
#table-plate {
  width: 65%;
}

.content-plate {
  padding: 0 0 20px;
  vertical-align: top;
  background: snow;
  border-radius: 4px;
  box-shadow: rgba(60, 66, 87, 0.12) 0px 7px 14px 0px, rgba(0, 0, 0, 0.12) 0px 3px 6px 0px;

}

.plate-top {
  display: inline-block;
  width: 100%;
  margin: 0;
  margin-bottom: 20px;
  padding: 0em 0;
  text-align: center;
  color: whitesmoke;
  background-color: #5469d4;
}

.plate-top-title {
  font-size: 18px;
  font-weight: normal;
}

#input-grid {
  width: 95%;
  margin: auto;
  height: auto;
  text-align: center;
}

.input-grid-label {
  width: 12%;
  font-weight: bold;
  /*height: auto;*/
}
#y-textinput {
  width: 75%;
  height: 20px;
  margin: 2% 0;
}
.r-checkbox{
  width: 78%;
  height: 25px;
  margin: 2% 0;
}
.center-labeled {
  display: inline-block;
  position: relative;
  margin: 0 1% 5%;
  width: 100%;
  font-size: 14px;
}

.center-labeled label {
  position: absolute;
  top: 18px;
  left: 6px;
}

/*.button-submit,.button-reset,.button-logout {*/
/*  margin-top: 2%;*/
/*}*/

.button-submit,.button-reset,.button-logout::before {
  content: "";

  display: inline-block;
  height: auto;
  width: 70px;
  background-color: #1a1f36;
  /*padding: 1%;*/
  margin: 0 auto 4% 1%;
}

.button-submit,.button-reset,.button-logout {
  height: 27px;
  width: 80px;
  margin-left: 1%;
  font-family: "Open Sans", "Arial", sans-serif;
  color: #ffffff;
  background-color: #1a1f36;
  border: none;
}

.button-submit,.button-reset,.button-logout:hover {
  font-weight: 15;
  background-color: #1a1f36;
}
/*.button-logout{*/
/*  padding: 0;*/
/*  font-weight: 50;*/
/*}*/

#table-plate {
  position: relative;
}

.scroll-container {
  position: absolute;
  bottom: 0;
  right: 0;
  top: 54px;
  width: 100%;
  overflow-y: scroll;
}

#result-table {
  width: 100%;
  text-align: center;
  border-collapse: collapse;
}

#result-table tr {
  height: 2em;
}

#result-table tr:nth-child(2n-1) {
  background-color: #8bb5ea;
}

#result-table tr:nth-child(2n):hover {
  background-color: #8b99e2;
}

#result-table tr:nth-child(2n-1):hover {
  background-color: #d2d8f4;
}

#result-table tr.table-header:hover {
  background-color: #8b99e2;
}

.coords-col {
  width: 12%;
}

.time-col {
  width: 25%;
}
.graph{
  width: auto;
  font-weight: 16;
  /*margin-left: 20%;*/
  height: auto;
}

</style>