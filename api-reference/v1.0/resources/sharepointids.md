---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 233c2aa4b8ce67b2382996181c9ba2ab57b9e69c
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480264"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="e9c92-102">SharePointIds 资源类型</span><span class="sxs-lookup"><span data-stu-id="e9c92-102">SharePointIds resource type</span></span>

<span data-ttu-id="e9c92-103">**SharePointIds** 资源将存储在 SharePoint 网站或 OneDrive for Business 中的项的各种标识符分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="e9c92-103">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="e9c92-104">**注意：** OneDrive 个人版返回的项将不包括 **SharePointIds** 方面。</span><span class="sxs-lookup"><span data-stu-id="e9c92-104">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9c92-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e9c92-105">JSON representation</span></span>

<span data-ttu-id="e9c92-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9c92-106">Here is a JSON representation of the resource</span></span>

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
    "webId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="e9c92-107">属性</span><span class="sxs-lookup"><span data-stu-id="e9c92-107">Properties</span></span>

| <span data-ttu-id="e9c92-108">属性</span><span class="sxs-lookup"><span data-stu-id="e9c92-108">Property</span></span>         | <span data-ttu-id="e9c92-109">类型</span><span class="sxs-lookup"><span data-stu-id="e9c92-109">Type</span></span>         | <span data-ttu-id="e9c92-110">说明</span><span class="sxs-lookup"><span data-stu-id="e9c92-110">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="e9c92-111">listId</span><span class="sxs-lookup"><span data-stu-id="e9c92-111">listId</span></span>           | <span data-ttu-id="e9c92-112">string</span><span class="sxs-lookup"><span data-stu-id="e9c92-112">string</span></span>       | <span data-ttu-id="e9c92-113">SharePoint 中的项列表的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="e9c92-113">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="e9c92-114">listItemId</span><span class="sxs-lookup"><span data-stu-id="e9c92-114">listItemId</span></span>       | <span data-ttu-id="e9c92-115">string</span><span class="sxs-lookup"><span data-stu-id="e9c92-115">string</span></span>       | <span data-ttu-id="e9c92-116">包含列表中的项的整数标识符。</span><span class="sxs-lookup"><span data-stu-id="e9c92-116">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="e9c92-117">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="e9c92-117">listItemUniqueId</span></span> | <span data-ttu-id="e9c92-118">string</span><span class="sxs-lookup"><span data-stu-id="e9c92-118">string</span></span>       | <span data-ttu-id="e9c92-119">OneDrive for Business 或 SharePoint 网站中的项的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="e9c92-119">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="e9c92-120">siteId</span><span class="sxs-lookup"><span data-stu-id="e9c92-120">siteId</span></span>           | <span data-ttu-id="e9c92-121">string</span><span class="sxs-lookup"><span data-stu-id="e9c92-121">string</span></span>       | <span data-ttu-id="e9c92-122">项的网站集 (SPSite) 的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="e9c92-122">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="e9c92-123">siteUrl</span><span class="sxs-lookup"><span data-stu-id="e9c92-123">siteUrl</span></span>          | <span data-ttu-id="e9c92-124">string (url)</span><span class="sxs-lookup"><span data-stu-id="e9c92-124">string (url)</span></span> | <span data-ttu-id="e9c92-125">包含项的网站的 SharePoint URL。</span><span class="sxs-lookup"><span data-stu-id="e9c92-125">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="e9c92-126">webId</span><span class="sxs-lookup"><span data-stu-id="e9c92-126">webId</span></span>            | <span data-ttu-id="e9c92-127">string</span><span class="sxs-lookup"><span data-stu-id="e9c92-127">string</span></span>       | <span data-ttu-id="e9c92-128">项的网站集 (SPWeb) 的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="e9c92-128">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="e9c92-129">注解</span><span class="sxs-lookup"><span data-stu-id="e9c92-129">Remarks</span></span>

<span data-ttu-id="e9c92-130">有关 **driveItem** 上 facet 的详细信息，请参阅 [**driveItem**](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="e9c92-130">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->
