---
title: Microsoft Graph 工具包中的 "人员" 组件
description: 您可以使用`mgt-people` web 组件显示一组用户或联系人, 方法是使用其照片或缩写。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: fcc44262f807d3f10f42e8af8e476975ad262cda
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242978"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具包中的 "人员" 组件

您可以使用`mgt-people` web 组件显示一组用户或联系人, 方法是使用其照片或缩写。 默认情况下, 它将显示登录用户最常使用的联系人。

此组件使用多个 "控制[人员](./person.md)" 控件, 但它可以绑定到一组人员描述符。 如果要显示的人员多于`show-max`该值, 则将添加一个数字以指示其他联系人的数量。

## <a name="example"></a>示例

[jsfiddle 示例](https://jsfiddle.net/metulev/az6pqy2r/)

```html
<mgt-people></mgt-people>
```

![组织-人员](./images/mgt-people.png)

## <a name="properties"></a>属性

默认情况下, `mgt-people`组件使用`personType/class eq 'Person'`筛选器从`/me/people`终结点提取事件, 以显示经常联系的用户。 您可以使用多个属性来更改此行为。

| 属性 | 属性 | 说明 |
| --- | --- | --- |
| `showMax` | `show-max` | 指示要显示的最大用户数。 默认值为3。 |
| `people` | `people` | 获取或设置组件呈现的人员列表的人员数组。 使用此属性可访问组件加载的人员。 设置此值可加载自己的人员。 |

下面的示例设置要显示的最大用户数。

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a>CSS 自定义属性

`mgt-people`组件定义以下 CSS 自定义属性。

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
}
```

## <a name="templates"></a>模板

支持多个[模板](../templates.md), 这些模板可用于替换组件的某些部分。 `mgt-people` 若要指定模板, 请在`<template>`组件内添加一个元素, 并`data-type`将值设置为下列值之一。

| 数据类型 | 数据上下文 | 说明 |
| --- | --- | --- |
| `default` | `people`: person 对象列表 | 默认模板会将整个组件替换为您自己的组件。 |
| `person` | `person`: person 对象 | 用于呈现每个人的模板。 |
| `overflow` | `people`: person 对象列表 <br> `max`: 显示的人员的数量 <br> `extra`: 额外人员数 | 用于将数字呈现在人员列表右侧的最大值之后的模板。 |
| `no-data` | 不传递数据上下文 | 没有人可用时使用的模板。 |

下面的示例演示如何使用`person`模板。

```html
<mgt-people>
  <template>
    <ul><li data-for="person in people">
      <mgt-person person-query="{{ person.userPrincipalName }}"></mgt-person>
      <h3>{{ person.displayName }}</h3>
      <p>{{ person.jobTitle }}</p>
      <p>{{ person.department }}</p>
    </li></ul>
  </template>
</mgt-people>
```

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此组件使用以下 Microsoft Graph Api 和权限:

| 资源 | 权限/范围 |
| - | - |
| [/me/people](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | `People.Read` |

## <a name="authentication"></a>身份验证

该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。
