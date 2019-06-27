---
title: Microsoft Graph 工具包中的模板
description: 使用自定义模板修改组件的内容。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: f0648d0ac1348fbadad6cebe8a022f9445fcf1e3
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242957"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具包中的模板

使用自定义模板修改组件的内容。

所有 web 组件都支持基于元素的`<template>`模板。 例如, 若要覆盖组件的模板, 请在组件中`<template>`添加元素。

```html
<mgt-agenda>
  <template data-type="event">
      <div>{{event.subject}}</div>
      <div data-for='attendee in event.attendees'>
          <mgt-person person-query="{{attendee.emailAddress.name}}">
            <template>
              <div data-if="person.image">
                <img src="{{person.image}}" />
              </div>
              <div data-else>
                {{person.displayName}}
              </div>
            </template>
          </mgt-person>
      </div>
  </template>
</mgt-agenda>
```

以下模板功能受支持:

- 使用双花括号 (`{{expression}}`) 展开表达式。 在上面的示例中, `<mgt-person>`传递一个`person`可在模板中使用的对象。
- 使用`data-if`和`data-else`属性进行条件呈现。 支持`event.attendees.length > 2`的条件表达式 (如支持)。
- `data-for`使用重复元素。
- `data-type`使用指定要模板的组件部分。 如果不指定类型, 则会将该模板应用于整个组件。

每个组件都记录`data-type`受支持的值和向下传递给每个模板的数据上下文。

模板的样式可以像在阴影 dom 外部呈现的那样正常显示。
