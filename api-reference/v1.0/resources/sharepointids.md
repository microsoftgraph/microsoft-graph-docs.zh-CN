---
author: JeremyKelley
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.prod: sharepoint
description: SharePointIds 资源将存储在 SharePoint 网站或 OneDrive for Business 中的项的各种标识符分组到一个单一结构。
doc_type: resourcePageType
ms.openlocfilehash: 38a186772ebdd4bf1bf0a35dc9789e96fdbd2ed2
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240085"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="500d9-103">SharePointIds 资源类型</span><span class="sxs-lookup"><span data-stu-id="500d9-103">SharePointIds resource type</span></span>

<span data-ttu-id="500d9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="500d9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="500d9-105">**SharePointIds** 资源将存储在 SharePoint 网站或 OneDrive for Business 中的项的各种标识符分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="500d9-105">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="500d9-106">**注意：** OneDrive 个人版返回的项将不包括 **SharePointIds** 方面。</span><span class="sxs-lookup"><span data-stu-id="500d9-106">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="500d9-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="500d9-107">JSON representation</span></span>

<span data-ttu-id="500d9-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="500d9-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "listId", "listItemId", "listItemUniqueId", "siteId", "siteUrl", "webId" ],
  "@odata.type": "microsoft.graph.sharepointIds"
}-->

```json
{
    "listId": "string",
    "listItemId": "string",
    "listItemUniqueId": "string",
    "siteId": "string",
    "siteUrl": "url",
    "tenantId": "string",
    "webId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="500d9-109">属性</span><span class="sxs-lookup"><span data-stu-id="500d9-109">Properties</span></span>

| <span data-ttu-id="500d9-110">属性</span><span class="sxs-lookup"><span data-stu-id="500d9-110">Property</span></span>         | <span data-ttu-id="500d9-111">类型</span><span class="sxs-lookup"><span data-stu-id="500d9-111">Type</span></span>         | <span data-ttu-id="500d9-112">说明</span><span class="sxs-lookup"><span data-stu-id="500d9-112">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="500d9-113">listId</span><span class="sxs-lookup"><span data-stu-id="500d9-113">listId</span></span>           | <span data-ttu-id="500d9-114">string</span><span class="sxs-lookup"><span data-stu-id="500d9-114">string</span></span>       | <span data-ttu-id="500d9-115">SharePoint 中的项列表的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="500d9-115">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="500d9-116">listItemId</span><span class="sxs-lookup"><span data-stu-id="500d9-116">listItemId</span></span>       | <span data-ttu-id="500d9-117">string</span><span class="sxs-lookup"><span data-stu-id="500d9-117">string</span></span>       | <span data-ttu-id="500d9-118">包含列表中的项的整数标识符。</span><span class="sxs-lookup"><span data-stu-id="500d9-118">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="500d9-119">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="500d9-119">listItemUniqueId</span></span> | <span data-ttu-id="500d9-120">string</span><span class="sxs-lookup"><span data-stu-id="500d9-120">string</span></span>       | <span data-ttu-id="500d9-121">OneDrive for Business 或 SharePoint 网站中的项的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="500d9-121">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="500d9-122">siteId</span><span class="sxs-lookup"><span data-stu-id="500d9-122">siteId</span></span>           | <span data-ttu-id="500d9-123">string</span><span class="sxs-lookup"><span data-stu-id="500d9-123">string</span></span>       | <span data-ttu-id="500d9-124">项的网站集 (SPSite) 的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="500d9-124">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="500d9-125">siteUrl</span><span class="sxs-lookup"><span data-stu-id="500d9-125">siteUrl</span></span>          | <span data-ttu-id="500d9-126">string (url)</span><span class="sxs-lookup"><span data-stu-id="500d9-126">string (url)</span></span> | <span data-ttu-id="500d9-127">包含项的网站的 SharePoint URL。</span><span class="sxs-lookup"><span data-stu-id="500d9-127">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="500d9-128">tenantId</span><span class="sxs-lookup"><span data-stu-id="500d9-128">tenantId</span></span>         | <span data-ttu-id="500d9-129">string</span><span class="sxs-lookup"><span data-stu-id="500d9-129">string</span></span>       | <span data-ttu-id="500d9-130">租户的唯 (guid) 标识符。</span><span class="sxs-lookup"><span data-stu-id="500d9-130">The unique identifier (guid) for the tenancy.</span></span>
| <span data-ttu-id="500d9-131">webId</span><span class="sxs-lookup"><span data-stu-id="500d9-131">webId</span></span>            | <span data-ttu-id="500d9-132">string</span><span class="sxs-lookup"><span data-stu-id="500d9-132">string</span></span>       | <span data-ttu-id="500d9-133">项的网站集 (SPWeb) 的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="500d9-133">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="500d9-134">注解</span><span class="sxs-lookup"><span data-stu-id="500d9-134">Remarks</span></span>

<span data-ttu-id="500d9-135">有关 **driveItem** 上 facet 的详细信息，请参阅 [**driveItem**](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="500d9-135">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->

