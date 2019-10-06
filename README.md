# React-Native-Questions
Contains list of all important questions and answers related to RN
<details>
<summary> Why do we use curly brace while importing some library? Eg: <code> import { Text, StyleSheet } from "react-native"; </code> </summary>
  </br>
Curcly braces are used to import small pieces of library. In above example we just want to make use of Text and StyleSheet component from react-native, so they are put in curly braces.
</details>

<details>
  <summary>Why didn't we use curly braces here ? <code>import React from "react";</code> </summary>
  </br>
    Because we wanted to import entire library and not part of react. 
</details>

<details>
  </details>

<details>
  <summary>What is benefit of using StyleSheet object as opposed to inline styles ? </summary>
  </br>
    StyleSheet will validate all styles rules and give error straight away, whereas inline style will show warning in case of error.
    
  For e.g.  This will just show warning 
  </br>
  <blockquote><pre><code> <Text style={{ fontsize: 40 }}>Example of inline style</Text> </code> </pre> </blockquote> 
  This will throw error right away
            <blockquote><pre><code> 
 const styles = StyleSheet.create({
     textStyle: {
       fontsize: 30
     }
 })</code> </pre> </blockquote> 
</details>
<details>
<summary>
            Will this piece of code work?
            <pre><code>
&lt;View&gt;
  &lt;Text>Hey there!&lt;/Text&gt;
  &lt;Text style={{ fontsize: 40 }} &gt;Example of inline style&lt;/Text&gt;;
&lt;/View&gt;
                </code> </pre></summary>
No. Text error will be thrown as Text strings must be rendered within Text component.
  Because here semi-colon in third line will be treated as text, and in React native all texts needs to be rendered inside Text tag.
    </details>
