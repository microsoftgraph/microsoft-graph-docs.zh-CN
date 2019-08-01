---
title: ListItemVersion 资源类型
description: '**listItemVersion** 资源表示先前版本的 ListItem 资源。'
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: resourcePageType
ms.openlocfilehash: 8523e77fd308ab4863a0c3d90ccacad73cc766cc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036447"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="c608f-103">ListItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="c608f-103">ListItemVersion resource type</span></span>

<span data-ttu-id="c608f-104">**listItemVersion** 资源表示先前版本的 [ListItem](listitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="c608f-104">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="c608f-105">ListItemVersion 资源上的任务</span><span class="sxs-lookup"><span data-stu-id="c608f-105">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="c608f-106">下列任务可用于 listItemVersion 资源。</span><span class="sxs-lookup"><span data-stu-id="c608f-106">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="c608f-107">常见任务</span><span class="sxs-lookup"><span data-stu-id="c608f-107">Common task</span></span>             |         <span data-ttu-id="c608f-108">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="c608f-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="c608f-109">[列出版本][version-list]</span><span class="sxs-lookup"><span data-stu-id="c608f-109">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="c608f-110">[获取版本][version-get]</span><span class="sxs-lookup"><span data-stu-id="c608f-110">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="c608f-111">[还原版本][version-restore]</span><span class="sxs-lookup"><span data-stu-id="c608f-111">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="c608f-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c608f-112">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="c608f-113">属性</span><span class="sxs-lookup"><span data-stu-id="c608f-113">Properties</span></span>

|      <span data-ttu-id="c608f-114">属性名称</span><span class="sxs-lookup"><span data-stu-id="c608f-114">Property name</span></span>       |                         <span data-ttu-id="c608f-115">类型</span><span class="sxs-lookup"><span data-stu-id="c608f-115">Type</span></span>                         |                               <span data-ttu-id="c608f-116">说明</span><span class="sxs-lookup"><span data-stu-id="c608f-116">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="c608f-117">**id**</span><span class="sxs-lookup"><span data-stu-id="c608f-117">**id**</span></span>                   | <span data-ttu-id="c608f-118">string</span><span class="sxs-lookup"><span data-stu-id="c608f-118">string</span></span>                                               | <span data-ttu-id="c608f-119">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="c608f-119">The ID of the version.</span></span> <span data-ttu-id="c608f-120">只读。</span><span class="sxs-lookup"><span data-stu-id="c608f-120">Read-only.</span></span>                                       |
| <span data-ttu-id="c608f-121">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="c608f-121">**lastModifiedBy**</span></span>       | [<span data-ttu-id="c608f-122">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="c608f-122">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="c608f-123">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="c608f-123">Identity of the user which last modified the version.</span></span> <span data-ttu-id="c608f-124">只读。</span><span class="sxs-lookup"><span data-stu-id="c608f-124">Read-only.</span></span>        |
| <span data-ttu-id="c608f-125">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="c608f-125">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="c608f-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c608f-126">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="c608f-127">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c608f-127">Date and time the version was last modified.</span></span> <span data-ttu-id="c608f-128">只读。</span><span class="sxs-lookup"><span data-stu-id="c608f-128">Read-only.</span></span>                 |
| <span data-ttu-id="c608f-129">**published**</span><span class="sxs-lookup"><span data-stu-id="c608f-129">**published**</span></span>            | [<span data-ttu-id="c608f-130">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="c608f-130">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="c608f-131">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="c608f-131">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="c608f-132">只读。</span><span class="sxs-lookup"><span data-stu-id="c608f-132">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="c608f-133">关系</span><span class="sxs-lookup"><span data-stu-id="c608f-133">Relationships</span></span>

<span data-ttu-id="c608f-134">下表定义了 **driveItemVersion** 资源与其他资源的关系。</span><span class="sxs-lookup"><span data-stu-id="c608f-134">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="c608f-135">关系名称</span><span class="sxs-lookup"><span data-stu-id="c608f-135">Relationship name</span></span> |                      <span data-ttu-id="c608f-136">类型</span><span class="sxs-lookup"><span data-stu-id="c608f-136">Type</span></span>                      |                               <span data-ttu-id="c608f-137">说明</span><span class="sxs-lookup"><span data-stu-id="c608f-137">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="c608f-138">**fields**</span><span class="sxs-lookup"><span data-stu-id="c608f-138">**fields**</span></span>        | [<span data-ttu-id="c608f-139">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="c608f-139">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="c608f-140">此版本列表项的字段和值集合。</span><span class="sxs-lookup"><span data-stu-id="c608f-140">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
