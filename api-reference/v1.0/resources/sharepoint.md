---
title: 使用 Microsoft Graph 中的 SharePoint 网站
description: Microsoft Graph 中的 SharePoint API 支持以下核心情形：
ms.localizationpriority: high
ms.prod: sharepoint
author: JeremyKelley
doc_type: conceptualPageType
ms.openlocfilehash: 705f1cd142cbcccef6c05046b8747354c4d05836
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021433"
---
# <a name="working-with-sharepoint-sites-in-microsoft-graph"></a>使用 Microsoft Graph 中的 SharePoint 网站

Microsoft Graph 中的 SharePoint API 支持以下核心情形：

* 访问 SharePoint **网站**、**列表** 和 **驱动器**（文档库）
* 支持对 **site** 资源进行只读访问（无法创建新网站）
* 支持对 **lists**、**listItems** 和 **driveItems** 进行读写访问
* 用 SharePoint ID、URL 或相对路径表示的 Address 资源

SharePoint API 公开了三种主要资源类型：

* [Site](site.md) _（顶层的对象）_
* [List](list.md)
* [ListItem](listitem.md)

下面的示例展示了 listItem 资源。

```json
{
  "fields": {
    "Title": "Access card",
    "Employee": "Ryan Gregg",
    "EmployeeId": "10",
    "CardSerial": "01235492",
    "Alias": "RGregg",
    "ID": 1,
    "ContentType": "Item",
    "Modified": "2016-09-19T23:15:25-07:00",
    "Created": "2016-09-19T23:15:25-07:00"
  },
  "createdBy": {
    "user": {
      "id": "b757fdcb-0271-4807-b243-504139e4ba04",
      "displayName": "Ryan Gregg"
    }
  },
  "createdDateTime": "2016-09-20T06:15:25Z",
  "eTag": "48e941c3-9515-4c48-9760-c07c90c79d48,1",
  "id": "4",
  "lastModifiedBy": {
    "user": {
      "id": "b757fdcb-0271-4807-b243-504139e4ba04",
      "displayName": "Ryan Gregg"
    }
  },
  "lastModifiedDateTime": "2016-09-20T06:15:25Z",
}
```

资源通过三种不同的方式公开数据：

* _属性_（如 **id** 和 **name**）公开简单值。
* _Facet_（如 **fields** 和 **createdBy**）公开复杂值。
* _引用_（如 **items**）指向其他资源的集合。

可以使用 _expand_ 查询参数展开 URL 中的引用；例如 `?expand=fields`。
可以使用 _select_ 查询参数请求特定属性和 facet；例如 `?select=id,name`。
默认情况下，虽然大部分属性和 Facet 都会返回，但所有引用都会被隐藏。
为了提高效率，建议将 _select_ 和 _expand_ 指定为仅返回你关注的数据。

## <a name="sharepoint-api-root-resources"></a>SharePoint API 根资源

以下示例与 `https://graph.microsoft.com/v1.0` 有关。

| 路径                                   | 说明
|:---------------------------------------|:------------------------------------
| /sites/root                            | 组织的默认[网站][]。
| /sites/{site-id}                       | 通过其 ID 访问特定[网站][]。
| /sites/{site-id}/drive                 | 访问给定[网站][]的默认[驱动器](drive.md)（文档库）。
| /sites/{site-id}/drives                | 枚举[网站][]下的[驱动器](drive.md)（文档库）。
| /sites/{site-id}/sites                 | 枚举[网站][]下的子网站。
| /sites/{site-id}/lists                 | 枚举[网站](site.md)下的[列表](list.md)。
| /sites/{site-id}/lists/{list-id}/items | 枚举[列表](list.md)下的 [listItem](listitem.md)。
| /groups/{group-id}/sites/root          | 访问组的团队[网站][]。

还可以使用 SharePoint 主机名，后面加上冒号和网站的相对路径，来为网站寻址。可以选择将另一个冒号置于末尾，转回为资源模型寻址。

| Path                                           | 说明
|:-----------------------------------------------|:-----------------------------------
| /sites/contoso.sharepoint.com:/teams/hr        | 与 https://contoso.sharepoint.com/teams/hr 相关联的网站
| /sites/contoso.sharepoint.com:/teams/hr:/drive | 访问此网站的默认[驱动器](drive.md)。

## <a name="note-for-existing-sharepoint-developers"></a>现有 SharePoint 开发人员须知

Microsoft Graph SharePoint API 与 CSOM API 有几个主要区别。
[网站][] 资源映射到 `SPWeb`。
网站集中的根[网站][] (`SPWeb`) 具有 [siteCollection](sitecollection.md) facet，其中包含有关 `SPSite` 的信息。
由于网站 ID 只在其网站集中是唯一的，因此按 ID 为网站寻址需要提供网站集标识符和网站标识符。

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname},{spsite-id},{spweb-id}/
```
仅使用主机名构造的 URL 将指向默认网站集中的根网站 (`SPWeb`)。

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname}
```

仅使用主机名和 siteCollection (`SPSite`) ID 构造的 URL 将指向给定网站集中的根网站 (`SPWeb`)。

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname},{spsite-id}
```

仅使用 siteCollection (`SPSite`) ID 构造的 URL 将指向给定网站集中的根网站 (`SPWeb`)。

```http
GET https://graph.microsoft.com/v1.0/sites/{spsite-id}
```

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

[网站]: site.md
[list]: list.md
[drive]: drive.md
[siteCollection]: sitecollection.md

<!-- {
  "type": "#page.annotation",
  "description": "Getting started programming with the SharePoint API",
  "keywords": "getting started sharepoint rest api programming C# ios android rest http",
  "section": "documentation",
  "tocPath": "Getting Started",
  "tocIndex": -100
} -->

