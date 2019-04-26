---
title: onenote 资源类型
description: OneNote 资源的入口点。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 44dfe7b33632bb6691802e46b66f54015b6aa6ae
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341489"
---
# <a name="onenote-resource-type"></a>onenote 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

OneNote 资源的入口点。

通过 Microsoft Graph API 对 OneNote 服务进行的所有调用都使用此服务根 URL:

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

该位置可以是 office 365 上的用户笔记本, 也可以是 office 365 上的使用者 OneDrive、组笔记本或 SharePoint 网站托管的团队笔记本。 

**用户笔记本**若要访问消费者 OneDrive 或 OneDrive for business 上的个人笔记本, 请使用下列 url 之一:

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

**组笔记本**若要访问组拥有的笔记本, 请使用以下服务根 URL:

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
**SharePoint 网站笔记本**若要访问 SharePoint 团队网站拥有的笔记本, 请使用以下服务根 URL:

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a>Authorization

有关使用 OneNote api 所需的权限的信息, 请参阅[Notes 权限](/graph/permissions-reference#notes-permissions)。

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|notebooks|[notebook](notebook.md) 集合|用户或组拥有的 OneNote 笔记本的集合。 只读。 可为 NULL。|
|operations|[onenoteOperation](onenoteoperation.md)集合 |OneNote 操作的状态。 不支持获取操作集合, 但如果响应中返回了`Operation-Location`标头, 则可以获取长时间运行的操作的状态。 只读。 可为 Null。|
|pages|[onenotePage](onenotepage.md)集合|由用户或组拥有的所有 OneNote 笔记本中的页面。  只读。 可为 Null。|
|资源|[onenoteResource](onenoteresource.md)集合 |OneNote 页面中的图像和其他文件资源。 不支持获取资源集合, 但可以[获取特定资源的二进制内容](onenoteresource.md)。 只读。 可为 Null。|
|sectionGroups|[sectionGroup](sectiongroup.md)集合|由用户或组拥有的所有 OneNote 笔记本中的分区组。  只读。 可为 Null。|
|分区|[onenoteSection](onenotesection.md)集合|所有 OneNote 笔记本中由用户或组所有的部分。  只读。 可为 Null。|

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建笔记本](../api/onenote-post-notebooks.md) |[笔记](notebook.md)| 通过发布到 "笔记本" 集合创建笔记本。|
|[列出笔记本](../api/onenote-list-notebooks.md) |[notebook](notebook.md) 集合| 获取笔记本的集合。|
|[创建页面](../api/onenote-post-pages.md) |[onenotePage](onenotepage.md) | 通过发布到 pages 集合创建页面。|
|[列出页面](../api/onenote-list-pages.md) |[onenotePage](onenotepage.md)集合| 获取页面的集合。|
|[列出分区组](../api/onenote-list-sectiongroups.md) |[sectionGroup](sectiongroup.md)集合| 获取节组的集合。|
|[列出分区](../api/onenote-list-sections.md) |[onenoteSection](onenotesection.md)集合| 获取节的集合。|
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.onenote"
}-->
``` json
{
  "notebooks": [{ "@odata.type": "microsoft.graph.notebook" }],
  "operations": [{ "@odata.type": "microsoft.graph.onenoteOperation" }],
  "pages": [{ "@odata.type": "microsoft.graph.onenotePage" }],
  "resources": [ { "@odata.type": "microsoft.graph.onenoteResource" } ],
  "sectionGroups": [ { "@odata.type": "microsoft.graph.sectionGroup" } ],
  "sections": [ { "@odata.type": "microsoft.graph.onenoteSection" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
