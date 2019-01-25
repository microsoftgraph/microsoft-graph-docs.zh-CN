---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: listItemVersion
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1d153a8ae8291e0299d1a470db6c8c7e0c8bd3e4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524749"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="e6040-102">ListItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6040-102">ListItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6040-103">**listItemVersion** 资源表示先前版本的 [ListItem](listitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="e6040-103">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="e6040-104">ListItemVersion 资源上的任务</span><span class="sxs-lookup"><span data-stu-id="e6040-104">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="e6040-105">下列任务可用于 listItemVersion 资源。</span><span class="sxs-lookup"><span data-stu-id="e6040-105">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="e6040-106">常见任务</span><span class="sxs-lookup"><span data-stu-id="e6040-106">Common task</span></span>             |         <span data-ttu-id="e6040-107">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="e6040-107">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="e6040-108">[列出版本][version-list]</span><span class="sxs-lookup"><span data-stu-id="e6040-108">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="e6040-109">[获取版本][version-get]</span><span class="sxs-lookup"><span data-stu-id="e6040-109">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| <span data-ttu-id="e6040-110">[还原版本][version-restore]</span><span class="sxs-lookup"><span data-stu-id="e6040-110">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="e6040-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6040-111">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.listItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "published": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="e6040-112">属性</span><span class="sxs-lookup"><span data-stu-id="e6040-112">Properties</span></span>

|      <span data-ttu-id="e6040-113">属性名称</span><span class="sxs-lookup"><span data-stu-id="e6040-113">Property name</span></span>       |                         <span data-ttu-id="e6040-114">类型</span><span class="sxs-lookup"><span data-stu-id="e6040-114">Type</span></span>                         |                               <span data-ttu-id="e6040-115">说明</span><span class="sxs-lookup"><span data-stu-id="e6040-115">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="e6040-116">**id**</span><span class="sxs-lookup"><span data-stu-id="e6040-116">**id**</span></span>                   | <span data-ttu-id="e6040-117">string</span><span class="sxs-lookup"><span data-stu-id="e6040-117">string</span></span>                                               | <span data-ttu-id="e6040-118">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="e6040-118">The ID of the version.</span></span> <span data-ttu-id="e6040-119">只读。</span><span class="sxs-lookup"><span data-stu-id="e6040-119">Read-only.</span></span>                                       |
| <span data-ttu-id="e6040-120">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="e6040-120">**lastModifiedBy**</span></span>       | [<span data-ttu-id="e6040-121">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="e6040-121">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="e6040-122">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="e6040-122">Identity of the user which last modified the version.</span></span> <span data-ttu-id="e6040-123">只读。</span><span class="sxs-lookup"><span data-stu-id="e6040-123">Read-only.</span></span>        |
| <span data-ttu-id="e6040-124">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="e6040-124">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="e6040-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6040-125">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="e6040-126">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e6040-126">Date and time the version was last modified.</span></span> <span data-ttu-id="e6040-127">只读。</span><span class="sxs-lookup"><span data-stu-id="e6040-127">Read-only.</span></span>                 |
| <span data-ttu-id="e6040-128">**published**</span><span class="sxs-lookup"><span data-stu-id="e6040-128">**published**</span></span>            | [<span data-ttu-id="e6040-129">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="e6040-129">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="e6040-130">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="e6040-130">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="e6040-131">只读。</span><span class="sxs-lookup"><span data-stu-id="e6040-131">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="e6040-132">关系</span><span class="sxs-lookup"><span data-stu-id="e6040-132">Relationships</span></span>

<span data-ttu-id="e6040-133">下表定义了 **driveItemVersion** 资源与其他资源的关系。</span><span class="sxs-lookup"><span data-stu-id="e6040-133">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="e6040-134">关系名称</span><span class="sxs-lookup"><span data-stu-id="e6040-134">Relationship name</span></span> |                      <span data-ttu-id="e6040-135">类型</span><span class="sxs-lookup"><span data-stu-id="e6040-135">Type</span></span>                      |                               <span data-ttu-id="e6040-136">说明</span><span class="sxs-lookup"><span data-stu-id="e6040-136">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="e6040-137">**fields**</span><span class="sxs-lookup"><span data-stu-id="e6040-137">**fields**</span></span>        | [<span data-ttu-id="e6040-138">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="e6040-138">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="e6040-139">此版本列表项的字段和值集合。</span><span class="sxs-lookup"><span data-stu-id="e6040-139">A collection of the fields and values for this version of the list item.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": [
    "Error: /api-reference/beta/resources/listitemversion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
