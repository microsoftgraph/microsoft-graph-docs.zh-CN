---
author: JeremyKelley
description: listItemVersion 资源表示先前版本的 ListItem 资源。
ms.date: 09/17/2017
title: ListItemVersion
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: ff3fbd3144a62939f9d4f6077c556c9d5884c687
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966954"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="f0068-103">ListItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0068-103">ListItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0068-104">**listItemVersion** 资源表示先前版本的 [ListItem](listitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="f0068-104">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="f0068-105">ListItemVersion 资源上的任务</span><span class="sxs-lookup"><span data-stu-id="f0068-105">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="f0068-106">下列任务可用于 listItemVersion 资源。</span><span class="sxs-lookup"><span data-stu-id="f0068-106">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="f0068-107">常见任务</span><span class="sxs-lookup"><span data-stu-id="f0068-107">Common task</span></span>             |         <span data-ttu-id="f0068-108">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="f0068-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="f0068-109">[列出版本][version-list]</span><span class="sxs-lookup"><span data-stu-id="f0068-109">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="f0068-110">[获取版本][version-get]</span><span class="sxs-lookup"><span data-stu-id="f0068-110">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| <span data-ttu-id="f0068-111">[还原版本][version-restore]</span><span class="sxs-lookup"><span data-stu-id="f0068-111">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="f0068-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0068-112">JSON representation</span></span>

<!-- { "blockType": "resource","keyProperty":"id", "@odata.type": "microsoft.graph.listItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

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

## <a name="properties"></a><span data-ttu-id="f0068-113">属性</span><span class="sxs-lookup"><span data-stu-id="f0068-113">Properties</span></span>

|      <span data-ttu-id="f0068-114">属性名称</span><span class="sxs-lookup"><span data-stu-id="f0068-114">Property name</span></span>       |                         <span data-ttu-id="f0068-115">类型</span><span class="sxs-lookup"><span data-stu-id="f0068-115">Type</span></span>                         |                               <span data-ttu-id="f0068-116">说明</span><span class="sxs-lookup"><span data-stu-id="f0068-116">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="f0068-117">**id**</span><span class="sxs-lookup"><span data-stu-id="f0068-117">**id**</span></span>                   | <span data-ttu-id="f0068-118">string</span><span class="sxs-lookup"><span data-stu-id="f0068-118">string</span></span>                                               | <span data-ttu-id="f0068-119">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="f0068-119">The ID of the version.</span></span> <span data-ttu-id="f0068-120">只读。</span><span class="sxs-lookup"><span data-stu-id="f0068-120">Read-only.</span></span>                                       |
| <span data-ttu-id="f0068-121">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="f0068-121">**lastModifiedBy**</span></span>       | [<span data-ttu-id="f0068-122">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="f0068-122">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="f0068-123">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="f0068-123">Identity of the user which last modified the version.</span></span> <span data-ttu-id="f0068-124">只读。</span><span class="sxs-lookup"><span data-stu-id="f0068-124">Read-only.</span></span>        |
| <span data-ttu-id="f0068-125">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="f0068-125">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="f0068-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0068-126">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="f0068-127">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f0068-127">Date and time the version was last modified.</span></span> <span data-ttu-id="f0068-128">只读。</span><span class="sxs-lookup"><span data-stu-id="f0068-128">Read-only.</span></span>                 |
| <span data-ttu-id="f0068-129">**published**</span><span class="sxs-lookup"><span data-stu-id="f0068-129">**published**</span></span>            | [<span data-ttu-id="f0068-130">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="f0068-130">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="f0068-131">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="f0068-131">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="f0068-132">只读。</span><span class="sxs-lookup"><span data-stu-id="f0068-132">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="f0068-133">关系</span><span class="sxs-lookup"><span data-stu-id="f0068-133">Relationships</span></span>

<span data-ttu-id="f0068-134">下表定义了 **driveItemVersion** 资源与其他资源的关系。</span><span class="sxs-lookup"><span data-stu-id="f0068-134">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="f0068-135">关系名称</span><span class="sxs-lookup"><span data-stu-id="f0068-135">Relationship name</span></span> |                      <span data-ttu-id="f0068-136">类型</span><span class="sxs-lookup"><span data-stu-id="f0068-136">Type</span></span>                      |                               <span data-ttu-id="f0068-137">说明</span><span class="sxs-lookup"><span data-stu-id="f0068-137">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="f0068-138">**fields**</span><span class="sxs-lookup"><span data-stu-id="f0068-138">**fields**</span></span>        | [<span data-ttu-id="f0068-139">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="f0068-139">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="f0068-140">此版本列表项的字段和值集合。</span><span class="sxs-lookup"><span data-stu-id="f0068-140">A collection of the fields and values for this version of the list item.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": []
}
-->
