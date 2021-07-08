---
title: Microsoft 服务中的文件列表Graph Toolkit
description: 文件列表组件用于通过显示文件图标和名称来显示文件列表
localization_priority: Normal
author: beth-panx
ms.openlocfilehash: 816ea4b76a08d089e419aad2a126b7b39c2727b1
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334778"
---
# <a name="file-list-component-in-the-microsoft-graph-toolkit"></a>Microsoft 服务中的文件列表Graph Toolkit

文件列表 [组件使用您](/graph/api/resources/onedrive) 指定的文件/文件夹名称、图标和其他属性显示多个文件夹和文件的列表。 此组件使用 [mgt 文件](./file.md) 组件。 您可以指定特定驱动器或网站、根据见解类型显示文件列表 (趋势、使用或共享) ，或者提供对自定义文件列表的查询。

## <a name="example"></a>示例

以下示例使用 组件显示 `mgt-file-list` 文件。 可以使用代码编辑器查看 [属性如何](#properties) 更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-file-list--file-list&source=docs" height="250"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-file-list--file-list&source=docs)

## <a name="properties"></a>属性

可以使用多个属性来自定义组件。

| 属性 | 属性 | 说明 |
| --------- | -------- | ----------- |
| file-list-query | fileListQuery | 包含要呈现的文件列表的驱动器或站点的完整查询或路径。 |
| 文件查询 | fileQueries | 由组件呈现的文件查询数组。 |
| 无 | files | 用于获取或设置组件呈现的文件列表的文件数组。 使用它来访问组件加载的文件。 设置此值以加载您自己的文件。 |
| insight-type | insightType | 设置为显示用户的趋势、使用的文件或共享文件。 |
| drive-id | driveId | 文件夹所属驱动器的 ID。 还必须提供 或 `item-id` `item-path` 。 |
| group-id | groupId | 文件夹所属组的 ID。 还必须提供 或 `item-id` `item-path` 。 |
| site-id | siteId | 文件夹所属网站的 ID。 还必须提供 或 `{item-id}` `{item-path}` 。 `{list-id}`如果从特定列表引用文件，则提供 。 |
| item-id | itemId | 文件夹的 ID。 默认查询为 `/me/drive/items` 。 提供 `{drive-id}` `{group-id}` 、 、 或 `{site-id}` `{user-id}` 以查询特定位置。 |
| item-path | itemPath | 文件夹的项目路径 (根文件夹) 。 默认查询为 `/me/drive/root` 。 提供 `{drive-id}` `{group-id}` 、 、 或 `{site-id}` `{user-id}` 以查询特定位置。 |
| 页面大小 | pageSize | 一个数字值，指示每个页面上要呈现的最大文件数。 |
| 文件扩展名 | fileExtensions | 用于筛选要显示的文件的文件扩展名数组。 |
| hide-more-files-button | hideMoreFilesButton | 用于指示是否显示按钮以呈现更多文件的布尔值。 |

下面的示例更改组件的行为，以从特定查询获取文件列表。

```html
<mgt-file-list file-list-query="/me/drive/items/01BYE5RZYJ43UXGBP23BBIFPISHHMCDTOY/children"></mgt-file-list>
```

以下示例通过提供文件夹 ID，更改组件的行为，以从文件夹获取文件列表。

```html
<mgt-file-list item-id="01BYE5RZYJ43UXGBP23BBIFPISHHMCDTOY"></mgt-file-list>
```

以下示例通过提供组 ID 和文件夹路径，更改组件的行为以从组提取文件列表。

```html
<mgt-file-list group-id="8090c93e-ba7c-433e-9f39-08c7ba07c0b3" item-path="/Design"></mgt-file-list>
```

以下示例通过提供用户 ID 和文件夹 ID，更改组件的行为以从用户获取文件列表。

```html
<mgt-file-list user-id="48d31887-5fad-4d73-a9f5-3c356e68a038" item-id="01BYE5RZYFPM65IDVARFELFLNTXR4ZKABD"></mgt-file-list>
```

以下示例通过提供见解类型，更改组件的行为以提取文件列表。

```html
<mgt-file-list insight-type="shared"></mgt-file-list>
```

## <a name="methods"></a>方法
| 方法 | 说明 |
| --- | --- |
| reload (clearCache = false)  | 调用 方法，根据组件的属性使用潜在的新数据重新加载组件。 传递 `true` 以在重新加载之前清除缓存。 |

## <a name="css-custom-properties"></a>CSS 自定义属性

组件 `mgt-file-list` 定义以下 CSS 自定义属性。

```css
mgt-file-list {
  --font-family: 'Segoe UI';
  --font-size: 14px;

  --file-list-background-color: #ffffff;
  --file-list-border: none;
  --file-list-box-shadow: none;
  --file-list-padding: 4px 0;
  --file-list-margin: 0;

  --file-item-background-color--hover: rgba(0, 0, 0, 0.1);
  --file-item-background-color--active: rgba(0, 0, 0, 0.05);
  --file-item-border-radius: 2px;
  --file-item-margin: 0 4px;

  --file-item-border-top: none;
  --file-item-border-left: none;
  --file-item-border-right: none;
  --file-item-border-bottom: none;

  --show-more-button-background-color: #f3f2f1;
  --show-more-button-background-color--hover: rgba(0, 0, 0, 0.1);
  --show-more-button-font-size: 12px;
  --show-more-button-padding: 6px;
  --show-more-button-border-bottom-right-radius: 4px;
  --show-more-button-border-bottom-left-radius: 4px;
}
```

若要了解更多信息，请参阅 [设置组件样式](../customize-components/style.md)。

## <a name="microsoft-graph-apis-and-permissions"></a>Microsoft Graph API 和权限

| 配置 | 权限 | API |
| ------------- | ----------------- | --- |
| 默认 (未提供标识符或)  | Files.Read、Files.Read.All、Sites.Read.All | `GET /me/drive/root/children` |
| 提供 `{drive-id}` AND `{item-id}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /drives/{drive-id}/items/{item-id}/children` |
| 提供 `{group-id}` AND `{item-id}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /groups/{group-id}/drive/items/{item-id}/children` |
| 仅提供 `{item-id}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /me/drive/items/{item-id}/children` |
| 提供 `{site-id}` AND `{item-id}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /sites/{site-id}/drive/items/{item-id}/children` |
| Pprovide `{user-id}` AND `{item-id}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /users/{user-id}/drive/items/{item-id}/children` |
| 提供 `{drive-id}` AND `{item-path}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /drives/{drive-id}/root:/{item-path}:/children` |
| 提供 `{group-id}` AND `{item-path}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /groups/{group-id}/root:/{item-path}:/children` |
| 提供 `{site-id}` AND `{item-path}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /sites/{site-id}/root:/{item-path}:/children` |
| 提供 `{user-id}` AND `{item-path}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /users/{user-id}/root:/{item-path}:/children` |
| 仅提供 `{item-path}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /me/drive/root:/{item-path}:/children` |
| `insight-type` 设置为趋势 | Sites.Read.All | `GET /me/insights/trending` |
| " `{user-id or upn}` `insight-type` 提供 AND"设置为 `trending` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/trending` |
| `insight-type` 设置为 `used` | Sites.Read.All | `GET /me/insights/used` |
| " `{user-id or upn}` `insight-type` 提供 AND"设置为 `used` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/used` |
| `insight-type` 设置为共享 | Sites.Read.All | `GET /me/insights/shared` |
| " `{user-id or upn}` `insight-type` 提供 AND"设置为 `shared` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/shared?$filter=((lastshared/sharedby/id eq '${user-id}') and (resourceReference/type eq 'microsoft.graph.driveItem'))` |

## <a name="events"></a>活动

事件 | 何时发出 | 自定义数据 | Cancelable | 气泡 | 使用自定义模板
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`itemClick` | 在用户单击文件时触发。 | 所选 [文件](/graph/api/resources/driveItem) | 否 | 否 | 是，使用自定义 **文件** 模板

有关处理事件的信息，请参阅 [事件](../customize-components/events.md)。

## <a name="templates"></a>模板

组件 `mgt-file-list` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。 若要指定模板，请包含组件内的元素，将值设置为下表 `<template>` `data-type` 中列出的数据类型之一。

| 数据类型 | 数据上下文 | 说明 |
| ----------- | -------------- | ------------ |
| default | `files`：文件对象列表 | 默认模板将整个组件替换为你自己的组件。 |
| file | `file`：file 对象 | 用于呈现每个文件的模板。 |
| no-data | 不传递任何数据上下文 | 没有可用数据时所使用的模板。 |
| loading | 不传递任何数据上下文 | 组件加载状态时所使用的模板。 |

## <a name="authentication"></a>身份验证

该控件使用身份验证文档中介绍的全局身份验证提供程序[](../providers/providers.md)获取所需数据。

## <a name="cache"></a>缓存

|对象存储|缓存数据|备注|
|---------|-----------|-------|
|`fileLists`|文件列表列表|用于存储文件列表的默认缓存列表。|
|`insightfileLists`|见解文件列表列表|提供时 `insightType` 使用。|

> [!NOTE]
> 组件 `mgt-file-list` 在提供时 `fileQueries` 还使用 `mgt-file` IndexedDB 中的对象存储来 `fileQueries` 缓存文件。

若要详细了解如何配置缓存[，请参阅](../customize-components/cache.md)Caching。