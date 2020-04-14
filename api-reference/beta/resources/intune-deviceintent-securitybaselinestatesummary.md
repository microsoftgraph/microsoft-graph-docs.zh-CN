---
title: securityBaselineStateSummary 资源类型
description: 帐户安全基准的安全基准合规性状态摘要。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d5d4fc9c256ca498e1a9e14136397847cf5c1953
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43419670"
---
# <a name="securitybaselinestatesummary-resource-type"></a><span data-ttu-id="b3ff9-103">securityBaselineStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3ff9-103">securityBaselineStateSummary resource type</span></span>

<span data-ttu-id="b3ff9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3ff9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3ff9-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b3ff9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3ff9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b3ff9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3ff9-107">帐户安全基准的安全基准合规性状态摘要。</span><span class="sxs-lookup"><span data-stu-id="b3ff9-107">The security baseline compliance state summary for the security baseline of the account.</span></span>

## <a name="methods"></a><span data-ttu-id="b3ff9-108">方法</span><span class="sxs-lookup"><span data-stu-id="b3ff9-108">Methods</span></span>
|<span data-ttu-id="b3ff9-109">方法</span><span class="sxs-lookup"><span data-stu-id="b3ff9-109">Method</span></span>|<span data-ttu-id="b3ff9-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b3ff9-110">Return Type</span></span>|<span data-ttu-id="b3ff9-111">说明</span><span class="sxs-lookup"><span data-stu-id="b3ff9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b3ff9-112">获取 securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="b3ff9-112">Get securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-get.md)|[<span data-ttu-id="b3ff9-113">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="b3ff9-113">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="b3ff9-114">读取[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b3ff9-114">Read properties and relationships of the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|
|[<span data-ttu-id="b3ff9-115">更新 securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="b3ff9-115">Update securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-update.md)|[<span data-ttu-id="b3ff9-116">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="b3ff9-116">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="b3ff9-117">更新[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b3ff9-117">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b3ff9-118">属性</span><span class="sxs-lookup"><span data-stu-id="b3ff9-118">Properties</span></span>
|<span data-ttu-id="b3ff9-119">属性</span><span class="sxs-lookup"><span data-stu-id="b3ff9-119">Property</span></span>|<span data-ttu-id="b3ff9-120">类型</span><span class="sxs-lookup"><span data-stu-id="b3ff9-120">Type</span></span>|<span data-ttu-id="b3ff9-121">说明</span><span class="sxs-lookup"><span data-stu-id="b3ff9-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3ff9-122">id</span><span class="sxs-lookup"><span data-stu-id="b3ff9-122">id</span></span>|<span data-ttu-id="b3ff9-123">String</span><span class="sxs-lookup"><span data-stu-id="b3ff9-123">String</span></span>|<span data-ttu-id="b3ff9-124">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b3ff9-124">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="b3ff9-125">secureCount</span><span class="sxs-lookup"><span data-stu-id="b3ff9-125">secureCount</span></span>|<span data-ttu-id="b3ff9-126">Int32</span><span class="sxs-lookup"><span data-stu-id="b3ff9-126">Int32</span></span>|<span data-ttu-id="b3ff9-127">安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="b3ff9-127">Number of secure devices</span></span>|
|<span data-ttu-id="b3ff9-128">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="b3ff9-128">notSecureCount</span></span>|<span data-ttu-id="b3ff9-129">Int32</span><span class="sxs-lookup"><span data-stu-id="b3ff9-129">Int32</span></span>|<span data-ttu-id="b3ff9-130">不安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="b3ff9-130">Number of not secure devices</span></span>|
|<span data-ttu-id="b3ff9-131">unknownCount</span><span class="sxs-lookup"><span data-stu-id="b3ff9-131">unknownCount</span></span>|<span data-ttu-id="b3ff9-132">Int32</span><span class="sxs-lookup"><span data-stu-id="b3ff9-132">Int32</span></span>|<span data-ttu-id="b3ff9-133">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="b3ff9-133">Number of unknown devices</span></span>|
|<span data-ttu-id="b3ff9-134">errorCount</span><span class="sxs-lookup"><span data-stu-id="b3ff9-134">errorCount</span></span>|<span data-ttu-id="b3ff9-135">Int32</span><span class="sxs-lookup"><span data-stu-id="b3ff9-135">Int32</span></span>|<span data-ttu-id="b3ff9-136">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="b3ff9-136">Number of error devices</span></span>|
|<span data-ttu-id="b3ff9-137">conflictCount</span><span class="sxs-lookup"><span data-stu-id="b3ff9-137">conflictCount</span></span>|<span data-ttu-id="b3ff9-138">Int32</span><span class="sxs-lookup"><span data-stu-id="b3ff9-138">Int32</span></span>|<span data-ttu-id="b3ff9-139">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="b3ff9-139">Number of conflict devices</span></span>|
|<span data-ttu-id="b3ff9-140">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="b3ff9-140">notApplicableCount</span></span>|<span data-ttu-id="b3ff9-141">Int32</span><span class="sxs-lookup"><span data-stu-id="b3ff9-141">Int32</span></span>|<span data-ttu-id="b3ff9-142">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="b3ff9-142">Number of not applicable devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3ff9-143">关系</span><span class="sxs-lookup"><span data-stu-id="b3ff9-143">Relationships</span></span>
<span data-ttu-id="b3ff9-144">无</span><span class="sxs-lookup"><span data-stu-id="b3ff9-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3ff9-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3ff9-145">JSON Representation</span></span>
<span data-ttu-id="b3ff9-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3ff9-146">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "id": "String (identifier)",
  "secureCount": 1024,
  "notSecureCount": 1024,
  "unknownCount": 1024,
  "errorCount": 1024,
  "conflictCount": 1024,
  "notApplicableCount": 1024
}
```



