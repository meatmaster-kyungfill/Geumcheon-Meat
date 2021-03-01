# Geumcheon-Meat 장바구니 분석

## 장바구니 분석이란


해당 금천미트 구매후기를 바탕으로한 장바구니 분석
구매후기 데이터를 얻은 금천미트
금천미트는 B2B 온라인몰으로써 회원들의 재구매율이 상당히 높다.
따라서 재구매 내역을 바탕으로 구매이력을 추정할 수 있었고
이러한 구매이력을 바탕으로 장바구니분석(상품연관분석)을 진행하였다.
![image](https://user-images.githubusercontent.com/71205453/109490613-cd861b80-7acb-11eb-8ef0-0bbd0bcc5fc5.png)
![image](https://user-images.githubusercontent.com/71205453/109490889-366d9380-7acc-11eb-8495-595c6f442f4f.png)

<div class="output_subarea output_html rendered_html output_result" dir="auto"><div>
<style scoped="">
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>antecedents</th>
      <th>consequents</th>
      <th>support</th>
      <th>confidence</th>
      <th>lift</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>11</th>
      <td>(부위3_양지(치마)</td>
      <td>(부위4_업진))</td>
      <td>0.013245</td>
      <td>1.000000</td>
      <td>75.500000</td>
    </tr>
    <tr>
      <th>12</th>
      <td>(부위4_업진))</td>
      <td>(부위3_양지(치마)</td>
      <td>0.013245</td>
      <td>1.000000</td>
      <td>75.500000</td>
    </tr>
    <tr>
      <th>9</th>
      <td>(부위2_양지(치마)</td>
      <td>(부위3_업진))</td>
      <td>0.016556</td>
      <td>1.000000</td>
      <td>60.400000</td>
    </tr>
    <tr>
      <th>10</th>
      <td>(부위3_업진))</td>
      <td>(부위2_양지(치마)</td>
      <td>0.016556</td>
      <td>1.000000</td>
      <td>60.400000</td>
    </tr>
    <tr>
      <th>16</th>
      <td>(부위14_갈비)</td>
      <td>(부위13_사태)</td>
      <td>0.013245</td>
      <td>0.800000</td>
      <td>48.320000</td>
    </tr>
    <tr>
      <th>15</th>
      <td>(부위13_사태)</td>
      <td>(부위14_갈비)</td>
      <td>0.013245</td>
      <td>0.800000</td>
      <td>48.320000</td>
    </tr>
    <tr>
      <th>5</th>
      <td>(부위2_업진))</td>
      <td>(부위1_양지(치마)</td>
      <td>0.039735</td>
      <td>1.000000</td>
      <td>25.166667</td>
    </tr>
    <tr>
      <th>6</th>
      <td>(부위1_양지(치마)</td>
      <td>(부위2_업진))</td>
      <td>0.039735</td>
      <td>1.000000</td>
      <td>25.166667</td>
    </tr>
    <tr>
      <th>13</th>
      <td>(부위6_삼겹살)</td>
      <td>(부위5_삼겹)</td>
      <td>0.013245</td>
      <td>0.666667</td>
      <td>25.166667</td>
    </tr>
    <tr>
      <th>14</th>
      <td>(부위9_항정)</td>
      <td>(부위5_안심)</td>
      <td>0.013245</td>
      <td>0.800000</td>
      <td>21.963636</td>
    </tr>
    <tr>
      <th>20</th>
      <td>(부위3_목심(암))</td>
      <td>(부위1_미박삼겹(암), 부위2_목심)</td>
      <td>0.019868</td>
      <td>0.666667</td>
      <td>20.133333</td>
    </tr>
    <tr>
      <th>19</th>
      <td>(부위1_미박삼겹(암), 부위2_목심)</td>
      <td>(부위3_목심(암))</td>
      <td>0.019868</td>
      <td>0.600000</td>
      <td>20.133333</td>
    </tr>
    <tr>
      <th>22</th>
      <td>(부위1_미박삼겹(암), 부위3_삼겹(암))</td>
      <td>(부위2_목심(암))</td>
      <td>0.016556</td>
      <td>1.000000</td>
      <td>15.894737</td>
    </tr>
    <tr>
      <th>8</th>
      <td>(부위6_삼겹살)</td>
      <td>(부위2_삼겹양지)</td>
      <td>0.013245</td>
      <td>0.666667</td>
      <td>13.422222</td>
    </tr>
    <tr>
      <th>0</th>
      <td>(부위6_삼겹살)</td>
      <td>(부위1_목살)</td>
      <td>0.013245</td>
      <td>0.666667</td>
      <td>13.422222</td>
    </tr>
    <tr>
      <th>18</th>
      <td>(부위3_목심(암), 부위2_목심)</td>
      <td>(부위1_미박삼겹(암))</td>
      <td>0.019868</td>
      <td>1.000000</td>
      <td>10.413793</td>
    </tr>
    <tr>
      <th>17</th>
      <td>(부위3_목심(암), 부위1_미박삼겹(암))</td>
      <td>(부위2_목심)</td>
      <td>0.019868</td>
      <td>0.857143</td>
      <td>10.354286</td>
    </tr>
    <tr>
      <th>3</th>
      <td>(부위3_목심(암))</td>
      <td>(부위1_미박삼겹(암))</td>
      <td>0.023179</td>
      <td>0.777778</td>
      <td>8.099617</td>
    </tr>
    <tr>
      <th>7</th>
      <td>(부위3_목심(암))</td>
      <td>(부위2_목심)</td>
      <td>0.019868</td>
      <td>0.666667</td>
      <td>8.053333</td>
    </tr>
    <tr>
      <th>21</th>
      <td>(부위2_목심(암), 부위3_삼겹(암))</td>
      <td>(부위1_미박삼겹(암))</td>
      <td>0.016556</td>
      <td>0.625000</td>
      <td>6.508621</td>
    </tr>
    <tr>
      <th>2</th>
      <td>(부위7_앞다리살)</td>
      <td>(부위1_목심)</td>
      <td>0.016556</td>
      <td>0.833333</td>
      <td>5.719697</td>
    </tr>
    <tr>
      <th>4</th>
      <td>(부위2_목살)</td>
      <td>(부위1_삼겹살)</td>
      <td>0.029801</td>
      <td>0.600000</td>
      <td>5.490909</td>
    </tr>
    <tr>
      <th>1</th>
      <td>(부위4_등뼈)</td>
      <td>(부위1_목심)</td>
      <td>0.013245</td>
      <td>0.666667</td>
      <td>4.575758</td>
    </tr>
  </tbody>
</table>
</div></div>
