---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/17/2017
title: DriveItemVersion
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 2f8b846652f930bd7d9337c0accc0ccbe7a60d1a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334558"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="27ebe-102">DriveItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="27ebe-102">DriveItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27ebe-103">**DriveItemVersion** 资源表示特定版本的 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="27ebe-103">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="27ebe-104">DriveItemVersion 资源上的任务</span><span class="sxs-lookup"><span data-stu-id="27ebe-104">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="27ebe-105">下列任务可用于 driveItemVersion 资源。</span><span class="sxs-lookup"><span data-stu-id="27ebe-105">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="27ebe-106">常见任务</span><span class="sxs-lookup"><span data-stu-id="27ebe-106">Common task</span></span>             |         <span data-ttu-id="27ebe-107">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="27ebe-107">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="27ebe-108">[列出版本][version-list]</span><span class="sxs-lookup"><span data-stu-id="27ebe-108">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="27ebe-109">[获取版本][version-get]</span><span class="sxs-lookup"><span data-stu-id="27ebe-109">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="27ebe-110">[获取内容][content-get]</span><span class="sxs-lookup"><span data-stu-id="27ebe-110">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="27ebe-111">[还原版本][version-restore]</span><span class="sxs-lookup"><span data-stu-id="27ebe-111">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="27ebe-112">在上表中，各示例使用的是 `/drive`，但有很多有效的请求。</span><span class="sxs-lookup"><span data-stu-id="27ebe-112">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="27ebe-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="27ebe-113">JSON representation</span></span>

<!-- { "blockType": "resource","keyProperty":"id", "@odata.type": "microsoft.graph.driveItemVersion", "@type.aka": "oneDrive.driveItemVersion" } -->

```json
{
  "content": {"@odata.type": "Edm.Stream"},
  "id": "string",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": {"@odata.type": "microsoft.graph.publicationFacet"},
  "size": 12356
}
```

## <a name="properties"></a><span data-ttu-id="27ebe-114">属性</span><span class="sxs-lookup"><span data-stu-id="27ebe-114">Properties</span></span>

|      <span data-ttu-id="27ebe-115">属性名称</span><span class="sxs-lookup"><span data-stu-id="27ebe-115">Property name</span></span>       |                         <span data-ttu-id="27ebe-116">类型</span><span class="sxs-lookup"><span data-stu-id="27ebe-116">Type</span></span>                         |                               <span data-ttu-id="27ebe-117">说明</span><span class="sxs-lookup"><span data-stu-id="27ebe-117">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="27ebe-118">**id**</span><span class="sxs-lookup"><span data-stu-id="27ebe-118">**id**</span></span>                   | <span data-ttu-id="27ebe-119">string</span><span class="sxs-lookup"><span data-stu-id="27ebe-119">string</span></span>                                               | <span data-ttu-id="27ebe-120">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="27ebe-120">The ID of the version.</span></span> <span data-ttu-id="27ebe-121">只读。</span><span class="sxs-lookup"><span data-stu-id="27ebe-121">Read-only.</span></span>                                       |
| <span data-ttu-id="27ebe-122">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="27ebe-122">**lastModifiedBy**</span></span>       | [<span data-ttu-id="27ebe-123">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="27ebe-123">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="27ebe-124">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="27ebe-124">Identity of the user which last modified the version.</span></span> <span data-ttu-id="27ebe-125">只读。</span><span class="sxs-lookup"><span data-stu-id="27ebe-125">Read-only.</span></span>        |
| <span data-ttu-id="27ebe-126">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="27ebe-126">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="27ebe-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27ebe-127">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="27ebe-128">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="27ebe-128">Date and time the version was last modified.</span></span> <span data-ttu-id="27ebe-129">只读。</span><span class="sxs-lookup"><span data-stu-id="27ebe-129">Read-only.</span></span>                 |
| <span data-ttu-id="27ebe-130">**publication**</span><span class="sxs-lookup"><span data-stu-id="27ebe-130">**publication**</span></span>          | [<span data-ttu-id="27ebe-131">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="27ebe-131">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="27ebe-132">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="27ebe-132">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="27ebe-133">只读。</span><span class="sxs-lookup"><span data-stu-id="27ebe-133">Read-only.</span></span> |
| <span data-ttu-id="27ebe-134">**size**</span><span class="sxs-lookup"><span data-stu-id="27ebe-134">**size**</span></span>                 | <span data-ttu-id="27ebe-135">Int64</span><span class="sxs-lookup"><span data-stu-id="27ebe-135">Int64</span></span>                                                | <span data-ttu-id="27ebe-136">指示此版本项的内容流大小。</span><span class="sxs-lookup"><span data-stu-id="27ebe-136">Indicates the size of the content stream for this version of the item.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="27ebe-137">关系</span><span class="sxs-lookup"><span data-stu-id="27ebe-137">Relationships</span></span>

<span data-ttu-id="27ebe-138">下表定义了 **driveItemVersion** 资源与其他资源的关系。</span><span class="sxs-lookup"><span data-stu-id="27ebe-138">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="27ebe-139">关系名称</span><span class="sxs-lookup"><span data-stu-id="27ebe-139">Relationship name</span></span> |  <span data-ttu-id="27ebe-140">类型</span><span class="sxs-lookup"><span data-stu-id="27ebe-140">Type</span></span>  |            <span data-ttu-id="27ebe-141">说明</span><span class="sxs-lookup"><span data-stu-id="27ebe-141">Description</span></span>             |
| :---------------- | :----- | :--------------------------------- |
| <span data-ttu-id="27ebe-142">**content**</span><span class="sxs-lookup"><span data-stu-id="27ebe-142">**content**</span></span>       | <span data-ttu-id="27ebe-143">Stream</span><span class="sxs-lookup"><span data-stu-id="27ebe-143">Stream</span></span> | <span data-ttu-id="27ebe-144">版本的内容流。</span><span class="sxs-lookup"><span data-stu-id="27ebe-144">The content stream of the version.</span></span> |

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
