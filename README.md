# MUTF8Encoding

<h1>编码原理</h1>
<table>
  <tbody>
    <tr>
      <th>字符范围</th>
      <th>表示位数</th>
      <th>占用字节</th>
      <th>字符集</th>
      <th>表示</th>
    </tr>
    <tr>
      <td>0</td>
      <td>11</td>
      <td>2</td>
      <td></td>
      <td>11010000 10000000</td>
    </tr>
    <tr>
      <td>0x0001 - 0x007F</td>
      <td>7</td>
      <td>1</td>
      <td>ACII</td>
      <td>0XXXXXXX</td>
    </tr>
    <tr>
      <td>0x0080 - 0x07FF</td>
      <td>11</td>
      <td>2</td>
      <td>UNICODE</td>
      <td>110XXXXX 10XXXXXX</td>
    </tr>
    <tr>
      <td>0x0800 - 0xFFFF</td>
      <td>16</td>
      <td>3</td>
      <td>UNICODE</td>
      <td>1110XXXX 10XXXXXX 10XXXXXX</td>
    </tr>
  </tbody>
</table>
