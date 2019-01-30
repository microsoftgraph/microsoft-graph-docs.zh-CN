---
title: DriveItemVersion 资源类型
description: '**DriveItemVersion**资源表示 DriveItem 的特定版本。'
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: fd6052464d40fcce86b83d93601282dda252c69b
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643984"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="cc425-103">DriveItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc425-103">DriveItemVersion resource type</span></span>

<span data-ttu-id="cc425-104">**DriveItemVersion** 资源表示特定版本的 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="cc425-104">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="cc425-105">DriveItemVersion 资源上的任务</span><span class="sxs-lookup"><span data-stu-id="cc425-105">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="cc425-106">下列任务可用于 driveItemVersion 资源。</span><span class="sxs-lookup"><span data-stu-id="cc425-106">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="cc425-107">常见任务</span><span class="sxs-lookup"><span data-stu-id="cc425-107">Common task</span></span>             |         <span data-ttu-id="cc425-108">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="cc425-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="cc425-109">[列出版本][version-list]</span><span class="sxs-lookup"><span data-stu-id="cc425-109">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="cc425-110">[获取版本][version-get]</span><span class="sxs-lookup"><span data-stu-id="cc425-110">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="cc425-111">[获取内容][content-get]</span><span class="sxs-lookup"><span data-stu-id="cc425-111">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="cc425-112">[还原版本][version-restore]</span><span class="sxs-lookup"><span data-stu-id="cc425-112">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="cc425-113">在上表中，各示例使用的是 `/drive`，但有很多有效的请求。</span><span class="sxs-lookup"><span data-stu-id="cc425-113">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc425-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc425-114">JSON representation</span></span>

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
  "size": 12356
}
```

## <a name="properties"></a><span data-ttu-id="cc425-115">属性</span><span class="sxs-lookup"><span data-stu-id="cc425-115">Properties</span></span>

|      <span data-ttu-id="cc425-116">属性名称</span><span class="sxs-lookup"><span data-stu-id="cc425-116">Property name</span></span>       |                         <span data-ttu-id="cc425-117">类型</span><span class="sxs-lookup"><span data-stu-id="cc425-117">Type</span></span>                         |                               <span data-ttu-id="cc425-118">说明</span><span class="sxs-lookup"><span data-stu-id="cc425-118">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="cc425-119">**id**</span><span class="sxs-lookup"><span data-stu-id="cc425-119">**id**</span></span>                   | <span data-ttu-id="cc425-120">string</span><span class="sxs-lookup"><span data-stu-id="cc425-120">string</span></span>                                               | <span data-ttu-id="cc425-121">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="cc425-121">The ID of the version.</span></span> <span data-ttu-id="cc425-122">只读。</span><span class="sxs-lookup"><span data-stu-id="cc425-122">Read-only.</span></span>                                       |
| <span data-ttu-id="cc425-123">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="cc425-123">**lastModifiedBy**</span></span>       | [<span data-ttu-id="cc425-124">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="cc425-124">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="cc425-125">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="cc425-125">Identity of the user which last modified the version.</span></span> <span data-ttu-id="cc425-126">只读。</span><span class="sxs-lookup"><span data-stu-id="cc425-126">Read-only.</span></span>        |
| <span data-ttu-id="cc425-127">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="cc425-127">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="cc425-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc425-128">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="cc425-129">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cc425-129">Date and time the version was last modified.</span></span> <span data-ttu-id="cc425-130">只读。</span><span class="sxs-lookup"><span data-stu-id="cc425-130">Read-only.</span></span>                 |
| <span data-ttu-id="cc425-131">**publication**</span><span class="sxs-lookup"><span data-stu-id="cc425-131">**publication**</span></span>          | [<span data-ttu-id="cc425-132">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="cc425-132">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="cc425-133">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="cc425-133">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="cc425-134">只读。</span><span class="sxs-lookup"><span data-stu-id="cc425-134">Read-only.</span></span> |
| <span data-ttu-id="cc425-135">**size**</span><span class="sxs-lookup"><span data-stu-id="cc425-135">**size**</span></span>                 | <span data-ttu-id="cc425-136">Int64</span><span class="sxs-lookup"><span data-stu-id="cc425-136">Int64</span></span>                                                | <span data-ttu-id="cc425-137">指示此版本项的内容流大小。</span><span class="sxs-lookup"><span data-stu-id="cc425-137">Indicates the size of the content stream for this version of the item.</span></span>  |
| <span data-ttu-id="cc425-138">**content**</span><span class="sxs-lookup"><span data-stu-id="cc425-138">**content**</span></span>              | <span data-ttu-id="cc425-139">Stream</span><span class="sxs-lookup"><span data-stu-id="cc425-139">Stream</span></span>                                               | <span data-ttu-id="cc425-140">对于此版本的项目内容流。</span><span class="sxs-lookup"><span data-stu-id="cc425-140">The content stream for this version of the item.</span></span>                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
