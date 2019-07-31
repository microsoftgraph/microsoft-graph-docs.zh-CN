---
author: JeremyKelley
description: SharePointIds 资源将存储在 SharePoint 网站或 OneDrive for Business 中的项的各种标识符分组到一个单一结构。
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: c7e18e43bcbe9c73500701577c752e7a30d47194
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965122"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="15da9-103">SharePointIds 资源类型</span><span class="sxs-lookup"><span data-stu-id="15da9-103">SharePointIds resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15da9-104">**SharePointIds** 资源将存储在 SharePoint 网站或 OneDrive for Business 中的项的各种标识符分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="15da9-104">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="15da9-105">**注意：** OneDrive 个人版返回的项将不包括 **SharePointIds** 方面。</span><span class="sxs-lookup"><span data-stu-id="15da9-105">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="15da9-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="15da9-106">JSON representation</span></span>

<span data-ttu-id="15da9-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15da9-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="15da9-108">属性</span><span class="sxs-lookup"><span data-stu-id="15da9-108">Properties</span></span>

| <span data-ttu-id="15da9-109">属性</span><span class="sxs-lookup"><span data-stu-id="15da9-109">Property</span></span>         | <span data-ttu-id="15da9-110">类型</span><span class="sxs-lookup"><span data-stu-id="15da9-110">Type</span></span>         | <span data-ttu-id="15da9-111">说明</span><span class="sxs-lookup"><span data-stu-id="15da9-111">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="15da9-112">listId</span><span class="sxs-lookup"><span data-stu-id="15da9-112">listId</span></span>           | <span data-ttu-id="15da9-113">string</span><span class="sxs-lookup"><span data-stu-id="15da9-113">string</span></span>       | <span data-ttu-id="15da9-114">SharePoint 中的项列表的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="15da9-114">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="15da9-115">listItemId</span><span class="sxs-lookup"><span data-stu-id="15da9-115">listItemId</span></span>       | <span data-ttu-id="15da9-116">string</span><span class="sxs-lookup"><span data-stu-id="15da9-116">string</span></span>       | <span data-ttu-id="15da9-117">包含列表中的项的整数标识符。</span><span class="sxs-lookup"><span data-stu-id="15da9-117">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="15da9-118">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="15da9-118">listItemUniqueId</span></span> | <span data-ttu-id="15da9-119">string</span><span class="sxs-lookup"><span data-stu-id="15da9-119">string</span></span>       | <span data-ttu-id="15da9-120">OneDrive for Business 或 SharePoint 网站中的项的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="15da9-120">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="15da9-121">siteId</span><span class="sxs-lookup"><span data-stu-id="15da9-121">siteId</span></span>           | <span data-ttu-id="15da9-122">string</span><span class="sxs-lookup"><span data-stu-id="15da9-122">string</span></span>       | <span data-ttu-id="15da9-123">项的网站集 (SPSite) 的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="15da9-123">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="15da9-124">siteUrl</span><span class="sxs-lookup"><span data-stu-id="15da9-124">siteUrl</span></span>          | <span data-ttu-id="15da9-125">string (url)</span><span class="sxs-lookup"><span data-stu-id="15da9-125">string (url)</span></span> | <span data-ttu-id="15da9-126">包含项的网站的 SharePoint URL。</span><span class="sxs-lookup"><span data-stu-id="15da9-126">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="15da9-127">tenantId</span><span class="sxs-lookup"><span data-stu-id="15da9-127">tenantId</span></span>         | <span data-ttu-id="15da9-128">string</span><span class="sxs-lookup"><span data-stu-id="15da9-128">string</span></span>       | <span data-ttu-id="15da9-129">租赁的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="15da9-129">The unique identifier (guid) for the tenancy.</span></span>
| <span data-ttu-id="15da9-130">webId</span><span class="sxs-lookup"><span data-stu-id="15da9-130">webId</span></span>            | <span data-ttu-id="15da9-131">string</span><span class="sxs-lookup"><span data-stu-id="15da9-131">string</span></span>       | <span data-ttu-id="15da9-132">项的网站集 (SPWeb) 的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="15da9-132">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="15da9-133">注解</span><span class="sxs-lookup"><span data-stu-id="15da9-133">Remarks</span></span>

<span data-ttu-id="15da9-134">有关 **driveItem** 上 facet 的详细信息，请参阅 [**driveItem**](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="15da9-134">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds",
  "suppressions": []
}
-->
