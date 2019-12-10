---
title: 获取 Microsoft Graph 工具包中的组件
description: 通过获取组件，可以在 HTML 中直接在 Microsoft Graph 中进行任何 GET 查询。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 77beb3940eb29a2c9158fba88d78084639e433ed
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39921696"
---
# <a name="get-component-in-the-microsoft-graph-toolkit"></a>获取 Microsoft Graph 工具包中的组件

您可以使用`mgt-get`从 Microsoft Graph 直接在 HTML 中进行任何 GET 查询。 组件不提供默认 UI，需要您编写模板。

## <a name="example"></a>示例

```html
<mgt-get resource="/me/messages" version="beta" scopes="mail.read" max-pages="2">
  <template>
    emails: {{value.length}}
  </template>
  <template data-type="loading">
    loading
  </template>
</mgt-get>
```

## <a name="properties-and-attributes"></a>属性和属性

您可以使用多个属性来更改组件的行为。 唯一的必需属性是`resource`。

| 属性 | 属性  | 说明 |
| --- | --- | --- |
| 资源 | resource | 要从 Microsoft Graph 中获取的资源（例如， `/me`）。 |
| scopes | scopes | 如果使用属性或以逗号分隔的范围（如果使用属性），则为可选的字符串数组。 组件将使用这些作用域（使用受支持的提供程序），以确保用户已同意正确的权限。 |
| version | version | 在发出 GET 请求时要使用的可选 API 版本。 默认值为 `v1.0`。  |
| 最大页数 | maxPages | 可选页数（针对支持分页的资源）。 默认值为3。 将此值设置为0将获取所有页面。  |
| 不适用 | 响应 | 如果请求成功，则为来自 Microsoft Graph 的只读响应。  |
| 不适用 |error| 如果请求不成功，则为 Microsoft Graph 中的只读错误。 |

## <a name="events"></a>事件
| 事件 | 详细信息 | 说明 |
| --- | --- | --- |
| dataChange | 详细信息包含`response`和`error`对象。 | 在响应或错误发生更改时激发。 |

## <a name="templates"></a>模板

`mgt-get`组件支持几个可用于定义外观的[模板](../templates.md)。 若要指定模板，请在`<template>`组件内添加一个元素，并`data-type`将值设置为下列值之一。

| 数据类型 | 数据上下文 | 说明 |
| --- | --- | --- |
| 设置 | 来自 Microsoft Graph 的响应。 | 若要呈现来自 Microsoft Graph 的数据，则需要默认模板。 |
| error | Microsoft Graph 中的错误。 | 如果发出请求时出错，将使用此模板。 |
| 装载 | 不适用 | 在发出请求时使用此模板。 |

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

有关权限的详细信息，请参阅 Microsoft Graph[权限参考](https://docs.microsoft.com/graph/permissions-reference)。 

## <a name="authentication"></a>身份验证

该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序提取所需的数据。
