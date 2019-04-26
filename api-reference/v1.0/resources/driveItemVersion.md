---
title: DriveItemVersion 资源类型
description: '**DriveItemVersion**资源表示 DriveItem 的特定版本。'
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: fd6052464d40fcce86b83d93601282dda252c69b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562683"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="788ef-103">DriveItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="788ef-103">DriveItemVersion resource type</span></span>

<span data-ttu-id="788ef-104">**DriveItemVersion** 资源表示特定版本的 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="788ef-104">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="788ef-105">DriveItemVersion 资源上的任务</span><span class="sxs-lookup"><span data-stu-id="788ef-105">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="788ef-106">下列任务可用于 driveItemVersion 资源。</span><span class="sxs-lookup"><span data-stu-id="788ef-106">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="788ef-107">常见任务</span><span class="sxs-lookup"><span data-stu-id="788ef-107">Common task</span></span>             |         <span data-ttu-id="788ef-108">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="788ef-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="788ef-109">[列出版本][version-list]</span><span class="sxs-lookup"><span data-stu-id="788ef-109">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="788ef-110">[获取版本][version-get]</span><span class="sxs-lookup"><span data-stu-id="788ef-110">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="788ef-111">[获取内容][content-get]</span><span class="sxs-lookup"><span data-stu-id="788ef-111">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="788ef-112">[还原版本][version-restore]</span><span class="sxs-lookup"><span data-stu-id="788ef-112">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="788ef-113">在上表中，各示例使用的是 `/drive`，但有很多有效的请求。</span><span class="sxs-lookup"><span data-stu-id="788ef-113">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="788ef-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="788ef-114">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="788ef-115">属性</span><span class="sxs-lookup"><span data-stu-id="788ef-115">Properties</span></span>

|      <span data-ttu-id="788ef-116">属性名称</span><span class="sxs-lookup"><span data-stu-id="788ef-116">Property name</span></span>       |                         <span data-ttu-id="788ef-117">类型</span><span class="sxs-lookup"><span data-stu-id="788ef-117">Type</span></span>                         |                               <span data-ttu-id="788ef-118">说明</span><span class="sxs-lookup"><span data-stu-id="788ef-118">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="788ef-119">**id**</span><span class="sxs-lookup"><span data-stu-id="788ef-119">**id**</span></span>                   | <span data-ttu-id="788ef-120">string</span><span class="sxs-lookup"><span data-stu-id="788ef-120">string</span></span>                                               | <span data-ttu-id="788ef-121">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="788ef-121">The ID of the version.</span></span> <span data-ttu-id="788ef-122">只读。</span><span class="sxs-lookup"><span data-stu-id="788ef-122">Read-only.</span></span>                                       |
| <span data-ttu-id="788ef-123">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="788ef-123">**lastModifiedBy**</span></span>       | [<span data-ttu-id="788ef-124">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="788ef-124">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="788ef-125">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="788ef-125">Identity of the user which last modified the version.</span></span> <span data-ttu-id="788ef-126">只读。</span><span class="sxs-lookup"><span data-stu-id="788ef-126">Read-only.</span></span>        |
| <span data-ttu-id="788ef-127">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="788ef-127">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="788ef-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="788ef-128">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="788ef-129">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="788ef-129">Date and time the version was last modified.</span></span> <span data-ttu-id="788ef-130">只读。</span><span class="sxs-lookup"><span data-stu-id="788ef-130">Read-only.</span></span>                 |
| <span data-ttu-id="788ef-131">**publication**</span><span class="sxs-lookup"><span data-stu-id="788ef-131">**publication**</span></span>          | [<span data-ttu-id="788ef-132">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="788ef-132">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="788ef-133">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="788ef-133">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="788ef-134">只读。</span><span class="sxs-lookup"><span data-stu-id="788ef-134">Read-only.</span></span> |
| <span data-ttu-id="788ef-135">**size**</span><span class="sxs-lookup"><span data-stu-id="788ef-135">**size**</span></span>                 | <span data-ttu-id="788ef-136">Int64</span><span class="sxs-lookup"><span data-stu-id="788ef-136">Int64</span></span>                                                | <span data-ttu-id="788ef-137">指示此版本项的内容流大小。</span><span class="sxs-lookup"><span data-stu-id="788ef-137">Indicates the size of the content stream for this version of the item.</span></span>  |
| <span data-ttu-id="788ef-138">**content**</span><span class="sxs-lookup"><span data-stu-id="788ef-138">**content**</span></span>              | <span data-ttu-id="788ef-139">Stream</span><span class="sxs-lookup"><span data-stu-id="788ef-139">Stream</span></span>                                               | <span data-ttu-id="788ef-140">此版本项目的内容流。</span><span class="sxs-lookup"><span data-stu-id="788ef-140">The content stream for this version of the item.</span></span>                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
