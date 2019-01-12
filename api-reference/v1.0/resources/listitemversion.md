---
title: ListItemVersion 资源类型
description: '**listItemVersion** 资源表示先前版本的 ListItem 资源。'
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 6e21be59b71a8f348931603c799ebbbe225e5d3f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951843"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="02ee8-103">ListItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="02ee8-103">ListItemVersion resource type</span></span>

<span data-ttu-id="02ee8-104">**listItemVersion** 资源表示先前版本的 [ListItem](listitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="02ee8-104">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="02ee8-105">ListItemVersion 资源上的任务</span><span class="sxs-lookup"><span data-stu-id="02ee8-105">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="02ee8-106">下列任务可用于 listItemVersion 资源。</span><span class="sxs-lookup"><span data-stu-id="02ee8-106">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="02ee8-107">常见任务</span><span class="sxs-lookup"><span data-stu-id="02ee8-107">Common task</span></span>             |         <span data-ttu-id="02ee8-108">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="02ee8-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="02ee8-109">[列出版本][version-list]</span><span class="sxs-lookup"><span data-stu-id="02ee8-109">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="02ee8-110">[获取版本][version-get]</span><span class="sxs-lookup"><span data-stu-id="02ee8-110">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="02ee8-111">[还原版本][version-restore]</span><span class="sxs-lookup"><span data-stu-id="02ee8-111">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="02ee8-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02ee8-112">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="02ee8-113">属性</span><span class="sxs-lookup"><span data-stu-id="02ee8-113">Properties</span></span>

|      <span data-ttu-id="02ee8-114">属性名称</span><span class="sxs-lookup"><span data-stu-id="02ee8-114">Property name</span></span>       |                         <span data-ttu-id="02ee8-115">类型</span><span class="sxs-lookup"><span data-stu-id="02ee8-115">Type</span></span>                         |                               <span data-ttu-id="02ee8-116">说明</span><span class="sxs-lookup"><span data-stu-id="02ee8-116">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="02ee8-117">**id**</span><span class="sxs-lookup"><span data-stu-id="02ee8-117">**id**</span></span>                   | <span data-ttu-id="02ee8-118">string</span><span class="sxs-lookup"><span data-stu-id="02ee8-118">string</span></span>                                               | <span data-ttu-id="02ee8-119">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="02ee8-119">The ID of the version.</span></span> <span data-ttu-id="02ee8-120">只读。</span><span class="sxs-lookup"><span data-stu-id="02ee8-120">Read-only.</span></span>                                       |
| <span data-ttu-id="02ee8-121">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="02ee8-121">**lastModifiedBy**</span></span>       | [<span data-ttu-id="02ee8-122">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="02ee8-122">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="02ee8-123">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="02ee8-123">Identity of the user which last modified the version.</span></span> <span data-ttu-id="02ee8-124">只读。</span><span class="sxs-lookup"><span data-stu-id="02ee8-124">Read-only.</span></span>        |
| <span data-ttu-id="02ee8-125">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="02ee8-125">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="02ee8-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02ee8-126">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="02ee8-127">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="02ee8-127">Date and time the version was last modified.</span></span> <span data-ttu-id="02ee8-128">只读。</span><span class="sxs-lookup"><span data-stu-id="02ee8-128">Read-only.</span></span>                 |
| <span data-ttu-id="02ee8-129">**published**</span><span class="sxs-lookup"><span data-stu-id="02ee8-129">**published**</span></span>            | [<span data-ttu-id="02ee8-130">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="02ee8-130">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="02ee8-131">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="02ee8-131">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="02ee8-132">只读。</span><span class="sxs-lookup"><span data-stu-id="02ee8-132">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="02ee8-133">关系</span><span class="sxs-lookup"><span data-stu-id="02ee8-133">Relationships</span></span>

<span data-ttu-id="02ee8-134">下表定义了 **driveItemVersion** 资源与其他资源的关系。</span><span class="sxs-lookup"><span data-stu-id="02ee8-134">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="02ee8-135">关系名称</span><span class="sxs-lookup"><span data-stu-id="02ee8-135">Relationship name</span></span> |                      <span data-ttu-id="02ee8-136">类型</span><span class="sxs-lookup"><span data-stu-id="02ee8-136">Type</span></span>                      |                               <span data-ttu-id="02ee8-137">说明</span><span class="sxs-lookup"><span data-stu-id="02ee8-137">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="02ee8-138">**fields**</span><span class="sxs-lookup"><span data-stu-id="02ee8-138">**fields**</span></span>        | [<span data-ttu-id="02ee8-139">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="02ee8-139">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="02ee8-140">此版本列表项的字段和值集合。</span><span class="sxs-lookup"><span data-stu-id="02ee8-140">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
