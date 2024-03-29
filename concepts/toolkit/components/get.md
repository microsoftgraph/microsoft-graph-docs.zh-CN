---
title: 获取 Microsoft Graph Toolkit
description: Get 组件允许你直接在 HTML 中从 Microsoft Graph GET 查询。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 38eea0b78214c5c647fc432f3e6cf04463dcffcd
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589420"
---
# <a name="get-component-in-the-microsoft-graph-toolkit"></a>获取 Microsoft Graph Toolkit

您可以使用 直接在 `mgt-get` HTML 中执行 Microsoft Graph GET 查询。 该组件不提供默认 UI，并且要求你编写模板。

## <a name="example"></a>示例

以下示例显示了如何使用组件 `mgt-get` 显示用户的电子邮件。 可以使用代码编辑器查看属性 [和属性](#properties-and-attributes) 如何更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-get--get-email&source=docs" height="500"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-get--get-email&source=docs)

## <a name="properties-and-attributes"></a>属性和属性

可以使用多个属性更改组件的行为。 唯一必需的属性是 `resource`。

| 属性 | 属性  | 说明 |
| --- | --- | --- |
| 资源 | resource | 从 Microsoft 获取的资源Graph (例如， `/me`) 。 |
| scopes | scopes | 字符串的可选数组（如果使用 属性）或逗号分隔的范围（如果使用 属性）。 组件将使用这些作用域 (支持) ，以确保用户已同意适当的权限。 |
| version | version | 进行 GET 请求时使用的可选 API 版本。 默认值为“`v1.0`”。  |
| max-pages | maxPages | 支持分页 (的资源的可选页面) 。 默认值为 3。 将此值设置为 0 将获取所有页面。  |
| 轮询率 | pollingRate | 可选毫秒数。 设置后，组件将按定义的间隔轮询请求 URI 以进行更新。 如果使用增量查询，轮询将始终查询 delta API。 模板仅在数据更改时刷新。 |
| 启用缓存 | cacheEnabled | 可选属性，类型为 Boolean。 设置后，它指示将缓存来自资源的响应。 Overriden if `refresh()` is called or if `pollingRate` is in use. 默认值为“`false`”。 |
| cache-invalidation-period | cacheInvalidationPeriod | 可选毫秒数。 如果与 一起设置 `cacheEnabled`，则此值将修改缓存达到其无效时段前的延迟。 默认值为 `0` ，将使用默认无效时段。 |
| type | type | 预期响应的可选类型。 默认值为“`json`”。 仅在 `json` (`image` 终结点上支持或 `/photo/value$` 支持) 。 |
| 不适用 | 响应 | 如果请求成功，Microsoft Graph只读响应。  |
| 不适用 |error| 如果请求失败，Microsoft Graph只读错误。 |

## <a name="methods"></a>方法

| 方法 | 说明 |
| --- | --- |
| refresh (force？：boolean)  | 调用 方法以刷新数据。 默认情况下，UI 仅在数据发生更改时更新。 传递 `true` 以强制组件更新。  |

## <a name="events"></a>事件

事件 | 何时发出 | 自定义数据 | Cancelable | 气泡 | 使用自定义模板
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`dataChange` | 在组件加载其数据后触发。 | `{ response: any, error: any }`. 属性`response`包含从 Microsoft Graph。 如果 `error` 发生错误，则属性包含有关错误的信息 | 否 | 否 | 是

> [!TIP]
> 有关 属性中返回的数据详细信息 `response` ，请参阅你在 Get 组件的 属性中使用的 API 的 API `resource` 引用。

有关处理事件的信息，请参阅 [事件](../customize-components/events.md)。

## <a name="templates"></a>模板

组件 `mgt-get` 支持 [多个](../customize-components/templates.md) 可用于定义外观的模板。 若要指定模板，请包含 `<template>` 组件中的元素，将 `data-type` 值设置为以下值之一。

| 数据类型 | 数据上下文 | 说明 |
| --- | --- | --- |
| default | 来自 Microsoft Graph。 | 需要默认模板才能呈现来自 Microsoft Graph。 |
| 值 | 返回的数组的数据 `value` 项 | `value`当预期来自`default`图形的响应包含一组项目（如消息、文件或用户）时，请使用模板而不是 **模板**。  将自动 `value` 为资源返回的每个项目重复模板。 与 `value` 默认模板模板不同，一旦准备好项目，模板 (即可开始) 。|
| error | Microsoft 错误Graph。 | 如果提出请求出错，将使用此模板。 |
| loading | 不适用 | 请求时使用此模板。 |
| no-data | 不适用 | 当请求未返回任何数据时，将使用此模板。 |

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此组件所需的权限取决于你要从 Microsoft Graph 中检索的数据。 有关权限详细信息，请参阅 Microsoft Graph[权限参考](../../permissions-reference.md)。

## <a name="authentication"></a>身份验证

该控件使用身份验证文档中介绍的全局身份验证提供程序[](../providers/providers.md)获取所需数据。

## <a name="cache"></a>缓存

若要启用和配置缓存，请使用 和 `cacheEnabled` `cacheInvalidationPeriod` 属性。 默认情况下，该 `mgt-get` 组件不缓存任何响应。

|对象存储|缓存数据|备注|
|-----------|-----------|-------|
|`response`|从 Microsoft 查询Graph针对 属性中指定的查询`resource`的完整响应`mgt-get`|

有关详细信息[Caching](../customize-components/cache.md)请参阅 Caching。
