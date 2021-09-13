---
title: Microsoft 服务中的文件列表Graph Toolkit
description: 文件列表组件用于通过显示文件图标和名称来显示文件列表
ms.localizationpriority: medium
author: beth-panx
ms.openlocfilehash: 1f3aea2c4d012cd4627167523540fcfeaaaf7651
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59035344"
---
# <a name="file-list-component-in-the-microsoft-graph-toolkit"></a>Microsoft 服务中的文件列表Graph Toolkit

文件列表 [组件使用您](/graph/api/resources/onedrive) 指定的文件/文件夹名称、图标和其他属性显示多个文件夹和文件的列表。 此组件使用 [mgt 文件](./file.md) 组件。 您可以指定特定驱动器或站点，根据见解类型 (趋势、使用或共享) 显示文件列表，或者向自定义文件列表提供查询。 该组件还提供允许用户将文件上载到 One Drive 或 SharePoint 中的指定位置的选项。

## <a name="example"></a>示例

以下示例使用 组件显示 `mgt-file-list` 文件。 可以使用代码编辑器查看属性 [如何](#properties) 更改组件的行为。

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
| item-path | itemPath | 文件夹的项目路径 (相对于根文件夹) 。 默认查询为 `/me/drive/root` 。 提供 `{drive-id}` `{group-id}` 、 、 或 `{site-id}` `{user-id}` 以查询特定位置。 |
| 页面大小 | pageSize | 一个数字值，指示每个页面上要呈现的最大文件数。 **注意：** `page-size` 不支持 `insight-type` 。 |
| 文件扩展名 | fileExtensions | 用于筛选要显示的文件的文件扩展名数组。 |
| hide-more-files-button | hideMoreFilesButton | 用于指示是否显示按钮以呈现更多文件的布尔值。 |
| enable-file-upload | enableFileUpload | 启用或禁用文件上载功能的布尔值。 默认值为 `false`。  |
| excluded-file-extensions | excludedFileExtensions | 要从文件上载中排除的文件扩展名的字符串数组。 还必须将 属性 `enable-file-upload` 设置为 `true` 。 |
| max-file-size | maxFileSize | 一个数字，表示最大文件上载大小 (KB) 。 还必须将 属性 `enable-file-upload` 设置为 `true` 。 |
| max-upload-file | maxUploadFile | 一个数字，表示允许上载的最大文件数。 默认值为 `10` files。 还必须将 属性 `enable-file-upload` 设置为 `true` 。 |

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

以下示例启用文件上载功能。

```html
<mgt-file-list enable-file-upload></mgt-file-list>
```

以下示例将可上载的最大文件数限制为 5 个。

```html
<mgt-file-list max-upload-file="5" enable-file-upload></mgt-file-list>
```

以下示例将可上载的最大文件大小限制为 10000 KB。

```html
<mgt-file-list max-file-size="10000" enable-file-upload></mgt-file-list>
```

以下示例排除文件扩展名为".doc，.pdf"的文件。

```html
<mgt-file-list excluded-file-extensions=".doc,.pdf" enable-file-upload></mgt-file-list>
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

  --file-upload-border: 4px dotted #ffbdc3;
  --file-upload-background-color: rgba(255, 0, 0, 0.1);
  --file-upload-button-float: left;
  --file-upload-button-color: #323130;
  --file-upload-button-background-color: #fef8dd;
  --file-upload-dialog-content-background-color: #ffe7c7;
  --file-upload-dialog-primarybutton-background-color: #ffe7c7;
  --file-upload-dialog-primarybutton-color: #323130;
}
```

若要了解更多信息，请参阅 [设置组件样式](../customize-components/style.md)。

## <a name="microsoft-graph-apis-and-permissions"></a>Microsoft Graph API 和权限

| 配置 | 权限 | API |
| ------------- | ----------------- | --- |
| 默认 (未提供标识符或查询)  | Files.Read、Files.Read.All、Sites.Read.All | `GET /me/drive/root/children` |
| 提供 `enable-file-upload` | Files.Read、Files.Read.All、Sites.Read.All、Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All | `GET /me/drive/root/children` <br /> `PUT /me/drive/root:/{filename}:/content` <br /> `POST /me/drive/root:/{filename}:/createUploadSession` |
| 提供 `{drive-id}` AND `{item-id}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /drives/{drive-id}/items/{item-id}/children`|
| 提供 `{drive-id}` AND `{item-id}` 和 `enable-file-upload` | Files.Read、Files.Read.All、Sites.Read.All、Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All | `GET /drives/{drive-id}/items/{item-id}/children` <br /> `PUT /drives/{drive-id}/items/{item-id}:/{filename}:/content` <br /> `POST /drives/{drive-id}/items/{item-id}:/{filename}:/createUploadSession` |
| 提供 `{group-id}` AND `{item-id}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /groups/{group-id}/drive/items/{item-id}/children` |
| 提供 `{group-id}` AND `{item-id}` 和 `enable-file-upload` | Files.Read、Files.Read.All、Sites.Read.All、Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All | `GET /groups/{group-id}/drive/items/{item-id}/children` <br /> `PUT /groups/{group-id}/drive/items/{item-id}:/{filename}:/content` <br /> `POST /groups/{group-id}/drive/items/{item-id}:/{filename}:/createUploadSession` |
| 仅提供 `{item-id}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /me/drive/items/{item-id}/children` |
| 仅提供 `{item-id}` AND `enable-file-upload` | Files.Read、Files.Read.All、Sites.Read.All、Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All | `GET /me/drive/items/{item-id}/children` <br /> `PUT /me/drive/items/{item-id}:/{filename}:/content` <br /> `POST /me/drive/items/{item-id}:/{filename}:/createUploadSession` |
| 提供 `{site-id}` AND `{item-id}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /sites/{site-id}/drive/items/{item-id}/children` |
| 提供 `{site-id}` AND `{item-id}` 和 `enable-file-upload` | Files.Read、Files.Read.All、Sites.Read.All、Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All | `GET /sites/{site-id}/drive/items/{item-id}/children` <br /> `PUT /sites/{site-id}/drive/items/{item-id}:/{filename}:/content` <br /> `POST /sites/{site-id}/drive/items/{item-id}:/{filename}:/createUploadSession` |
| 提供 `{user-id}` AND `{item-id}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /users/{user-id}/drive/items/{item-id}/children` |
| 提供 `{user-id}` AND `{item-id}` 和 `enable-file-upload` | Files.Read、Files.Read.All、Sites.Read.All、Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All | `GET /users/{user-id}/drive/items/{item-id}/children` <br /> `PUT /users/{user-id}/drive/items/{item-id}:/{filename}:/content` <br /> `POST /users/{user-id}/drive/items/{item-id}:/{filename}:/createUploadSession` |
| 提供 `{drive-id}` AND `{item-path}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /drives/{drive-id}/root:/{item-path}:/children` |
| 提供 `{drive-id}` AND `{item-path}` 和 `enable-file-upload` | Files.Read、Files.Read.All、Sites.Read.All、Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All | `GET /drives/{drive-id}/root:/{item-path}:/children` <br /> `PUT /drives/{drive-id}/root:/{item-path}/{filename}:/content` <br /> `POST /drives/{drive-id}/root:/{item-path}/{filename}:/createUploadSession` |
| 提供 `{group-id}` AND `{item-path}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /groups/{group-id}/root:/{item-path}:/children` |
| 提供 `{group-id}` AND `{item-path}` 和 `enable-file-upload` | Files.Read、Files.Read.All、Sites.Read.All、Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All | `GET /groups/{group-id}/root:/{item-path}:/children` <br /> `PUT /groups/{group-id}/root:/{item-path}/{filename}:/content` <br /> `POST /groups/{group-id}/root:/{item-path}/{filename}:/createUploadSession` |
| 提供 `{site-id}` AND `{item-path}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /sites/{site-id}/root:/{item-path}:/children` |
| 提供 `{site-id}` AND `{item-path}` 和 `enable-file-upload` | Files.Read、Files.Read.All、Sites.Read.All、Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All | `GET /sites/{site-id}/root:/{item-path}:/children` <br /> `PUT /sites/{site-id}/root:/{item-path}/{filename}:/content` <br /> `POST /sites/{site-id}/root:/{item-path}/{filename}:/createUploadSession` |
| 提供 `{user-id}` AND `{item-path}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /users/{user-id}/root:/{item-path}:/children` |
| 提供 `{user-id}` AND `{item-path}` 和 `enable-file-upload` | Files.Read、Files.Read.All、Sites.Read.All、Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All | `GET /users/{user-id}/root:/{item-path}:/children` <br /> `PUT /users/{user-id}/root:/{item-path}/{filename}:/content` <br /> `POST /users/{user-id}/root:/{item-path}/{filename}:/createUploadSession` |
| 仅提供 `{item-path}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /me/drive/root:/{item-path}:/children` |
| 仅提供 `{item-path}` AND `enable-file-upload` | Files.Read、Files.Read.All、Sites.Read.All、Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All | `GET /me/drive/root:/{item-path}:/children` <br /> `PUT /me/drive/root:/{item-path}/{filename}:/content` <br /> `POST /me/drive/root:/{item-path}/{filename}:/createUploadSession` |
| `insight-type` 设置为趋势 | Sites.Read.All | `GET /me/insights/trending` |
| " `{user-id or upn}` `insight-type` 提供 AND"设置为 `trending` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/trending` |
| `insight-type` 设置为 `used` | Sites.Read.All | `GET /me/insights/used` |
| " `{user-id or upn}` `insight-type` 提供 AND"设置为 `used` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/used` |
| `insight-type` 设置为共享 | Sites.Read.All | `GET /me/insights/shared` |
| " `{user-id or upn}` `insight-type` 提供 AND"设置为 `shared` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/shared?$filter=((lastshared/sharedby/id eq '${user-id}') and (resourceReference/type eq 'microsoft.graph.driveItem'))` |

## <a name="events"></a>活动

Event | 何时发出 | 自定义数据 | Cancelable | 气泡 | 使用自定义模板
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
> 组件 `mgt-file-list` 在提供时 `fileQueries` 还使用 IndexedDB 中的对象存储 `mgt-file` 来 `fileQueries` 缓存文件。

若要详细了解如何配置缓存[，请参阅](../customize-components/cache.md)Caching。
