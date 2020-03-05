---
author: JeremyKelley
description: SharePointIds 资源将存储在 SharePoint 网站或 OneDrive for Business 中的项的各种标识符分组到一个单一结构。
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: e22c653bf2dd88fe75fdb43dd8e9601c2a9d6d4e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520686"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="097db-103">SharePointIds 资源类型</span><span class="sxs-lookup"><span data-stu-id="097db-103">SharePointIds resource type</span></span>

<span data-ttu-id="097db-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="097db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="097db-105">**SharePointIds** 资源将存储在 SharePoint 网站或 OneDrive for Business 中的项的各种标识符分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="097db-105">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="097db-106">**注意：** OneDrive 个人版返回的项将不包括 **SharePointIds** 方面。</span><span class="sxs-lookup"><span data-stu-id="097db-106">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="097db-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="097db-107">JSON representation</span></span>

<span data-ttu-id="097db-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="097db-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="097db-109">属性</span><span class="sxs-lookup"><span data-stu-id="097db-109">Properties</span></span>

| <span data-ttu-id="097db-110">属性</span><span class="sxs-lookup"><span data-stu-id="097db-110">Property</span></span>         | <span data-ttu-id="097db-111">类型</span><span class="sxs-lookup"><span data-stu-id="097db-111">Type</span></span>         | <span data-ttu-id="097db-112">说明</span><span class="sxs-lookup"><span data-stu-id="097db-112">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="097db-113">listId</span><span class="sxs-lookup"><span data-stu-id="097db-113">listId</span></span>           | <span data-ttu-id="097db-114">string</span><span class="sxs-lookup"><span data-stu-id="097db-114">string</span></span>       | <span data-ttu-id="097db-115">SharePoint 中的项列表的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="097db-115">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="097db-116">listItemId</span><span class="sxs-lookup"><span data-stu-id="097db-116">listItemId</span></span>       | <span data-ttu-id="097db-117">string</span><span class="sxs-lookup"><span data-stu-id="097db-117">string</span></span>       | <span data-ttu-id="097db-118">包含列表中的项的整数标识符。</span><span class="sxs-lookup"><span data-stu-id="097db-118">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="097db-119">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="097db-119">listItemUniqueId</span></span> | <span data-ttu-id="097db-120">string</span><span class="sxs-lookup"><span data-stu-id="097db-120">string</span></span>       | <span data-ttu-id="097db-121">OneDrive for Business 或 SharePoint 网站中的项的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="097db-121">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="097db-122">siteId</span><span class="sxs-lookup"><span data-stu-id="097db-122">siteId</span></span>           | <span data-ttu-id="097db-123">string</span><span class="sxs-lookup"><span data-stu-id="097db-123">string</span></span>       | <span data-ttu-id="097db-124">项的网站集 (SPSite) 的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="097db-124">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="097db-125">siteUrl</span><span class="sxs-lookup"><span data-stu-id="097db-125">siteUrl</span></span>          | <span data-ttu-id="097db-126">string (url)</span><span class="sxs-lookup"><span data-stu-id="097db-126">string (url)</span></span> | <span data-ttu-id="097db-127">包含项的网站的 SharePoint URL。</span><span class="sxs-lookup"><span data-stu-id="097db-127">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="097db-128">tenantId</span><span class="sxs-lookup"><span data-stu-id="097db-128">tenantId</span></span>         | <span data-ttu-id="097db-129">string</span><span class="sxs-lookup"><span data-stu-id="097db-129">string</span></span>       | <span data-ttu-id="097db-130">租赁的唯一标识符（guid）。</span><span class="sxs-lookup"><span data-stu-id="097db-130">The unique identifier (guid) for the tenancy.</span></span>
| <span data-ttu-id="097db-131">webId</span><span class="sxs-lookup"><span data-stu-id="097db-131">webId</span></span>            | <span data-ttu-id="097db-132">string</span><span class="sxs-lookup"><span data-stu-id="097db-132">string</span></span>       | <span data-ttu-id="097db-133">项的网站集 (SPWeb) 的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="097db-133">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="097db-134">注解</span><span class="sxs-lookup"><span data-stu-id="097db-134">Remarks</span></span>

<span data-ttu-id="097db-135">有关 **driveItem** 上 facet 的详细信息，请参阅 [**driveItem**](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="097db-135">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



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
