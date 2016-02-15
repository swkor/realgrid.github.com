---
layout: apipost
title: showToast
part: Objects
objectname: GridBase
directiontype: Function
permalink: /api/GridBase/showToast/
---


#### Description

> Toast 팝업 창을 표시한다.  

#### Syntax

> function showToast(options, force)  

#### Parameters

> **options**  
> Type: [ToastOptions](/api/types/ToastOptions/)  
> 메시지와 메시지 표시여부를 지정, 기본적으로 메시지만 지정해도 된다.  

> **force**  
> Type: Boolean  
> Default: undefined  
> 기존 toast창이 표시되어 있을때 강제로 다시 표시 여부를 지정한다.   

#### Return value

> None.  

#### Example

<pre class="prettyprint">
    gridView.showToast("toast 창을 표시합니다.");
</pre>
