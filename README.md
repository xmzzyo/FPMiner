# FPMiner
# FPMiner
<table class="tg">
  <tr>
    <th class="tg-0pky">Category<br></th>
    <th class="tg-0pky">Features</th>
    <th class="tg-0pky">Description</th>
  </tr>
  <tr>
    <td class="tg-uys7" rowspan="2">Term</td>
    <td class="tg-uys7">POSTAG</td>
    <td class="tg-0pky">The result of Part-Of-Speech Tagger on the word</td>
  </tr>
  <tr>
    <td class="tg-uys7">DEPREL</td>
    <td class="tg-0pky">The universal dependency relation to the word</td>
  </tr>
  <tr>
    <td class="tg-uys7" rowspan="5">Frequency</td>
    <td class="tg-uys7">TF</td>
    <td class="tg-0pky">The term frequency of the word in the whole user story</td>
  </tr>
  <tr>
    <td class="tg-s6z2">IDF</td>
    <td class="tg-0lax">The inverse document frequency of the word among all the user stories in one product</td>
  </tr>
  <tr>
    <td class="tg-s6z2">SF</td>
    <td class="tg-0lax">The term frequency of the word in the summary</td>
  </tr>
  <tr>
    <td class="tg-s6z2">DF</td>
    <td class="tg-0lax">The term frequency of the word in the description</td>
  </tr>
  <tr>
    <td class="tg-s6z2">AF</td>
    <td class="tg-0lax">The term frequency of the word in the acceptance criteria</td>
  </tr>
  <tr>
    <td class="tg-s6z2" rowspan="5">Position</td>
    <td class="tg-s6z2">SRO</td>
    <td class="tg-0lax">Whether the word appear in the content of ‘role’ in summary</td>
  </tr>
  <tr>
    <td class="tg-s6z2">SGO</td>
    <td class="tg-0lax">Whether the word appear in the content of ‘goal/desire’ in summary</td>
  </tr>
  <tr>
    <td class="tg-s6z2">SBO</td>
    <td class="tg-0lax">Whether the word appear in the content of ‘beneﬁt’ in summary</td>
  </tr>
  <tr>
    <td class="tg-s6z2">DO</td>
    <td class="tg-0lax">Whether the word appear in the content of description</td>
  </tr>
  <tr>
    <td class="tg-s6z2">AO</td>
    <td class="tg-0lax">Whether the word appear in the content of acceptance criteria</td>
  </tr>
  <tr>
    <td class="tg-s6z2" rowspan="2">History</td>
    <td class="tg-s6z2">RFP</td>
    <td class="tg-0lax">The proportion of term frequency of the word among all the words in the historical function<br>points</td>
  </tr>
  <tr>
    <td class="tg-s6z2">SRFP</td>
    <td class="tg-0lax">The proportion of term frequency of the word among all the similar words in the historical<br>function points</td>
  </tr>
  <tr>
    <td class="tg-s6z2" rowspan="4">Importance</td>
    <td class="tg-s6z2">DHV</td>
    <td class="tg-0lax">The shortest path from the word to the root verb in the content of ‘goal/desire’</td>
  </tr>
  <tr>
    <td class="tg-s6z2">DHN</td>
    <td class="tg-0lax">The shortest path from the word to the root noun in the content of ‘goal/desire’</td>
  </tr>
  <tr>
    <td class="tg-s6z2">SV</td>
    <td class="tg-0lax">The semantic similarity between the word and root verb</td>
  </tr>
  <tr>
    <td class="tg-s6z2">SN</td>
    <td class="tg-0lax">The semantic similarity between the word and root noun</td>
  </tr>
  <tr>
    <td class="tg-s6z2" rowspan="4">Representativeness</td>
    <td class="tg-s6z2">NSWS</td>
    <td class="tg-0lax">The number of similar words to the target word in the content of summary</td>
  </tr>
  <tr>
    <td class="tg-s6z2">NSWD</td>
    <td class="tg-0lax">The number of similar words to the target word in the content of description</td>
  </tr>
  <tr>
    <td class="tg-s6z2">NSWA</td>
    <td class="tg-0lax">The number of similar words to the target word in the content of acceptance criteria</td>
  </tr>
  <tr>
    <td class="tg-s6z2">TRS</td>
    <td class="tg-0lax">The TextRank score</td>
  </tr>
  <tr>
    <td class="tg-s6z2" rowspan="5">Graph</td>
    <td class="tg-s6z2">WD</td>
    <td class="tg-0lax">Degree Centrality is the number of weighted edges incident upon a vertex</td>
  </tr>
  <tr>
    <td class="tg-s6z2">BW</td>
    <td class="tg-0lax">The Betweenness Centrality of a vertex is a measurement of the number of shortest paths<br>traversing that vertex</td>
  </tr>
  <tr>
    <td class="tg-s6z2">CN</td>
    <td class="tg-0lax">The Closeness Centrality of a vertex is a measurement of its proximity to the rest of the<br>vertices in the network</td>
  </tr>
  <tr>
    <td class="tg-s6z2">EC</td>
    <td class="tg-0lax">The Eigenvector Centrality is a measure of the importance of a vertex in a network</td>
  </tr>
  <tr>
    <td class="tg-baqh">PR</td>
    <td class="tg-0lax">The scores calculated with Page Rank Algorithm</td>
  </tr>
