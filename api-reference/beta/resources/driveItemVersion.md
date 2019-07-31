---
author: JeremyKelley
description: DriveItemVersion 资源表示特定版本的 DriveItem。
ms.date: 09/17/2017
title: DriveItemVersion
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: e3886c27ded6b26082609933d5ac7382dc182b45
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973088"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="d0704-103">DriveItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="d0704-103">DriveItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0704-104">**DriveItemVersion** 资源表示特定版本的 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="d0704-104">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="d0704-105">DriveItemVersion 资源上的任务</span><span class="sxs-lookup"><span data-stu-id="d0704-105">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="d0704-106">下列任务可用于 driveItemVersion 资源。</span><span class="sxs-lookup"><span data-stu-id="d0704-106">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="d0704-107">常见任务</span><span class="sxs-lookup"><span data-stu-id="d0704-107">Common task</span></span>             |         <span data-ttu-id="d0704-108">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="d0704-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="d0704-109">[列出版本][version-list]</span><span class="sxs-lookup"><span data-stu-id="d0704-109">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="d0704-110">[获取版本][version-get]</span><span class="sxs-lookup"><span data-stu-id="d0704-110">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="d0704-111">[获取内容][content-get]</span><span class="sxs-lookup"><span data-stu-id="d0704-111">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="d0704-112">[还原版本][version-restore]</span><span class="sxs-lookup"><span data-stu-id="d0704-112">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="d0704-113">在上表中，各示例使用的是 `/drive`，但有很多有效的请求。</span><span class="sxs-lookup"><span data-stu-id="d0704-113">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0704-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0704-114">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="d0704-115">属性</span><span class="sxs-lookup"><span data-stu-id="d0704-115">Properties</span></span>

|      <span data-ttu-id="d0704-116">属性名称</span><span class="sxs-lookup"><span data-stu-id="d0704-116">Property name</span></span>       |                         <span data-ttu-id="d0704-117">类型</span><span class="sxs-lookup"><span data-stu-id="d0704-117">Type</span></span>                         |                               <span data-ttu-id="d0704-118">说明</span><span class="sxs-lookup"><span data-stu-id="d0704-118">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="d0704-119">**id**</span><span class="sxs-lookup"><span data-stu-id="d0704-119">**id**</span></span>                   | <span data-ttu-id="d0704-120">string</span><span class="sxs-lookup"><span data-stu-id="d0704-120">string</span></span>                                               | <span data-ttu-id="d0704-121">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="d0704-121">The ID of the version.</span></span> <span data-ttu-id="d0704-122">只读。</span><span class="sxs-lookup"><span data-stu-id="d0704-122">Read-only.</span></span>                                       |
| <span data-ttu-id="d0704-123">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="d0704-123">**lastModifiedBy**</span></span>       | [<span data-ttu-id="d0704-124">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="d0704-124">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="d0704-125">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="d0704-125">Identity of the user which last modified the version.</span></span> <span data-ttu-id="d0704-126">只读。</span><span class="sxs-lookup"><span data-stu-id="d0704-126">Read-only.</span></span>        |
| <span data-ttu-id="d0704-127">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="d0704-127">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="d0704-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0704-128">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="d0704-129">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d0704-129">Date and time the version was last modified.</span></span> <span data-ttu-id="d0704-130">只读。</span><span class="sxs-lookup"><span data-stu-id="d0704-130">Read-only.</span></span>                 |
| <span data-ttu-id="d0704-131">**publication**</span><span class="sxs-lookup"><span data-stu-id="d0704-131">**publication**</span></span>          | [<span data-ttu-id="d0704-132">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="d0704-132">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="d0704-133">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="d0704-133">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="d0704-134">只读。</span><span class="sxs-lookup"><span data-stu-id="d0704-134">Read-only.</span></span> |
| <span data-ttu-id="d0704-135">**size**</span><span class="sxs-lookup"><span data-stu-id="d0704-135">**size**</span></span>                 | <span data-ttu-id="d0704-136">Int64</span><span class="sxs-lookup"><span data-stu-id="d0704-136">Int64</span></span>                                                | <span data-ttu-id="d0704-137">指示此版本项的内容流大小。</span><span class="sxs-lookup"><span data-stu-id="d0704-137">Indicates the size of the content stream for this version of the item.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="d0704-138">关系</span><span class="sxs-lookup"><span data-stu-id="d0704-138">Relationships</span></span>

<span data-ttu-id="d0704-139">下表定义了 **driveItemVersion** 资源与其他资源的关系。</span><span class="sxs-lookup"><span data-stu-id="d0704-139">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="d0704-140">关系名称</span><span class="sxs-lookup"><span data-stu-id="d0704-140">Relationship name</span></span> |  <span data-ttu-id="d0704-141">类型</span><span class="sxs-lookup"><span data-stu-id="d0704-141">Type</span></span>  |            <span data-ttu-id="d0704-142">说明</span><span class="sxs-lookup"><span data-stu-id="d0704-142">Description</span></span>             |
| :---------------- | :----- | :--------------------------------- |
| <span data-ttu-id="d0704-143">**content**</span><span class="sxs-lookup"><span data-stu-id="d0704-143">**content**</span></span>       | <span data-ttu-id="d0704-144">Stream</span><span class="sxs-lookup"><span data-stu-id="d0704-144">Stream</span></span> | <span data-ttu-id="d0704-145">版本的内容流。</span><span class="sxs-lookup"><span data-stu-id="d0704-145">The content stream of the version.</span></span> |

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
