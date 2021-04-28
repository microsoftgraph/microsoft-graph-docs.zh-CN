---
title: catalogEntry 资源类型
description: 您可以批准部署的内容段的元数据。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 5c9766fd93c0a550556cb7f47e3275f65c238de7
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067314"
---
# <a name="catalogentry-resource-type"></a><span data-ttu-id="153b6-103">catalogEntry 资源类型</span><span class="sxs-lookup"><span data-stu-id="153b6-103">catalogEntry resource type</span></span>

<span data-ttu-id="153b6-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="153b6-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="153b6-105">您可以批准部署的内容段的元数据。</span><span class="sxs-lookup"><span data-stu-id="153b6-105">Metadata for a piece of content that you can approve for deployment.</span></span>

<span data-ttu-id="153b6-106">所有目录项作为以下派生类型之一存在 [：featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) 和 [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md)。</span><span class="sxs-lookup"><span data-stu-id="153b6-106">All catalog entries exist as one of the following derived types: [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) and [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md).</span></span>

<span data-ttu-id="153b6-107">[softwareUpdateCatalogEntry 的基类型](../resources/windowsupdates-softwareupdatecatalogentry.md)。</span><span class="sxs-lookup"><span data-stu-id="153b6-107">Base type for [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>

<span data-ttu-id="153b6-108">这是一个抽象类型。</span><span class="sxs-lookup"><span data-stu-id="153b6-108">This is an abstract type.</span></span>

## <a name="properties"></a><span data-ttu-id="153b6-109">属性</span><span class="sxs-lookup"><span data-stu-id="153b6-109">Properties</span></span>
|<span data-ttu-id="153b6-110">属性</span><span class="sxs-lookup"><span data-stu-id="153b6-110">Property</span></span>|<span data-ttu-id="153b6-111">类型</span><span class="sxs-lookup"><span data-stu-id="153b6-111">Type</span></span>|<span data-ttu-id="153b6-112">说明</span><span class="sxs-lookup"><span data-stu-id="153b6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="153b6-113">deployableUntilDateTime</span><span class="sxs-lookup"><span data-stu-id="153b6-113">deployableUntilDateTime</span></span>|<span data-ttu-id="153b6-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="153b6-114">DateTimeOffset</span></span>|<span data-ttu-id="153b6-115">使用该服务不再提供内容部署的日期。</span><span class="sxs-lookup"><span data-stu-id="153b6-115">The date on which the content is no longer available to deploy using the service.</span></span> <span data-ttu-id="153b6-116">只读。</span><span class="sxs-lookup"><span data-stu-id="153b6-116">Read-only.</span></span>|
|<span data-ttu-id="153b6-117">displayName</span><span class="sxs-lookup"><span data-stu-id="153b6-117">displayName</span></span>|<span data-ttu-id="153b6-118">String</span><span class="sxs-lookup"><span data-stu-id="153b6-118">String</span></span>|<span data-ttu-id="153b6-119">内容的显示名称。</span><span class="sxs-lookup"><span data-stu-id="153b6-119">The display name of the content.</span></span> <span data-ttu-id="153b6-120">只读。</span><span class="sxs-lookup"><span data-stu-id="153b6-120">Read-only.</span></span>|
|<span data-ttu-id="153b6-121">id</span><span class="sxs-lookup"><span data-stu-id="153b6-121">id</span></span>|<span data-ttu-id="153b6-122">String</span><span class="sxs-lookup"><span data-stu-id="153b6-122">String</span></span>|<span data-ttu-id="153b6-123">目录项的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="153b6-123">The unique identifier for the catalog entry.</span></span> <span data-ttu-id="153b6-124">只读。</span><span class="sxs-lookup"><span data-stu-id="153b6-124">Read-only.</span></span>|
|<span data-ttu-id="153b6-125">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="153b6-125">releaseDateTime</span></span>|<span data-ttu-id="153b6-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="153b6-126">DateTimeOffset</span></span>|<span data-ttu-id="153b6-127">内容的发布日期。</span><span class="sxs-lookup"><span data-stu-id="153b6-127">The release date for the content.</span></span> <span data-ttu-id="153b6-128">只读。</span><span class="sxs-lookup"><span data-stu-id="153b6-128">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="153b6-129">关系</span><span class="sxs-lookup"><span data-stu-id="153b6-129">Relationships</span></span>
<span data-ttu-id="153b6-130">无。</span><span class="sxs-lookup"><span data-stu-id="153b6-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="153b6-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="153b6-131">JSON representation</span></span>
<span data-ttu-id="153b6-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="153b6-132">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.catalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.catalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)"
}
```

