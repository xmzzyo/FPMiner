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
    <th class="tg-0pky">Summary<br></th>
    <th class="tg-0pky">Description</th>
    <th class="tg-0pky">Acceptance</th>
    <th class="tg-0pky">Recommendation FP List</th>
  </tr>
  <tr>
    <td class="tg-0pky">作为客户经理，我希望根据我选择的考核时间，查询近24个月的****</td>
    <td class="tg-0pky">**时间筛选条件*****</td>
    <td class="tg-0pky">1、根据数据获取时间筛选范围。2、确初始化时间选择控件。</td>
    <td class="tg-0pky">考核时间选择</td>
  </tr>
  <tr>
    <td class="tg-0pky">作为***管理员，我想要新增某**的******,使得**的******的准确性。</td>
    <td class="tg-0pky">1、能成功保存修改的******信息2、**查询功能，能够查询到修改后的******信息3、并能将******回传到***系统</td>
    <td class="tg-0pky">业务要求：该功能隐藏AC1、能成功保存修改的******2、**查询功能，能够查询到修改后的********3、并能将******回传到***系统</td>
    <td class="tg-0pky">******新增</td>
  </tr>
  <tr>
    <td class="tg-0pky">作为**人员，我希望在设置****时能够直接进行**操作，以便减少我的操作步骤</td>
    <td class="tg-0pky">在****管理  **管理  ****  **结果调整界面，在“添加”和“提交”之间，新加“提交并重对”按钮，点击后提交对应关系，并自动对该**的该调整记录对应的****进行重对处理</td>
    <td class="tg-0pky">按钮增加正常点击后，**关系可以建立，并能够正对该调整信息对应的**记录进行重新**</td>
    <td class="tg-0pky">**结果提交并重对</td>
  </tr>
  <tr>
    <td class="tg-0lax">作为客户经理，我想希望在客户画像页展示客户的******，以便为客户购买**</td>
    <td class="tg-0lax">1、***客户****承受能力评估信息***评估类型代码**:****、**:****2、需要开发CSV接口</td>
    <td class="tg-0lax">在客户画像显示******</td>
    <td class="tg-0lax">客户******、******显示</td>
  </tr>
  <tr>
    <td class="tg-0lax">作为使用者，我想要看到******的视频和相关文档</td>
    <td class="tg-0lax">*****页面添加视频和相关文档</td>
    <td class="tg-0lax">在*****页面，********区域添加第2期的3个视频和相关文档，视频播放和文档下载均正常</td>
    <td class="tg-0lax">***视频播放, ***视频下载</td>
  </tr>
</table>
