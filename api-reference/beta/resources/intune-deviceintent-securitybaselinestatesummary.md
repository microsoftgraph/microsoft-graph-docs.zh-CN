---
title: securityBaselineStateSummary 资源类型
description: 帐户安全基准的安全基准合规性状态摘要。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7b4a9380e528561477f3b55704f32042e623d314
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785187"
---
# <a name="securitybaselinestatesummary-resource-type"></a><span data-ttu-id="55607-103">securityBaselineStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="55607-103">securityBaselineStateSummary resource type</span></span>

> <span data-ttu-id="55607-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="55607-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55607-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="55607-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55607-106">帐户安全基准的安全基准合规性状态摘要。</span><span class="sxs-lookup"><span data-stu-id="55607-106">The security baseline compliance state summary for the security baseline of the account.</span></span>

## <a name="methods"></a><span data-ttu-id="55607-107">方法</span><span class="sxs-lookup"><span data-stu-id="55607-107">Methods</span></span>
|<span data-ttu-id="55607-108">方法</span><span class="sxs-lookup"><span data-stu-id="55607-108">Method</span></span>|<span data-ttu-id="55607-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="55607-109">Return Type</span></span>|<span data-ttu-id="55607-110">说明</span><span class="sxs-lookup"><span data-stu-id="55607-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="55607-111">获取 securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="55607-111">Get securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-get.md)|[<span data-ttu-id="55607-112">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="55607-112">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="55607-113">读取[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="55607-113">Read properties and relationships of the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|
|[<span data-ttu-id="55607-114">更新 securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="55607-114">Update securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-update.md)|[<span data-ttu-id="55607-115">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="55607-115">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="55607-116">更新[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="55607-116">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="55607-117">属性</span><span class="sxs-lookup"><span data-stu-id="55607-117">Properties</span></span>
|<span data-ttu-id="55607-118">属性</span><span class="sxs-lookup"><span data-stu-id="55607-118">Property</span></span>|<span data-ttu-id="55607-119">类型</span><span class="sxs-lookup"><span data-stu-id="55607-119">Type</span></span>|<span data-ttu-id="55607-120">说明</span><span class="sxs-lookup"><span data-stu-id="55607-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55607-121">id</span><span class="sxs-lookup"><span data-stu-id="55607-121">id</span></span>|<span data-ttu-id="55607-122">String</span><span class="sxs-lookup"><span data-stu-id="55607-122">String</span></span>|<span data-ttu-id="55607-123">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="55607-123">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="55607-124">secureCount</span><span class="sxs-lookup"><span data-stu-id="55607-124">secureCount</span></span>|<span data-ttu-id="55607-125">Int32</span><span class="sxs-lookup"><span data-stu-id="55607-125">Int32</span></span>|<span data-ttu-id="55607-126">安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="55607-126">Number of secure devices</span></span>|
|<span data-ttu-id="55607-127">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="55607-127">notSecureCount</span></span>|<span data-ttu-id="55607-128">Int32</span><span class="sxs-lookup"><span data-stu-id="55607-128">Int32</span></span>|<span data-ttu-id="55607-129">不安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="55607-129">Number of not secure devices</span></span>|
|<span data-ttu-id="55607-130">unknownCount</span><span class="sxs-lookup"><span data-stu-id="55607-130">unknownCount</span></span>|<span data-ttu-id="55607-131">Int32</span><span class="sxs-lookup"><span data-stu-id="55607-131">Int32</span></span>|<span data-ttu-id="55607-132">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="55607-132">Number of unknown devices</span></span>|
|<span data-ttu-id="55607-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="55607-133">errorCount</span></span>|<span data-ttu-id="55607-134">Int32</span><span class="sxs-lookup"><span data-stu-id="55607-134">Int32</span></span>|<span data-ttu-id="55607-135">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="55607-135">Number of error devices</span></span>|
|<span data-ttu-id="55607-136">conflictCount</span><span class="sxs-lookup"><span data-stu-id="55607-136">conflictCount</span></span>|<span data-ttu-id="55607-137">Int32</span><span class="sxs-lookup"><span data-stu-id="55607-137">Int32</span></span>|<span data-ttu-id="55607-138">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="55607-138">Number of conflict devices</span></span>|
|<span data-ttu-id="55607-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="55607-139">notApplicableCount</span></span>|<span data-ttu-id="55607-140">Int32</span><span class="sxs-lookup"><span data-stu-id="55607-140">Int32</span></span>|<span data-ttu-id="55607-141">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="55607-141">Number of not applicable devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="55607-142">关系</span><span class="sxs-lookup"><span data-stu-id="55607-142">Relationships</span></span>
<span data-ttu-id="55607-143">无</span><span class="sxs-lookup"><span data-stu-id="55607-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55607-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55607-144">JSON Representation</span></span>
<span data-ttu-id="55607-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55607-145">Here is a JSON representation of the resource.</span></span>
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



