---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 01e4c3087f9504255975ab28f935ceed8815b6b0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343092"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="acdc1-102">SharePointIds 资源类型</span><span class="sxs-lookup"><span data-stu-id="acdc1-102">SharePointIds resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acdc1-103">**SharePointIds** 资源将存储在 SharePoint 网站或 OneDrive for Business 中的项的各种标识符分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="acdc1-103">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="acdc1-104">**注意：** OneDrive 个人版返回的项将不包括 **SharePointIds** 方面。</span><span class="sxs-lookup"><span data-stu-id="acdc1-104">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="acdc1-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="acdc1-105">JSON representation</span></span>

<span data-ttu-id="acdc1-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="acdc1-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="acdc1-107">属性</span><span class="sxs-lookup"><span data-stu-id="acdc1-107">Properties</span></span>

| <span data-ttu-id="acdc1-108">属性</span><span class="sxs-lookup"><span data-stu-id="acdc1-108">Property</span></span>         | <span data-ttu-id="acdc1-109">类型</span><span class="sxs-lookup"><span data-stu-id="acdc1-109">Type</span></span>         | <span data-ttu-id="acdc1-110">说明</span><span class="sxs-lookup"><span data-stu-id="acdc1-110">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="acdc1-111">listId</span><span class="sxs-lookup"><span data-stu-id="acdc1-111">listId</span></span>           | <span data-ttu-id="acdc1-112">string</span><span class="sxs-lookup"><span data-stu-id="acdc1-112">string</span></span>       | <span data-ttu-id="acdc1-113">SharePoint 中的项列表的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="acdc1-113">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="acdc1-114">listItemId</span><span class="sxs-lookup"><span data-stu-id="acdc1-114">listItemId</span></span>       | <span data-ttu-id="acdc1-115">string</span><span class="sxs-lookup"><span data-stu-id="acdc1-115">string</span></span>       | <span data-ttu-id="acdc1-116">包含列表中的项的整数标识符。</span><span class="sxs-lookup"><span data-stu-id="acdc1-116">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="acdc1-117">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="acdc1-117">listItemUniqueId</span></span> | <span data-ttu-id="acdc1-118">string</span><span class="sxs-lookup"><span data-stu-id="acdc1-118">string</span></span>       | <span data-ttu-id="acdc1-119">OneDrive for Business 或 SharePoint 网站中的项的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="acdc1-119">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="acdc1-120">siteId</span><span class="sxs-lookup"><span data-stu-id="acdc1-120">siteId</span></span>           | <span data-ttu-id="acdc1-121">string</span><span class="sxs-lookup"><span data-stu-id="acdc1-121">string</span></span>       | <span data-ttu-id="acdc1-122">项的网站集 (SPSite) 的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="acdc1-122">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="acdc1-123">siteUrl</span><span class="sxs-lookup"><span data-stu-id="acdc1-123">siteUrl</span></span>          | <span data-ttu-id="acdc1-124">string (url)</span><span class="sxs-lookup"><span data-stu-id="acdc1-124">string (url)</span></span> | <span data-ttu-id="acdc1-125">包含项的网站的 SharePoint URL。</span><span class="sxs-lookup"><span data-stu-id="acdc1-125">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="acdc1-126">tenantId</span><span class="sxs-lookup"><span data-stu-id="acdc1-126">tenantId</span></span>         | <span data-ttu-id="acdc1-127">string</span><span class="sxs-lookup"><span data-stu-id="acdc1-127">string</span></span>       | <span data-ttu-id="acdc1-128">租赁的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="acdc1-128">The unique identifier (guid) for the tenancy.</span></span>
| <span data-ttu-id="acdc1-129">webId</span><span class="sxs-lookup"><span data-stu-id="acdc1-129">webId</span></span>            | <span data-ttu-id="acdc1-130">string</span><span class="sxs-lookup"><span data-stu-id="acdc1-130">string</span></span>       | <span data-ttu-id="acdc1-131">项的网站集 (SPWeb) 的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="acdc1-131">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="acdc1-132">注解</span><span class="sxs-lookup"><span data-stu-id="acdc1-132">Remarks</span></span>

<span data-ttu-id="acdc1-133">有关 **driveItem** 上 facet 的详细信息，请参阅 [**driveItem**](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="acdc1-133">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



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
