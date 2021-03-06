---
layout: apipost
title: getValues
part: Objects
objectname: GridView
directiontype: Function
permalink: /api/GridView/getValues/
tags: 
  - JSON
  - 가져오기
  - 행의 값
---


#### Description

 지정한 itemIndex의 값들을 JSON객체로 가져온다. itemIndex와 연결된 dataRow는 return되는 객체의 __rowId에 담겨있다.   
 입력된 itemIndex가 dataRow와 연결된 행이 아닌경우 null이 출력된다.  

#### Syntax

> function getValues(itemIndex)  

#### Parameters

> **itemIndex**  
> Type: integer  
> itemIndex를 입력한다.  

#### Return value

> Type: Object  
> JSON객체로 만들어진 item행의 값  

#### Examples 

<pre class="prettyprint">
var values = gridView.getValues(0);
</pre>

---

#### Demo Links

* [GetValues](http://demo.realgrid.com/DataManager/GetValues){:target="_blank"} 