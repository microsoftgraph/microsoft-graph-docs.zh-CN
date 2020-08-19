---
title: ListItemVersion 资源类型
description: '**listItemVersion** 资源表示先前版本的 ListItem 资源。'
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: resourcePageType
ms.openlocfilehash: 73b1c0e8f98a5f7ef321632e06619ba040cbd020
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807750"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="2befb-103">ListItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="2befb-103">ListItemVersion resource type</span></span>

<span data-ttu-id="2befb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2befb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2befb-105">**listItemVersion** 资源表示先前版本的 [ListItem](listitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="2befb-105">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="2befb-106">ListItemVersion 资源上的任务</span><span class="sxs-lookup"><span data-stu-id="2befb-106">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="2befb-107">下列任务可用于 listItemVersion 资源。</span><span class="sxs-lookup"><span data-stu-id="2befb-107">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="2befb-108">常见任务</span><span class="sxs-lookup"><span data-stu-id="2befb-108">Common task</span></span>             |         <span data-ttu-id="2befb-109">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="2befb-109">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="2befb-110">[列出版本][version-list]</span><span class="sxs-lookup"><span data-stu-id="2befb-110">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="2befb-111">[获取版本][version-get]</span><span class="sxs-lookup"><span data-stu-id="2befb-111">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="2befb-112">[还原版本][version-restore]</span><span class="sxs-lookup"><span data-stu-id="2befb-112">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="2befb-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2befb-113">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.listItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "published": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="2befb-114">属性</span><span class="sxs-lookup"><span data-stu-id="2befb-114">Properties</span></span>

|      <span data-ttu-id="2befb-115">属性名称</span><span class="sxs-lookup"><span data-stu-id="2befb-115">Property name</span></span>       |                         <span data-ttu-id="2befb-116">类型</span><span class="sxs-lookup"><span data-stu-id="2befb-116">Type</span></span>                         |                               <span data-ttu-id="2befb-117">说明</span><span class="sxs-lookup"><span data-stu-id="2befb-117">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="2befb-118">**id**</span><span class="sxs-lookup"><span data-stu-id="2befb-118">**id**</span></span>                   | <span data-ttu-id="2befb-119">string</span><span class="sxs-lookup"><span data-stu-id="2befb-119">string</span></span>                                               | <span data-ttu-id="2befb-120">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="2befb-120">The ID of the version.</span></span> <span data-ttu-id="2befb-121">只读。</span><span class="sxs-lookup"><span data-stu-id="2befb-121">Read-only.</span></span>                                       |
| <span data-ttu-id="2befb-122">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="2befb-122">**lastModifiedBy**</span></span>       | [<span data-ttu-id="2befb-123">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="2befb-123">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="2befb-124">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="2befb-124">Identity of the user which last modified the version.</span></span> <span data-ttu-id="2befb-125">只读。</span><span class="sxs-lookup"><span data-stu-id="2befb-125">Read-only.</span></span>        |
| <span data-ttu-id="2befb-126">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="2befb-126">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="2befb-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2befb-127">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="2befb-128">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2befb-128">Date and time the version was last modified.</span></span> <span data-ttu-id="2befb-129">只读。</span><span class="sxs-lookup"><span data-stu-id="2befb-129">Read-only.</span></span>                 |
| <span data-ttu-id="2befb-130">**published**</span><span class="sxs-lookup"><span data-stu-id="2befb-130">**published**</span></span>            | [<span data-ttu-id="2befb-131">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="2befb-131">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="2befb-132">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="2befb-132">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="2befb-133">只读。</span><span class="sxs-lookup"><span data-stu-id="2befb-133">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="2befb-134">关系</span><span class="sxs-lookup"><span data-stu-id="2befb-134">Relationships</span></span>

<span data-ttu-id="2befb-135">下表定义了 **driveItemVersion** 资源与其他资源的关系。</span><span class="sxs-lookup"><span data-stu-id="2befb-135">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="2befb-136">关系名称</span><span class="sxs-lookup"><span data-stu-id="2befb-136">Relationship name</span></span> |                      <span data-ttu-id="2befb-137">类型</span><span class="sxs-lookup"><span data-stu-id="2befb-137">Type</span></span>                      |                               <span data-ttu-id="2befb-138">说明</span><span class="sxs-lookup"><span data-stu-id="2befb-138">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="2befb-139">**fields**</span><span class="sxs-lookup"><span data-stu-id="2befb-139">**fields**</span></span>        | [<span data-ttu-id="2befb-140">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="2befb-140">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="2befb-141">此版本列表项的字段和值集合。</span><span class="sxs-lookup"><span data-stu-id="2befb-141">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