</table>


# Examples

<table class="tg">
  <tr>
    <th class="tg-0pky">Story<br></th>
    <th class="tg-0pky">Actual FP List</th>
    <th class="tg-0pky">Recommendation FP List/Confidence</th>
  </tr>
  <tr>
    <td class="tg-0pky">作为系统管理员，我希望将新的客户信息添加到系统中，以便于管理客户信息。客户基本信息除备注外均为必填项，联系方式信息应至少包含一种有效联系方式。添加过程中会验证身份证号是否重复，如果重复会提示<br>As a system administrator, I want to add new customer's information to the system to manage customer's information. The customer's basic information is required except for the remarks. The contact information should contain at least one valid contact method. During the adding process, it will verify whether the ID number is duplicated. If it is repeated, it will prompt.</td>
    <td class="tg-0pky">添加客户信息<br>Add customer's information</td>
    <td class="tg-0pky">客户信息添加/-1.127306858698527<br>Add customer's information</td>
  </tr>
  <tr>
    <td class="tg-0pky">作为系统管理员，我希望显示客户信息列表，对选中的客户显示并维护其基本信息。以便于对选中的客户显示并维护其基本信息。<br>修改前需要验证系统管理员密码。<br>As a system administrator, I want to display a list of customer information, display and maintain basic information about selected customers, so that I can display and maintain basic information about selected customers.<br>The system administrator password needs to be verified before modification.<br></td>
    <td class="tg-0pky">维护客户基本信息<br>Maintain customer's basic information<br><br>显示客户信息<br>Display customer's information</td>
    <td class="tg-0pky">基本信息维护/-0.9490731557210287<br>Maintain basic information<br><br>系统管理员修改/-1.140566280909947<br>System administrator modification <br> <br>基本信息显示/-1.2586131890614827<br>Display basic information<br><br>信息列表显示/-1.4162368774414062<br>Display basic information list</td>
  </tr>
  <tr>
    <td class="tg-0pky">作为系统管理员，我希望输入客户姓名或联系方式，显示查询结果，以便于我查询特定的客户。<br>如果多名用户符合查询条件，则全部显示。<br>As a system administrator, I want to enter the customer's name or contact information to display the results of the query so that I can query a specific customer.<br>If multiple users meet the query criteria, they are all displayed.<br></td>
    <td class="tg-0pky">客户查询<br>Query customer</td>
    <td class="tg-0pky">客户查询/-1.1395772695541382<br>Query customer<br><br>查询结果显示/-1.5421965916951497<br>Display query result<br> <br>客户姓名输入/-1.7091108957926433<br>Enter customer's name</td>
  </tr>
</table>
