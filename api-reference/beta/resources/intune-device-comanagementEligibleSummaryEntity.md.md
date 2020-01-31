---
title: comanagementEligibleSummaryEntity 资源类型
description: comanagementEligibleSummaryEntity 资源类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 80c2afff56d845097990ef927a743678a248c9fd
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636579"
---
# <a name="comanagementeligiblesummaryentity-resource-type"></a><span data-ttu-id="375e8-103">comanagementEligibleSummaryEntity 资源类型</span><span class="sxs-lookup"><span data-stu-id="375e8-103">comanagementEligibleSummaryEntity resource type</span></span>

> <span data-ttu-id="375e8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="375e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="375e8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="375e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="375e8-106">给定设备的托管设备移动应用配置状态。</span><span class="sxs-lookup"><span data-stu-id="375e8-106">Managed Device Mobile App Configuration State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="375e8-107">方法</span><span class="sxs-lookup"><span data-stu-id="375e8-107">Methods</span></span>
|<span data-ttu-id="375e8-108">方法</span><span class="sxs-lookup"><span data-stu-id="375e8-108">Method</span></span>|<span data-ttu-id="375e8-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="375e8-109">Return Type</span></span>|<span data-ttu-id="375e8-110">说明</span><span class="sxs-lookup"><span data-stu-id="375e8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="375e8-111">列出 comanagementEligibleSummaryEntity</span><span class="sxs-lookup"><span data-stu-id="375e8-111">List comanagementEligibleSummaryEntity</span></span>](../api/intune-device-comanagementEligibleSummaryEntity-list.md)|<span data-ttu-id="375e8-112">comanagementEligibleSummaryEntity 集合</span><span class="sxs-lookup"><span data-stu-id="375e8-112">comanagementEligibleSummaryEntity collection</span></span>|<span data-ttu-id="375e8-113">列出 comanagementEligibleSummaryEntity 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="375e8-113">List properties and relationships of the comanagementEligibleSummaryEntity objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="375e8-114">属性</span><span class="sxs-lookup"><span data-stu-id="375e8-114">Properties</span></span>
|<span data-ttu-id="375e8-115">属性</span><span class="sxs-lookup"><span data-stu-id="375e8-115">Property</span></span>|<span data-ttu-id="375e8-116">类型</span><span class="sxs-lookup"><span data-stu-id="375e8-116">Type</span></span>|<span data-ttu-id="375e8-117">说明</span><span class="sxs-lookup"><span data-stu-id="375e8-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="375e8-118">id</span><span class="sxs-lookup"><span data-stu-id="375e8-118">id</span></span>|<span data-ttu-id="375e8-119">字符串</span><span class="sxs-lookup"><span data-stu-id="375e8-119">String</span></span>|<span data-ttu-id="375e8-120">EligibleDeviceSummaryEntity 的唯一 Id</span><span class="sxs-lookup"><span data-stu-id="375e8-120">Unique Id of the EligibleDeviceSummaryEntity</span></span>|
|<span data-ttu-id="375e8-121">coManagedCount</span><span class="sxs-lookup"><span data-stu-id="375e8-121">coManagedCount</span></span>|<span data-ttu-id="375e8-122">Int32</span><span class="sxs-lookup"><span data-stu-id="375e8-122">Int32</span></span>|<span data-ttu-id="375e8-123">已 CoManaged 的设备计数</span><span class="sxs-lookup"><span data-stu-id="375e8-123">Count of devices already CoManaged</span></span>|
|<span data-ttu-id="375e8-124">eligibleCount</span><span class="sxs-lookup"><span data-stu-id="375e8-124">eligibleCount</span></span>|<span data-ttu-id="375e8-125">Int32</span><span class="sxs-lookup"><span data-stu-id="375e8-125">Int32</span></span>|<span data-ttu-id="375e8-126">完全符合条件的设备计数 CoManagement</span><span class="sxs-lookup"><span data-stu-id="375e8-126">Count of devices fully eligible for CoManagement</span></span>|
|<span data-ttu-id="375e8-127">eligibleButNotAadJoinedCount</span><span class="sxs-lookup"><span data-stu-id="375e8-127">eligibleButNotAadJoinedCount</span></span>|<span data-ttu-id="375e8-128">Int32</span><span class="sxs-lookup"><span data-stu-id="375e8-128">Int32</span></span>|<span data-ttu-id="375e8-129">符合 CoManagement 但尚未加入 Azure Active Directory 的设备的计数</span><span class="sxs-lookup"><span data-stu-id="375e8-129">Count of devices eligible for CoManagement but not yet joined to Azure Active Directory</span></span>|
|<span data-ttu-id="375e8-130">needsOSUpdateCount</span><span class="sxs-lookup"><span data-stu-id="375e8-130">needsOSUpdateCount</span></span>|<span data-ttu-id="375e8-131">Int32</span><span class="sxs-lookup"><span data-stu-id="375e8-131">Int32</span></span>|<span data-ttu-id="375e8-132">在 OS 更新后符合 CoManagement 条件的设备的计数</span><span class="sxs-lookup"><span data-stu-id="375e8-132">Count of devices that will be eligible for CoManagement after an OS update</span></span>|

## <a name="relationships"></a><span data-ttu-id="375e8-133">关系</span><span class="sxs-lookup"><span data-stu-id="375e8-133">Relationships</span></span>
<span data-ttu-id="375e8-134">无</span><span class="sxs-lookup"><span data-stu-id="375e8-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="375e8-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="375e8-135">JSON Representation</span></span>
<span data-ttu-id="375e8-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="375e8-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.comanagementEligibleSummaryEntity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleSummaryEntity",
  "id": "String (identifier)",
  "coManagedCount": 1024,
  "eligibleCount": 1024,
  "eligibleButNotAadJoinedCount": 1024,
  "needsOSUpdateCount": 1024
}
```

