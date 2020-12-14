---
title: 获取 Microsoft Graph Toolkit
description: Get 组件允许你直接在 HTML 中从 Microsoft Graph 进行任何 GET 查询。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 7ce33d231b02603c953a57df8ae8751f8544ee7a
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659378"
---
# <a name="get-component-in-the-microsoft-graph-toolkit"></a>获取 Microsoft Graph Toolkit

可以使用 HTML 直接从 Microsoft Graph 进行任何 `mgt-get` GET 查询。 该组件不提供默认 UI，并且要求您编写模板。

## <a name="example"></a>示例

以下示例显示组件 `mgt-get` 用于显示用户的电子邮件。 可以使用代码编辑器查看 [属性和属性](#properties-and-attributes) 如何更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-get--get-email&source=docs" height="500"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-get--get-email&source=docs)

## <a name="properties-and-attributes"></a>属性和属性

可以使用多个属性更改组件的行为。 唯一必需的属性是 `resource` 。

| 属性 | 属性  | 说明 |
| --- | --- | --- |
| 资源 | resource | 从 Microsoft Graph 获取的资源 (例如 `/me` ，) 。 |
| scopes | scopes | 可选字符串数组（如果使用属性）或逗号分隔范围（如果使用该属性）。 组件将使用这些作用域 (支持) ，以确保用户已同意适当的权限。 |
| version | version | 进行 GET 请求时使用的可选 API 版本。 默认值为“`v1.0`”。  |
| max-pages | maxPages | 支持分页 (资源的可选页面) 。 默认值为 3。 将此值设置为 0 将获取所有页面。  |
| 轮询率 | pollingRate | 可选数量的 miliseconds。 设置后，组件将轮询请求 URI，以按定义的间隔进行更新。 如果使用 delta 查询，轮询将始终查询增量 API。 模板仅在数据更改时刷新。 |
| 启用缓存 | cacheEnabled | 可选属性，类型为 Boolean。 设置后，它表示将缓存来自资源的响应。 如果已 `refresh()` 调用或正在使用， `pollingRate` 则替代。 默认值为“`false`”。 |
| cache-invalidation-period | cacheInvalidationPeriod | 可选数量 miliseconds。 如果结合使用设置，则此值将修改缓存达到其无效时段 `cacheEnabled` 前的延迟。 默认值为 `0` ，并且将使用默认无效时段。 |
| type | type | 预期响应的可选类型。 默认值为“`json`”。 仅在 `json` (终结点上 `image` 支持或支持 `/photo/value$`) 。 |
| 不适用 | 响应 | 如果请求成功，来自 Microsoft Graph 的只读响应。  |
| 不适用 |error| 如果请求未成功，来自 Microsoft Graph 的只读错误。 |

## <a name="methods"></a>方法
| 方法 | 说明 |
| --- | --- |
| refresh (force？：boolean)  | 调用该方法以刷新数据。 默认情况下，UI 仅在数据发生更改时更新。 传递 `true` 以强制更新组件。  |


## <a name="events"></a>活动
| 事件 | 详情 | 说明 |
| --- | --- | --- |
| dataChange | 详细信息包含 `response` and `error` 对象。 | 响应或错误更改时触发。 |

## <a name="templates"></a>模板

该 `mgt-get` 组件支持 [多个](../customize-components/templates.md) 可用于定义外观的模板。 若要指定模板，请包含 `<template>` 组件中的元素，将值设置为下列 `data-type` 值之一。

| 数据类型 | 数据上下文 | 说明 |
| --- | --- | --- |
| default | 来自 Microsoft Graph 的响应。 | 呈现来自 Microsoft Graph 的数据需要默认模板。 |
| 值 | 返回数组的数据 `value` 项 | 当预期来自图形的响应包含项目数组（如消息、文件或用户）时，请使用模板而不是 `value` `default` **模板**。   `value`将自动为资源返回的每个项目重复模板。 与默认模板模板不同，模板一旦准备好 (`value` 即可开始呈现) 。|
| error | Microsoft Graph 中的错误。 | 如果提出请求时出错，将使用此模板。 |
| loading | 不适用 | 请求时使用此模板。 |

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

有关权限详细信息，请参阅 Microsoft Graph [权限参考](../../permissions-reference.md)。 

## <a name="authentication"></a>身份验证

该控件使用身份验证文档中介绍的全局身份验证提供程序[](../providers/providers.md)获取所需数据。
