---
title: expeditedQualityUpdateReference 资源类型
description: 表示Windows 10质量更新内容以加快更新。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 685f65d8c5661cd4c8308ed712ab3fddedbae51d
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067877"
---
# <a name="expeditedqualityupdatereference-resource-type"></a><span data-ttu-id="ef418-103">expeditedQualityUpdateReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="ef418-103">expeditedQualityUpdateReference resource type</span></span>

<span data-ttu-id="ef418-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="ef418-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef418-105">表示Windows 10质量更新内容以加快更新。</span><span class="sxs-lookup"><span data-stu-id="ef418-105">Represents Windows 10 quality update content to expedite.</span></span>

<span data-ttu-id="ef418-106">在部署中，相同的快速质量更新参考可能会导致设备接收不同的更新修订，但内容被视为与部署中所有设备的上下文等效。</span><span class="sxs-lookup"><span data-stu-id="ef418-106">In a deployment, the same expedited quality update reference could result in devices receiving different update revisions, but the content is considered contextually equivalent for all devices in the deployment.</span></span>

<span data-ttu-id="ef418-107">继承自 [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md)。</span><span class="sxs-lookup"><span data-stu-id="ef418-107">Inherits from [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ef418-108">属性</span><span class="sxs-lookup"><span data-stu-id="ef418-108">Properties</span></span>
|<span data-ttu-id="ef418-109">属性</span><span class="sxs-lookup"><span data-stu-id="ef418-109">Property</span></span>|<span data-ttu-id="ef418-110">类型</span><span class="sxs-lookup"><span data-stu-id="ef418-110">Type</span></span>|<span data-ttu-id="ef418-111">说明</span><span class="sxs-lookup"><span data-stu-id="ef418-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef418-112">classification</span><span class="sxs-lookup"><span data-stu-id="ef418-112">classification</span></span>|<span data-ttu-id="ef418-113">microsoft.graph.windowsUpdates.qualityUpdateClassification</span><span class="sxs-lookup"><span data-stu-id="ef418-113">microsoft.graph.windowsUpdates.qualityUpdateClassification</span></span>|<span data-ttu-id="ef418-114">指定所引用内容的分类。</span><span class="sxs-lookup"><span data-stu-id="ef418-114">Specifies the classification of the referenced content.</span></span> <span data-ttu-id="ef418-115">支持 **qualityUpdateClassification 值的子集**。</span><span class="sxs-lookup"><span data-stu-id="ef418-115">Supports a subset of the values for **qualityUpdateClassification**.</span></span> <span data-ttu-id="ef418-116">默认值为 `security`。</span><span class="sxs-lookup"><span data-stu-id="ef418-116">Default value is `security`.</span></span> <span data-ttu-id="ef418-117">可能的值是 `security` ：。</span><span class="sxs-lookup"><span data-stu-id="ef418-117">Possible values are: `security`.</span></span> <span data-ttu-id="ef418-118">继承自 [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md)。</span><span class="sxs-lookup"><span data-stu-id="ef418-118">Inherited from [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).</span></span>|
|<span data-ttu-id="ef418-119">equivalentContent</span><span class="sxs-lookup"><span data-stu-id="ef418-119">equivalentContent</span></span>|<span data-ttu-id="ef418-120">microsoft.graph.windowsUpdates.equivalentContentOption</span><span class="sxs-lookup"><span data-stu-id="ef418-120">microsoft.graph.windowsUpdates.equivalentContentOption</span></span>|<span data-ttu-id="ef418-121">指定要视为等效内容的其他内容。</span><span class="sxs-lookup"><span data-stu-id="ef418-121">Specifies other content to consider as equivalent.</span></span> <span data-ttu-id="ef418-122">支持 **equivalentContentOption 值的子集**。</span><span class="sxs-lookup"><span data-stu-id="ef418-122">Supports a subset of the values for **equivalentContentOption**.</span></span> <span data-ttu-id="ef418-123">默认值为 `latestSecurity`。</span><span class="sxs-lookup"><span data-stu-id="ef418-123">Default value is `latestSecurity`.</span></span> <span data-ttu-id="ef418-124">可能的值是 `latestSecurity` ：。</span><span class="sxs-lookup"><span data-stu-id="ef418-124">Possible values are: `latestSecurity`.</span></span>|
|<span data-ttu-id="ef418-125">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="ef418-125">releaseDateTime</span></span>|<span data-ttu-id="ef418-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef418-126">DateTimeOffset</span></span>|<span data-ttu-id="ef418-127">按给定分类的发布日期指定质量更新 (即指定日期发布的最后一个) 。</span><span class="sxs-lookup"><span data-stu-id="ef418-127">Specifies a quality update with the given **classification** by its publish date (i.e. the last update published on the specified date).</span></span> <span data-ttu-id="ef418-128">任何具有在 **releaseDateTime** 之前发布的更新的设备都将收到快速的质量更新。</span><span class="sxs-lookup"><span data-stu-id="ef418-128">Any devices with an update that was published prior to the **releaseDateTime** will receive an expedited quality update.</span></span> <span data-ttu-id="ef418-129">继承自 [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md)。</span><span class="sxs-lookup"><span data-stu-id="ef418-129">Inherited from [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef418-130">关系</span><span class="sxs-lookup"><span data-stu-id="ef418-130">Relationships</span></span>
<span data-ttu-id="ef418-131">无。</span><span class="sxs-lookup"><span data-stu-id="ef418-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef418-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ef418-132">JSON representation</span></span>
<span data-ttu-id="ef418-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef418-133">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.expeditedQualityUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.expeditedQualityUpdateReference",
  "classification": "String",
  "releaseDateTime": "String (timestamp)",
  "equivalentContent": "String"
}
```

