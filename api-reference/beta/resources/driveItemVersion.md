---
author: JeremyKelley
description: DriveItemVersion 资源表示特定版本的 DriveItem。
ms.date: 09/17/2017
title: DriveItemVersion
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: ec7abdcb6ae65ebe3333289dca384448a1569988
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505656"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="11a1f-103">DriveItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="11a1f-103">DriveItemVersion resource type</span></span>

<span data-ttu-id="11a1f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="11a1f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11a1f-105">**DriveItemVersion** 资源表示特定版本的 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="11a1f-105">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="11a1f-106">DriveItemVersion 资源上的任务</span><span class="sxs-lookup"><span data-stu-id="11a1f-106">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="11a1f-107">下列任务可用于 driveItemVersion 资源。</span><span class="sxs-lookup"><span data-stu-id="11a1f-107">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="11a1f-108">常见任务</span><span class="sxs-lookup"><span data-stu-id="11a1f-108">Common task</span></span>             |         <span data-ttu-id="11a1f-109">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="11a1f-109">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="11a1f-110">[列出版本][version-list]</span><span class="sxs-lookup"><span data-stu-id="11a1f-110">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="11a1f-111">[获取版本][version-get]</span><span class="sxs-lookup"><span data-stu-id="11a1f-111">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="11a1f-112">[获取内容][content-get]</span><span class="sxs-lookup"><span data-stu-id="11a1f-112">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="11a1f-113">[还原版本][version-restore]</span><span class="sxs-lookup"><span data-stu-id="11a1f-113">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="11a1f-114">在上表中，各示例使用的是 `/drive`，但有很多有效的请求。</span><span class="sxs-lookup"><span data-stu-id="11a1f-114">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="11a1f-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11a1f-115">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="11a1f-116">属性</span><span class="sxs-lookup"><span data-stu-id="11a1f-116">Properties</span></span>

|      <span data-ttu-id="11a1f-117">属性名称</span><span class="sxs-lookup"><span data-stu-id="11a1f-117">Property name</span></span>       |                         <span data-ttu-id="11a1f-118">类型</span><span class="sxs-lookup"><span data-stu-id="11a1f-118">Type</span></span>                         |                               <span data-ttu-id="11a1f-119">说明</span><span class="sxs-lookup"><span data-stu-id="11a1f-119">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="11a1f-120">**id**</span><span class="sxs-lookup"><span data-stu-id="11a1f-120">**id**</span></span>                   | <span data-ttu-id="11a1f-121">string</span><span class="sxs-lookup"><span data-stu-id="11a1f-121">string</span></span>                                               | <span data-ttu-id="11a1f-122">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="11a1f-122">The ID of the version.</span></span> <span data-ttu-id="11a1f-123">只读。</span><span class="sxs-lookup"><span data-stu-id="11a1f-123">Read-only.</span></span>                                       |
| <span data-ttu-id="11a1f-124">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="11a1f-124">**lastModifiedBy**</span></span>       | [<span data-ttu-id="11a1f-125">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="11a1f-125">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="11a1f-126">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="11a1f-126">Identity of the user which last modified the version.</span></span> <span data-ttu-id="11a1f-127">只读。</span><span class="sxs-lookup"><span data-stu-id="11a1f-127">Read-only.</span></span>        |
| <span data-ttu-id="11a1f-128">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="11a1f-128">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="11a1f-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11a1f-129">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="11a1f-130">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="11a1f-130">Date and time the version was last modified.</span></span> <span data-ttu-id="11a1f-131">只读。</span><span class="sxs-lookup"><span data-stu-id="11a1f-131">Read-only.</span></span>                 |
| <span data-ttu-id="11a1f-132">**publication**</span><span class="sxs-lookup"><span data-stu-id="11a1f-132">**publication**</span></span>          | [<span data-ttu-id="11a1f-133">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="11a1f-133">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="11a1f-134">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="11a1f-134">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="11a1f-135">只读。</span><span class="sxs-lookup"><span data-stu-id="11a1f-135">Read-only.</span></span> |
| <span data-ttu-id="11a1f-136">**size**</span><span class="sxs-lookup"><span data-stu-id="11a1f-136">**size**</span></span>                 | <span data-ttu-id="11a1f-137">Int64</span><span class="sxs-lookup"><span data-stu-id="11a1f-137">Int64</span></span>                                                | <span data-ttu-id="11a1f-138">指示此版本项的内容流大小。</span><span class="sxs-lookup"><span data-stu-id="11a1f-138">Indicates the size of the content stream for this version of the item.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="11a1f-139">关系</span><span class="sxs-lookup"><span data-stu-id="11a1f-139">Relationships</span></span>

<span data-ttu-id="11a1f-140">下表定义了 **driveItemVersion** 资源与其他资源的关系。</span><span class="sxs-lookup"><span data-stu-id="11a1f-140">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="11a1f-141">关系名称</span><span class="sxs-lookup"><span data-stu-id="11a1f-141">Relationship name</span></span> |  <span data-ttu-id="11a1f-142">类型</span><span class="sxs-lookup"><span data-stu-id="11a1f-142">Type</span></span>  |            <span data-ttu-id="11a1f-143">说明</span><span class="sxs-lookup"><span data-stu-id="11a1f-143">Description</span></span>             |
| :---------------- | :----- | :--------------------------------- |
| <span data-ttu-id="11a1f-144">**content**</span><span class="sxs-lookup"><span data-stu-id="11a1f-144">**content**</span></span>       | <span data-ttu-id="11a1f-145">Stream</span><span class="sxs-lookup"><span data-stu-id="11a1f-145">Stream</span></span> | <span data-ttu-id="11a1f-146">版本的内容流。</span><span class="sxs-lookup"><span data-stu-id="11a1f-146">The content stream of the version.</span></span> |

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
