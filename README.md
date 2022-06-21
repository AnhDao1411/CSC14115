| MSSV | Name |  GitHub account | Kaggle account |
| -------- | -------- | -------- | -------- |
| 18127039   | Lâm Ngọc Phương Anh     | [lnpanh](https://github.com/lnpanh) | [anhlam2109](https://www.kaggle.com/anhlam2109) |
| 18127046   | Lư Ngọc Liên     |  [Ngocien](https://github.com/Ngocien) | [linlngc](https://www.kaggle.com/linlngc) |
| 18127272   | Nguyễn Thị Anh Đào    | [AnhDao1411](https://github.com/AnhDao1411) | [anhonguynth](https://www.kaggle.com/anhonguynth) |

# New York City Taxi Trip Duration

## Problem Statement

### Overview
This is a kaggle competition that challenges us to predict the taxi trip duration in New York city. Dataset is provided by the NYC taxi and Limousine commision for building a model.

Money prize: 30,000$.

Business motivation:
- Improving traffic operations and solving bottlenecks that appear in the taxi traffic network.
- Providing user accurate time estimation to let them choose an optimized route.

Input: a taxi trip with it's attributes. \
Output: trip duration in seconds. 
 
### Input and Output Data description

There are three files:
- train.csv: (1458644,11)
- test.csv: (625134,9)
- sample_submission.csv: (625134,2) 

| Column name | Description | 
| -------- | -------- | 
| id   | the id for each trip     |
| vendor_id   | the id provided Associated with the trip record     |
| pickup_datetime   | date and time when the meter was engaged     |
| dropoff_datetime   | date and time when the meter was disengaged    |
| passenger_count   | The number of passengers in the taxi    |
| pickup_longitude   | the longitude when the meter was engaged     |
| pickup_latitude   | the latitude when the meter was engaged   |
| dropoff_longitude   | the longitude when the meter was disengaged     |
| dropoff_latitude   | the latitude when the meter was disengaged     |
| store_and_fwd_flag   | This flag indicates whether the trip record was held in vehicle memory before sending to the vendor because the vehicle did not have a connection to the server  |
| trip_duration  | duration of the trip in seconds     |


- A record in train.csv

![](https://i.imgur.com/LtLFbTO.png)

- A record in test.csv
![](https://i.imgur.com/gEJR1jT.png)

- A record in sample_submission.csv
![](https://i.imgur.com/zwq0ezw.png)



### Evaluation Metric
- **Root Mean Squared Logarithmic Error** (RMSLE) is the metric was used to assess the result of this contest.

$$\epsilon = \sqrt{\frac{1}{n}\sum^{n}_{i=1}(log(p_i + 1) -log(a_i + 1)) ^2}$$

* With respect to:
    * $\epsilon$: RMSLE score
    * n: the number of records (trip duration's observations) in the dataset
    * $p_i$: the prediction of trip duration
    * $a_i$: the actual value of trip duration
    * log(x): natural logarithm (base is e)

* **The smaller the RMSLE value is, the better the model**.


### Weekly plan
<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky"></th>
    <th class="tg-rk9a">Main task</th>
    <th class="tg-rk9a">Sub-task</th>
    <th class="tg-rk9a">Assignee</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-9hil" rowspan="5">W05</td>
    <td class="tg-9wq8" rowspan="3">Write report about problem statement</td>
    <td class="tg-0pky">Describe problem</td>
    <td class="tg-kgv7"><span style="color:#000">Nguyễn Thị Anh Đào</span></td>
  </tr>
  <tr>
    <td class="tg-0pky">Describe data</td>
    <td class="tg-kgv7"><span style="color:#000">Lư Ngọc Liên</span></td>
  </tr>
  <tr>
    <td class="tg-0pky">Describe metric</td>
    <td class="tg-kgv7"><span style="color:#000">Lâm Ngọc Phương Anh</span></td>
  </tr>
  <tr>
    <td class="tg-9wq8" rowspan="2">Refer the process of different solutions</td>
    <td class="tg-0pky">Read idea</td>
    <td class="tg-0pky">All Team</td>
  </tr>
  <tr>
    <td class="tg-0pky">Note the strong point of each idea</td>
    <td class="tg-0pky">All Team</td>
  </tr>
</tbody>
</table>
