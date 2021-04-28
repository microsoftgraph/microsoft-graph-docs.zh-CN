---
title: featureUpdateCatalogEntry 资源类型
description: 可以批准Windows 10部署的功能更新的元数据。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 64ad4c2506a2d8f90276e50e7fe5288e1af1d8db
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067317"
---
# <a name="featureupdatecatalogentry-resource-type"></a><span data-ttu-id="06b78-103">featureUpdateCatalogEntry 资源类型</span><span class="sxs-lookup"><span data-stu-id="06b78-103">featureUpdateCatalogEntry resource type</span></span>

<span data-ttu-id="06b78-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="06b78-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06b78-105">可以批准Windows 10部署的功能更新的元数据。</span><span class="sxs-lookup"><span data-stu-id="06b78-105">Metadata for a Windows 10 feature update that you can approve for deployment.</span></span>

<span data-ttu-id="06b78-106">Windows 10功能更新每两年发布一次，其中包含适用于Windows 10。</span><span class="sxs-lookup"><span data-stu-id="06b78-106">Windows 10 feature updates are released bi-annually and contain new features for Windows 10.</span></span> <span data-ttu-id="06b78-107">安装这些更新会增加Windows 10内部版本数，并且通常会导致新的服务生命周期和服务结束日期。</span><span class="sxs-lookup"><span data-stu-id="06b78-107">Installing these updates increases the Windows 10 build number and typically results in a new servicing lifecycle and end of service date.</span></span> <span data-ttu-id="06b78-108">Microsoft 建议组织定期部署新功能更新，作为采用Windows服务的一部分。</span><span class="sxs-lookup"><span data-stu-id="06b78-108">Microsoft recommends organizations regularly deploy new feature updates as part of adopting Windows as a service.</span></span>

<span data-ttu-id="06b78-109">继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。</span><span class="sxs-lookup"><span data-stu-id="06b78-109">Inherits from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>

## <a name="properties"></a><span data-ttu-id="06b78-110">属性</span><span class="sxs-lookup"><span data-stu-id="06b78-110">Properties</span></span>
|<span data-ttu-id="06b78-111">属性</span><span class="sxs-lookup"><span data-stu-id="06b78-111">Property</span></span>|<span data-ttu-id="06b78-112">类型</span><span class="sxs-lookup"><span data-stu-id="06b78-112">Type</span></span>|<span data-ttu-id="06b78-113">说明</span><span class="sxs-lookup"><span data-stu-id="06b78-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06b78-114">deployableUntilDateTime</span><span class="sxs-lookup"><span data-stu-id="06b78-114">deployableUntilDateTime</span></span>|<span data-ttu-id="06b78-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06b78-115">DateTimeOffset</span></span>|<span data-ttu-id="06b78-116">内容不再可用于使用服务部署的日期。</span><span class="sxs-lookup"><span data-stu-id="06b78-116">The date on which the content is no longer available for deployment using the service.</span></span> <span data-ttu-id="06b78-117">只读。</span><span class="sxs-lookup"><span data-stu-id="06b78-117">Read-only.</span></span> <span data-ttu-id="06b78-118">继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。</span><span class="sxs-lookup"><span data-stu-id="06b78-118">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|
|<span data-ttu-id="06b78-119">displayName</span><span class="sxs-lookup"><span data-stu-id="06b78-119">displayName</span></span>|<span data-ttu-id="06b78-120">String</span><span class="sxs-lookup"><span data-stu-id="06b78-120">String</span></span>|<span data-ttu-id="06b78-121">内容的显示名称。</span><span class="sxs-lookup"><span data-stu-id="06b78-121">The display name of the content.</span></span> <span data-ttu-id="06b78-122">只读。</span><span class="sxs-lookup"><span data-stu-id="06b78-122">Read-only.</span></span> <span data-ttu-id="06b78-123">继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。</span><span class="sxs-lookup"><span data-stu-id="06b78-123">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|
|<span data-ttu-id="06b78-124">id</span><span class="sxs-lookup"><span data-stu-id="06b78-124">id</span></span>|<span data-ttu-id="06b78-125">String</span><span class="sxs-lookup"><span data-stu-id="06b78-125">String</span></span>|<span data-ttu-id="06b78-126">目录项的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="06b78-126">The unique identifier for the catalog entry.</span></span> <span data-ttu-id="06b78-127">只读。</span><span class="sxs-lookup"><span data-stu-id="06b78-127">Read-only.</span></span> <span data-ttu-id="06b78-128">继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。</span><span class="sxs-lookup"><span data-stu-id="06b78-128">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|
|<span data-ttu-id="06b78-129">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="06b78-129">releaseDateTime</span></span>|<span data-ttu-id="06b78-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06b78-130">DateTimeOffset</span></span>|<span data-ttu-id="06b78-131">内容的发布日期。</span><span class="sxs-lookup"><span data-stu-id="06b78-131">The release date for the content.</span></span> <span data-ttu-id="06b78-132">只读。</span><span class="sxs-lookup"><span data-stu-id="06b78-132">Read-only.</span></span> <span data-ttu-id="06b78-133">继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。</span><span class="sxs-lookup"><span data-stu-id="06b78-133">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|
|<span data-ttu-id="06b78-134">version</span><span class="sxs-lookup"><span data-stu-id="06b78-134">version</span></span>|<span data-ttu-id="06b78-135">String</span><span class="sxs-lookup"><span data-stu-id="06b78-135">String</span></span>|<span data-ttu-id="06b78-136">功能更新的版本。</span><span class="sxs-lookup"><span data-stu-id="06b78-136">The version of the feature update.</span></span> <span data-ttu-id="06b78-137">只读。</span><span class="sxs-lookup"><span data-stu-id="06b78-137">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06b78-138">关系</span><span class="sxs-lookup"><span data-stu-id="06b78-138">Relationships</span></span>
<span data-ttu-id="06b78-139">无。</span><span class="sxs-lookup"><span data-stu-id="06b78-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="06b78-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06b78-140">JSON representation</span></span>
<span data-ttu-id="06b78-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06b78-141">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
  "baseType": "microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)",
  "version": "String"
}
```

