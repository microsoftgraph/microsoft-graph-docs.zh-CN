---
title: securityBaselineStateSummary 资源类型
description: 帐户安全基准的安全基准合规性状态摘要。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 28a479ec175a939d65d4d11c963df575a28e59d1
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523957"
---
# <a name="securitybaselinestatesummary-resource-type"></a><span data-ttu-id="303d0-103">securityBaselineStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="303d0-103">securityBaselineStateSummary resource type</span></span>

> <span data-ttu-id="303d0-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="303d0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="303d0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="303d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="303d0-106">帐户安全基准的安全基准合规性状态摘要。</span><span class="sxs-lookup"><span data-stu-id="303d0-106">The security baseline compliance state summary for the security baseline of the account.</span></span>

## <a name="methods"></a><span data-ttu-id="303d0-107">方法</span><span class="sxs-lookup"><span data-stu-id="303d0-107">Methods</span></span>
|<span data-ttu-id="303d0-108">方法</span><span class="sxs-lookup"><span data-stu-id="303d0-108">Method</span></span>|<span data-ttu-id="303d0-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="303d0-109">Return Type</span></span>|<span data-ttu-id="303d0-110">说明</span><span class="sxs-lookup"><span data-stu-id="303d0-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="303d0-111">获取 securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="303d0-111">Get securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-get.md)|[<span data-ttu-id="303d0-112">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="303d0-112">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="303d0-113">读取[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="303d0-113">Read properties and relationships of the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|
|[<span data-ttu-id="303d0-114">更新 securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="303d0-114">Update securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-update.md)|[<span data-ttu-id="303d0-115">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="303d0-115">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="303d0-116">更新[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="303d0-116">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="303d0-117">属性</span><span class="sxs-lookup"><span data-stu-id="303d0-117">Properties</span></span>
|<span data-ttu-id="303d0-118">属性</span><span class="sxs-lookup"><span data-stu-id="303d0-118">Property</span></span>|<span data-ttu-id="303d0-119">类型</span><span class="sxs-lookup"><span data-stu-id="303d0-119">Type</span></span>|<span data-ttu-id="303d0-120">说明</span><span class="sxs-lookup"><span data-stu-id="303d0-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="303d0-121">id</span><span class="sxs-lookup"><span data-stu-id="303d0-121">id</span></span>|<span data-ttu-id="303d0-122">String</span><span class="sxs-lookup"><span data-stu-id="303d0-122">String</span></span>|<span data-ttu-id="303d0-123">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="303d0-123">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="303d0-124">secureCount</span><span class="sxs-lookup"><span data-stu-id="303d0-124">secureCount</span></span>|<span data-ttu-id="303d0-125">Int32</span><span class="sxs-lookup"><span data-stu-id="303d0-125">Int32</span></span>|<span data-ttu-id="303d0-126">安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="303d0-126">Number of secure devices</span></span>|
|<span data-ttu-id="303d0-127">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="303d0-127">notSecureCount</span></span>|<span data-ttu-id="303d0-128">Int32</span><span class="sxs-lookup"><span data-stu-id="303d0-128">Int32</span></span>|<span data-ttu-id="303d0-129">不安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="303d0-129">Number of not secure devices</span></span>|
|<span data-ttu-id="303d0-130">unknownCount</span><span class="sxs-lookup"><span data-stu-id="303d0-130">unknownCount</span></span>|<span data-ttu-id="303d0-131">Int32</span><span class="sxs-lookup"><span data-stu-id="303d0-131">Int32</span></span>|<span data-ttu-id="303d0-132">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="303d0-132">Number of unknown devices</span></span>|
|<span data-ttu-id="303d0-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="303d0-133">errorCount</span></span>|<span data-ttu-id="303d0-134">Int32</span><span class="sxs-lookup"><span data-stu-id="303d0-134">Int32</span></span>|<span data-ttu-id="303d0-135">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="303d0-135">Number of error devices</span></span>|
|<span data-ttu-id="303d0-136">conflictCount</span><span class="sxs-lookup"><span data-stu-id="303d0-136">conflictCount</span></span>|<span data-ttu-id="303d0-137">Int32</span><span class="sxs-lookup"><span data-stu-id="303d0-137">Int32</span></span>|<span data-ttu-id="303d0-138">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="303d0-138">Number of conflict devices</span></span>|
|<span data-ttu-id="303d0-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="303d0-139">notApplicableCount</span></span>|<span data-ttu-id="303d0-140">Int32</span><span class="sxs-lookup"><span data-stu-id="303d0-140">Int32</span></span>|<span data-ttu-id="303d0-141">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="303d0-141">Number of not applicable devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="303d0-142">关系</span><span class="sxs-lookup"><span data-stu-id="303d0-142">Relationships</span></span>
<span data-ttu-id="303d0-143">无</span><span class="sxs-lookup"><span data-stu-id="303d0-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="303d0-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="303d0-144">JSON Representation</span></span>
<span data-ttu-id="303d0-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="303d0-145">Here is a JSON representation of the resource.</span></span>
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







