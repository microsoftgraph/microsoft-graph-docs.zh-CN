---
title: 获取 Microsoft Graph 工具包中的组件
description: 通过获取组件，可以在 HTML 中直接在 Microsoft Graph 中进行任何 GET 查询。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 3accdc821fb1c4b2118c278ae0e88877199f94fa
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288628"
---
# <a name="get-component-in-the-microsoft-graph-toolkit"></a>获取 Microsoft Graph 工具包中的组件

您可以使用 `mgt-get` 从 Microsoft Graph 直接在 HTML 中进行任何 GET 查询。 组件不提供默认 UI，需要您编写模板。

## <a name="example"></a>示例

下面的示例演示 `mgt-get` 如何使用组件来显示用户的电子邮件。 您可以使用代码编辑器来查看 [属性和属性](#properties-and-attributes) 如何更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-get--get-email&source=docs" height="500"></iframe>

[在 "dev" 中打开此示例](https://mgt.dev/?path=/story/components-mgt-get--get-email&source=docs)

## <a name="properties-and-attributes"></a>属性和属性

您可以使用多个属性来更改组件的行为。 唯一的必需属性是 `resource` 。

| 属性 | 属性  | 说明 |
| --- | --- | --- |
| 资源 | resource | 要从 Microsoft Graph 获取的资源 (例如， `/me`) 。 |
| scopes | scopes | 如果使用属性或以逗号分隔的范围（如果使用属性），则为可选的字符串数组。 组件将使用这些作用域 (与受支持的提供程序) ，以确保用户同意正确的权限。 |
| version | version | 在发出 GET 请求时要使用的可选 API 版本。 默认值为 `v1.0`。  |
| 最大页数 | maxPages |  (支持分页) 的资源的可选页数。 默认值为3。 将此值设置为0将获取所有页面。  |
| 轮询率 | pollingRate | 可选的 miliseconds 数量。 设置后，组件将按照定义的时间间隔轮询更新的请求 URI。 如果使用 delta 查询，轮询将始终查询 delta API。 模板仅在数据更改时才会刷新。 |
| 无 | 响应 | 如果请求成功，则为来自 Microsoft Graph 的只读响应。  |
| 无 |error| 如果请求不成功，则为 Microsoft Graph 中的只读错误。 |

## <a name="methods"></a>方法
| 方法 | 说明 |
| --- | --- |
| refresh (force？： boolean)  | 调用方法以刷新数据。 默认情况下，UI 仅在数据发生更改时才会更新。 通过传递 `true` 以强制更新组件。  |


## <a name="events"></a>活动
| 事件 | 详情 | 说明 |
| --- | --- | --- |
| dataChange | 详细信息包含 `response` 和 `error` 对象。 | 在响应或错误发生更改时激发。 |

## <a name="templates"></a>模板

`mgt-get`组件支持几个可用于定义外观的[模板](../templates.md)。 若要指定模板，请在 `<template>` 组件内添加一个元素，并将 `data-type` 值设置为下列值之一。

| 数据类型 | 数据上下文 | 说明 |
| --- | --- | --- |
| 设置 | 来自 Microsoft Graph 的响应。 | 若要呈现来自 Microsoft Graph 的数据，则需要默认模板。 |
| 值 | 返回的数组中的数据项 `value` | `value` `default` 在预期来自图表的响应以包含一组项目（如**邮件**、**文件**或**用户**）时，使用模板而不是模板。 该 `value` 模板将自动为资源返回的每个项目重复。 `value`模板还将在项目准备就绪后立即开始呈现项目， (不同) 的默认模板。|
| error | Microsoft Graph 中的错误。 | 如果发出请求时出错，将使用此模板。 |
| 装载 | 无 | 在发出请求时使用此模板。 |

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

有关权限的详细信息，请参阅 Microsoft Graph [权限参考](../../permissions-reference.md)。 

## <a name="authentication"></a>身份验证

该控件使用 [身份验证文档](./../providers.md) 中介绍的全局身份验证提供程序提取所需的数据。