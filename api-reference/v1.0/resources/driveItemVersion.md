---
title: driveItemVersion 资源类型
description: 表示 DriveItem 的特定版本。
ms.localizationpriority: medium
ms.prod: sharepoint
author: JeremyKelley
doc_type: resourcePageType
ms.openlocfilehash: 9dea3f33013c4d6fe0530c4f65253873ec3a1a69
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60354761"
---
# <a name="driveitemversion-resource-type"></a>driveItemVersion 资源类型

命名空间：microsoft.graph

表示 [driveItem 的特定版本](driveitem.md)。

以下任务可用于 **driveItemVersion** 资源。

|            常见任务             |         HTTP 方法         |
| :--------------------------------- | :-------------------------- |
| [列出版本][version-list]      | `GET /drive/items/{item-id}/versions`  |
| [获取版本][version-get]         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| [获取内容][content-get]        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| [还原版本][version-restore] | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

在上表中，各示例使用的是 `/drive`，但有很多有效的请求。

## <a name="properties"></a>属性

|      属性名称       |                         类型                         |                               说明                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | string                                               | 版本 ID。 只读。                                       |
| **lastModifiedBy**       | [IdentitySet](../resources/identityset.md)           | 上次修改版本的用户的标识。 只读。        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | 上次修改版本的日期和时间。 只读。                 |
| **publication**          | [PublicationFacet](../resources/publicationfacet.md) | 指示此特定版本的发布状态。 只读。 |
| **size**                 | Int64                                                | 指示此版本项的内容流大小。  |
| **content**              | Stream                                               | 此版本的项的内容流。                        |

## <a name="instance-attributes"></a>实例属性

| 属性名称                     | 类型   | 说明
|:----------------------------------|:-------|:--------------------------------
| @microsoft.graph.downloadUrl      | string | 可用于下载此版本的文件内容的 URL。 不需要使用此 URL 进行身份验证。 只读。

>**注意：**`@microsoft.graph.downloadUrl`该值是短期 URL，无法缓存。 此 URL 在失效前只能使用很短的时间（1 小时）。
>删除用户的文件权限可能不会立即使 URL 无效。

## <a name="json-representation"></a>JSON 表示形式

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.driveItemVersion",
  "@type.aka": "oneDrive.driveItemVersion"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" },
  "size": 12356,

  /* instance annotations */
  "@microsoft.graph.downloadUrl": "url",
}
```


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
