---
title: securityBaselineStateSummary 资源类型
description: 帐户安全基准的安全基准合规性状态摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 94883b3cf9ece434a080f8896a06a81af81affc1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060921"
---
# <a name="securitybaselinestatesummary-resource-type"></a><span data-ttu-id="5f018-103">securityBaselineStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f018-103">securityBaselineStateSummary resource type</span></span>

<span data-ttu-id="5f018-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f018-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f018-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5f018-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f018-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5f018-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f018-107">帐户安全基准的安全基准合规性状态摘要。</span><span class="sxs-lookup"><span data-stu-id="5f018-107">The security baseline compliance state summary for the security baseline of the account.</span></span>

## <a name="methods"></a><span data-ttu-id="5f018-108">方法</span><span class="sxs-lookup"><span data-stu-id="5f018-108">Methods</span></span>
|<span data-ttu-id="5f018-109">方法</span><span class="sxs-lookup"><span data-stu-id="5f018-109">Method</span></span>|<span data-ttu-id="5f018-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5f018-110">Return Type</span></span>|<span data-ttu-id="5f018-111">说明</span><span class="sxs-lookup"><span data-stu-id="5f018-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5f018-112">获取 securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="5f018-112">Get securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-get.md)|[<span data-ttu-id="5f018-113">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="5f018-113">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="5f018-114">读取 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5f018-114">Read properties and relationships of the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|
|[<span data-ttu-id="5f018-115">更新 securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="5f018-115">Update securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-update.md)|[<span data-ttu-id="5f018-116">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="5f018-116">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="5f018-117">更新 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5f018-117">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5f018-118">属性</span><span class="sxs-lookup"><span data-stu-id="5f018-118">Properties</span></span>
|<span data-ttu-id="5f018-119">属性</span><span class="sxs-lookup"><span data-stu-id="5f018-119">Property</span></span>|<span data-ttu-id="5f018-120">类型</span><span class="sxs-lookup"><span data-stu-id="5f018-120">Type</span></span>|<span data-ttu-id="5f018-121">说明</span><span class="sxs-lookup"><span data-stu-id="5f018-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f018-122">id</span><span class="sxs-lookup"><span data-stu-id="5f018-122">id</span></span>|<span data-ttu-id="5f018-123">String</span><span class="sxs-lookup"><span data-stu-id="5f018-123">String</span></span>|<span data-ttu-id="5f018-124">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5f018-124">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="5f018-125">secureCount</span><span class="sxs-lookup"><span data-stu-id="5f018-125">secureCount</span></span>|<span data-ttu-id="5f018-126">Int32</span><span class="sxs-lookup"><span data-stu-id="5f018-126">Int32</span></span>|<span data-ttu-id="5f018-127">安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="5f018-127">Number of secure devices</span></span>|
|<span data-ttu-id="5f018-128">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="5f018-128">notSecureCount</span></span>|<span data-ttu-id="5f018-129">Int32</span><span class="sxs-lookup"><span data-stu-id="5f018-129">Int32</span></span>|<span data-ttu-id="5f018-130">不安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="5f018-130">Number of not secure devices</span></span>|
|<span data-ttu-id="5f018-131">unknownCount</span><span class="sxs-lookup"><span data-stu-id="5f018-131">unknownCount</span></span>|<span data-ttu-id="5f018-132">Int32</span><span class="sxs-lookup"><span data-stu-id="5f018-132">Int32</span></span>|<span data-ttu-id="5f018-133">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="5f018-133">Number of unknown devices</span></span>|
|<span data-ttu-id="5f018-134">errorCount</span><span class="sxs-lookup"><span data-stu-id="5f018-134">errorCount</span></span>|<span data-ttu-id="5f018-135">Int32</span><span class="sxs-lookup"><span data-stu-id="5f018-135">Int32</span></span>|<span data-ttu-id="5f018-136">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="5f018-136">Number of error devices</span></span>|
|<span data-ttu-id="5f018-137">conflictCount</span><span class="sxs-lookup"><span data-stu-id="5f018-137">conflictCount</span></span>|<span data-ttu-id="5f018-138">Int32</span><span class="sxs-lookup"><span data-stu-id="5f018-138">Int32</span></span>|<span data-ttu-id="5f018-139">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="5f018-139">Number of conflict devices</span></span>|
|<span data-ttu-id="5f018-140">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="5f018-140">notApplicableCount</span></span>|<span data-ttu-id="5f018-141">Int32</span><span class="sxs-lookup"><span data-stu-id="5f018-141">Int32</span></span>|<span data-ttu-id="5f018-142">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="5f018-142">Number of not applicable devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f018-143">关系</span><span class="sxs-lookup"><span data-stu-id="5f018-143">Relationships</span></span>
<span data-ttu-id="5f018-144">无</span><span class="sxs-lookup"><span data-stu-id="5f018-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f018-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f018-145">JSON Representation</span></span>
<span data-ttu-id="5f018-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f018-146">Here is a JSON representation of the resource.</span></span>
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






