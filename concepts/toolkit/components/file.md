---
title: Microsoft 服务中的文件Graph Toolkit
description: 文件组件用于通过显示图标和名称来显示文件
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 1519b314be1d41d1a2df87cebbfb99d2e593c6a4
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589063"
---
# <a name="file-component-in-the-microsoft-graph-toolkit"></a>Microsoft 服务中的文件Graph Toolkit

文件组件用于表示 [OneDrive 或 SharePoint](/graph/onedrive-concept-overview) 中的单个文件/文件夹，具体方法为显示文件/文件夹名称、指示文件类型的图标以及其他属性（如作者、上次修改日期或其他详细信息）。 你可以提供文件的标识符，组件将生成查询以根据提供的标识符检索文件。 此组件可以自己使用，也可以作为 [mgt-file-list组件的一部分](./file-list.md) 使用。

## <a name="example"></a>示例

以下示例使用 组件显示文件 `mgt-file` 。 可以使用代码编辑器查看属性 [如何](#properties) 更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-file--file&source=docs" height="250"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-file--file&source=docs)

## <a name="properties"></a>属性

可以使用多个属性来自定义组件。

| 属性 | 属性 | 说明 |
| --------- | -------- | ----------- |
| 文件查询 | fileQuery | 要检索的文件的完整查询或路径。 |
| drive-id | driveId | 文件所属驱动器的 ID。 还必须提供 或 `item-id` `item-path`。 |
| group-id | groupId | 文件所属组的 ID。 还必须提供 或 `item-id` `item-path`。 |
| site-id | siteId | 文件所属网站的 ID。 还必须提供 或 `{item-id}` `{item-path}`。 `{list-id}`如果从特定列表引用文件，则也提供 。 |
| list-id | listId | 文件所属列表的 ID。 还必须提供 `{site-id}` 和 `{item-id}`。 |
| item-id | itemId | 文件的 ID。 默认查询为 `/me/drive/items`。 提供 `{drive-id}`、 `{group-id}``{site-id}`、 或 `{user-id}` 以查询特定位置。 |
| item-path | itemPath | 文件的项目路径。 默认查询为 `/me/drive/root`。 提供 `{drive-id}`、 `{group-id}``{site-id}`、 或 `{user-id}` 以查询特定位置。 |
| insight-type | insightType | 从中检索文件的见解类型。 可以是 、`trending``used`、 或 `shared`。 |
| insight-id | insightId | 见解资源的 ID。 |
| file-details | fileDetails | 设置为表示文件的对象 |
| file-icon | fileIcon | 设置为要显示文件的图标 |
| view | view | 设置为控制文件的呈现方式。 默认值为 `oneline`。 <br>`image` - 只显示图标 <br>`oneline`- 显示图标和一行文本 (默认为文件) `name` <br>`twolines`- 显示图标和两行`name``lastModifiedDateTime`文本 (默认情况下显示) <br> `threelines`- 默认显示作者的图标 (`name`、`lastModifiedDateTime``displayName`、和三行文本)  |
| line1-property | line1Property | 设置 要用于 `fileDetails` 第一行文本的属性。 `name`默认值为 文件。 |
| line2-property | line2Property | 设置 要用于 `fileDetails` 第二行文本的属性。 默认值为“`lastModifiedDateTime`”。 |
| line3-property | line3Property | 设置 要用于 `fileDetails` 第三行文本的属性。 `size`默认值为 文件。 |

以下示例将组件的行为更改为从特定查询提取数据。

```html
<mgt-file file-query="/me/drive/items/01BYE5RZZFWGWWVNHHKVHYXE3OUJHGWCT2"></mgt-file>
```

以下示例更改组件的行为以从特定查询提取数据，显示三行信息（默认情况下为文件名、上次修改日期时间和文件大小）并设置文件图标。

```html
<mgt-file file-query="/me/drive/items/01BYE5RZZFWGWWVNHHKVHYXE3OUJHGWCT2" view="threeLines" file-icon="ICON_PATH"></mgt-file>
```

以下示例将组件的行为更改为从特定驱动器提取数据。

```html
<mgt-file drive-id="b!-RIj2DuyvEyV1T4NlOaMHk8XkS_I8MdFlUCq1BlcjgmhRfAj3-Z8RY2VpuvV_tpd" item-id="01BYE5RZ5MYLM2SMX75ZBIPQZIHT6OAYPB"></mgt-file>
```

以下示例将组件的内容更改为从网站和路径SharePoint数据。

```html
  <mgt-file site-id="m365x214355.sharepoint.com,5a58bb09-1fba-41c1-8125-69da264370a0,9f2ec1da-0be4-4a74-9254-973f0add78fd" item-Path="/DemoDocs/AdminDemo"></mgt-file>
```

以下示例将组件的行为更改为按见解类型提取数据。

```html
<mgt-file insight-type="shared" insight-id="AW1GxMvkOztMkJX-SCppUSRPF5EvyPDHRZVAqtQZXI4JoUXwI9_mfEWNlabr1f7aXRBWDMt2C2FDop4fP1vsUw9tRsTL5Ds7TJCV_kgqaVEkBA"></mgt-file>
```

## <a name="css-custom-properties"></a>CSS 自定义属性

组件 `mgt-file` 定义以下 CSS 自定义属性。

```css
mgt-file {
  --file-type-icon-size: 28px;
  --file-border: none;
  --file-box-shadow: none;
  --file-background-color: #ffffff;

  --font-family: 'Segoe UI';
  --font-size: 14px;
  --font-weight: 400;
  --text-transform: none;
  --color: #323130;

  --line2-font-size: 12px;
  --line2-font-weight: 400;
  --line2-color: #797775;
  --line2-text-transform: none;

  --line3-font-size: 12px;
  --line3-font-weight: 400;
  --line3-color: #797775;
  --line3-text-transform: none;
}
```

若要了解更多信息，请参阅 [设置组件样式](../customize-components/style.md)。

## <a name="microsoft-graph-apis-and-permissions"></a>Microsoft Graph API 和权限

此控件使用下列 Microsoft Graph API 和权限。

| 配置 | 权限范围 | API |
| ------------- | ----------------- | --- |
| 开发人员提供 `{drive-id}` AND `{item-id}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /drives/{drive-id}/items/{item-id}` |
| 开发人员提供 `{drive-id}` AND `{item-path}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /drives/{drive-id}/root:/{item-path}` |
| 开发人员提供 `{group-id}` AND `{item-id}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /groups/{group-id}/drive/items/{item-id}` |
| 开发人员提供 `{group-id}` AND `{item-path}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /groups/{group-id}/drive/root:/{item-path}` |
| 开发人员提供 ONLY `{item-id}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /me/drive/items/{item-id}` |
| 开发人员提供 ONLY `{item-path}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /me/drive/root:/{item-path}` |
| 开发人员提供 `{site-id}` AND `{item-id}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /sites/{site-id}/drive/items/{item-id}` |
| 开发人员提供 `{site-id}` AND `{item-path}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /sites/{site-id}/drive/root:/{item-path}` |
| 开发人员提供 `{site-id}` AND `{list-id}` AND `{item-id}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /sites/{site-id}/lists/{list-id}/items/{item-id}/driveItem` |
| 开发人员提供 `{user-id}` AND `{item-id}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /users/{user-id}/drive/items/{item-id}` |
| 开发人员提供 `{user-id}` AND `{item-path}` | Files.Read、Files.Read.All、Sites.Read.All | `GET /users/{user-id}/drive/root:/{item-path}` |
| `insight-type` 设置为 AND `trending` 开发人员提供 `{insight-id}` | Sites.Read.All | `GET /me/insights/trending/{insight-id}/resource` |
| 开发人员提供 `{user-id or upn}` AND `{insight-id}` AND `insight-type` 设置为 `trending` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/trending/{insight-id}/resource` |
| `insight-type` 设置为 AND `used` 开发人员提供 `{insight-id}` | Sites.Read.All | `GET /me/insights/used/{id}/resource` |
| 开发人员提供 `{user-id or upn}` AND `{insight-id}` AND `insight-type` 设置为 `used` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/used/{id}/resource` |
| `insight-type` is `shared` AND 开发人员提供 `{insight-id}` | Sites.Read.All | `GET /me/insights/shared/{id}/resource` |
| 开发人员提供 `{user-id or upn}` AND `{insight-id}` AND `insight-type` 设置为 `shared` | Sites.Read.All | `GET /users/{id or userPrincipalName}/insights/shared/{id}/resource` |

## <a name="templates"></a>模板

组件 `mgt-file` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。 若要指定模板，请包含 `<template>` 组件内的元素，将 `data-type` 值设置为下列值之一：

| 数据类型 | 数据上下文 | 说明 |
| ----------- | -------------- | ------------- |
| loading | 无 | 组件在加载状态时要呈现的模板。 |
| no-data | 无 | 在文件数据不可用时要呈现的模板。 |
| default | file：文件详细信息对象 | 默认模板将整个组件替换为你自己的组件。 |

## <a name="authentication"></a>身份验证

该控件使用身份验证文档中介绍的全局身份验证提供程序[](../providers/providers.md)获取所需数据。

## <a name="cache"></a>缓存

|对象存储|缓存数据|备注|
|---------|-----------|-------|
|`driveFiles`|按驱动器 ID 列出文件|提供时 `driveId` 使用|
|`groupFiles`|按组 ID 列出文件|提供时 `groupId` 使用|
|`siteFiles`|按网站 ID 列出文件|提供时 `siteId` 使用|
|`userFiles`|按用户 ID 列出文件|提供时 `userId` 使用|
|`insightFiles`|按见解列出文件|提供 和 `insightType` `insightId` 时使用|
|`fileQueries`|按查询列出文件|提供时 `fileQuery` 使用|

若要详细了解如何配置缓存[，请参阅Caching](../customize-components/cache.md)。
