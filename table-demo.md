

          #  liquid table starts here





    ###
    ###  LIQUID TABLE ADDED USING YAML DATA
    ###
    ###  liquid is a simple markup language that allows
    ###  web designers to separate page layouts from
    ###  page content without databases
    ###
    ###  &lbrace;%  function in liquid  %}
    ###  &lbrace;&lbrace;  variable in liquid  }}
    ###

        ###
        ###  YAML HEADER FOR PAGE
        ###

        ---
        layout: liquid-table
        title: 'amiright?'
        reynolds:
          strengths:
          - good father
          - funny
          - dated alanis morissette
          weaknesses: 
          - singing
          - green lantern movie
          - tennis backhand 
        gosling:
          strengths: 
          - builds houses
          - is a real boy
          - never dated alanis morissette
          weaknesses: 
          - micky mouse club
          - cries a lot
          - not ryan reynolds
        ---
![](assets/img/ryan-v-ryan.jpg) 

       ### Lorem Ipsum
       
       Lorem ipsum dolor sit amet....
       
       
       ###
       ###  LIQUID TAG TABLE IN LAYOUT
       ###
       ###  HTML ELEMENTS: 
       ###  &lt;thead> table header
       ###  &lt;tr>  table row 
       ###  &lt;td>  table cell (or data)
       ###  &lt;ul> unordered list
       ###  &lt;li> list item 
       ###

        &lt;h2> Ryan vs Ryan &lt;/h2>

        &lt;table id="ryan-v-ryan">

        &lt;thead>
          &lt;tr>
            &lt;th>  &lt;h3>  Ryan Reynolds  &lt;/h3>  &lt;/th>
            &lt;th>  &lt;h3>  Ryan Gosling  &lt;/h3>  &lt;/th>
          &lt;/tr>
        &lt;/thead>

        &lt;tbody>
        &lt;tr>
          &lt;td>
            &lt;h4>  Strengths  &lt;/h4>
            &lt;ul>

              ###  LIQUID LOOPS WITH YAML DATA
              ###  reynolds:
              ###    strengths:
              ###    - good father
              ###    - funny
              ###    - dated alanis morissette

              &lbrace;% for item in page.reynolds.strengths %}
                 &lt;li>  &lbrace;&lbrace; item }}  &lt;/li>
              &lbrace;% endfor %}

              ###    LIQUID LOOP CREATES HTML CODES:
              ###    &lt;li> good father &lt;/li>
              ###    &lt;li> funny &lt;/li>
              ###    &lt;li> dated alanis morissette &lt;/li>        

            &lt;/ul>
            &lt;br>
            &lt;h4>  Weaknessess  &lt;/h4>
            &lt;ul>

              &lbrace;% for item in page.reynolds.weaknesses %}
                 &lt;li>  &lbrace;&lbrace; item }}  &lt;/li>
              &lbrace;% endfor %}

            &lt;/ul>  
          &lt;/td>
          &lt;td>
            &lt;h4>  Strengths  &lt;/h4>
            &lt;ul>

              &lbrace;% for item in page.gosling.strengths %}
                &lt;li>  &lbrace;&lbrace; item }}  &lt;/li>
              &lbrace;% endfor %}

            &lt;/ul>
            &lt;br>
            &lt;h4>  Weaknessess  &lt;/h4>
            &lt;ul>

              &lbrace;% for item in page.gosling.weaknesses %}
                 &lt;li>  &lbrace;&lbrace; item }}  &lt;/li>
              &lbrace;% endfor %}

            &lt;/ul>
          &lt;/td>
        &lt;/tr> 
        &lt;/table>

</code>
</pre>
</blockquote>





<style>
  pre{
  font-family: Consolas, Menlo, Monaco, Lucida Console, Liberation Mono, DejaVu Sans Mono, Bitstream Vera Sans Mono, Courier New, monospace, serif;
  margin-bottom: 10px;
  padding: 5px;
  background-color: #eee;
  width: 750px!ie7;
  padding-bottom: 20px!ie7;
}

ui {
  padding-inline-start: 10px;
  }
  
table {
  margin-left: 20px;
  }
  
</style>
