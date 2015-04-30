---
layout: apipost
title: onRowUpdating
part: Objects
objectname: LocalDataProvider
directiontype: Callback
permalink: /api/LocalDataProvider/onRowUpdating/
---


#### Description

> localDataProvider에 데이터를 수정하기 직전에 호출된다.
> 결과값으로 false를 돌려주면 grid에서 편집중이던 내용이 무시되고 편집이전으로 돌아간다.
> [LocalDataProvider setValue|localDataProvider.setValue](/api/LocalDataProvider/)(row, field, value)로 수정되는 경우에는 호출되지 않는다.

#### Syntax

> function onRowUpdating(provider, row);

#### Parameters

> *provider*
> Type: [LocalDataProvider](/api/LocalDataProvider/)
> LocalDataProvider object.

> *row*
> Type: Number
> 편집중인 데이터행이다.

#### Return value

> None.

#### Example

<pre class="prettyprint">
    dataProvider.onRowUpdating = function (provider, row) {
        if ($("#chkAllow").is(":checked")) {
            // 그리드 콜백을 종료한 후 메시지를 표시되도록 해야 한다.
            RealGrids.alert('수정할 수 없습니다!');
            return false;
        }
        return true; 
    };
</pre>
