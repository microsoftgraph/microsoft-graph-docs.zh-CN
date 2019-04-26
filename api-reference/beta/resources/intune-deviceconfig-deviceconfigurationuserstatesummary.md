---
title: deviceConfigurationUserStateSummary 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d6d79f4e36ae66aa871f08eaa69aaa2bcf39a76
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553860"
---
# <a name="deviceconfigurationuserstatesummary-resource-type"></a><span data-ttu-id="c8002-103">deviceConfigurationUserStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="c8002-103">deviceConfigurationUserStateSummary resource type</span></span>

> <span data-ttu-id="c8002-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c8002-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8002-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c8002-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8002-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c8002-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="c8002-107">方法</span><span class="sxs-lookup"><span data-stu-id="c8002-107">Methods</span></span>
|<span data-ttu-id="c8002-108">方法</span><span class="sxs-lookup"><span data-stu-id="c8002-108">Method</span></span>|<span data-ttu-id="c8002-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c8002-109">Return Type</span></span>|<span data-ttu-id="c8002-110">说明</span><span class="sxs-lookup"><span data-stu-id="c8002-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c8002-111">获取 deviceConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="c8002-111">Get deviceConfigurationUserStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationuserstatesummary-get.md)|[<span data-ttu-id="c8002-112">deviceConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="c8002-112">deviceConfigurationUserStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|<span data-ttu-id="c8002-113">读取[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c8002-113">Read properties and relationships of the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>|
|[<span data-ttu-id="c8002-114">更新 deviceConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="c8002-114">Update deviceConfigurationUserStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationuserstatesummary-update.md)|[<span data-ttu-id="c8002-115">deviceConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="c8002-115">deviceConfigurationUserStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|<span data-ttu-id="c8002-116">更新[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c8002-116">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c8002-117">属性</span><span class="sxs-lookup"><span data-stu-id="c8002-117">Properties</span></span>
|<span data-ttu-id="c8002-118">属性</span><span class="sxs-lookup"><span data-stu-id="c8002-118">Property</span></span>|<span data-ttu-id="c8002-119">类型</span><span class="sxs-lookup"><span data-stu-id="c8002-119">Type</span></span>|<span data-ttu-id="c8002-120">说明</span><span class="sxs-lookup"><span data-stu-id="c8002-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8002-121">id</span><span class="sxs-lookup"><span data-stu-id="c8002-121">id</span></span>|<span data-ttu-id="c8002-122">String</span><span class="sxs-lookup"><span data-stu-id="c8002-122">String</span></span>|<span data-ttu-id="c8002-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c8002-123">Key of the entity.</span></span>|
|<span data-ttu-id="c8002-124">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="c8002-124">unknownUserCount</span></span>|<span data-ttu-id="c8002-125">Int32</span><span class="sxs-lookup"><span data-stu-id="c8002-125">Int32</span></span>|<span data-ttu-id="c8002-126">未知用户的数量</span><span class="sxs-lookup"><span data-stu-id="c8002-126">Number of unknown users</span></span>|
|<span data-ttu-id="c8002-127">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="c8002-127">notApplicableUserCount</span></span>|<span data-ttu-id="c8002-128">Int32</span><span class="sxs-lookup"><span data-stu-id="c8002-128">Int32</span></span>|<span data-ttu-id="c8002-129">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="c8002-129">Number of not applicable users</span></span>|
|<span data-ttu-id="c8002-130">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="c8002-130">compliantUserCount</span></span>|<span data-ttu-id="c8002-131">Int32</span><span class="sxs-lookup"><span data-stu-id="c8002-131">Int32</span></span>|<span data-ttu-id="c8002-132">合规用户数</span><span class="sxs-lookup"><span data-stu-id="c8002-132">Number of compliant users</span></span>|
|<span data-ttu-id="c8002-133">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="c8002-133">remediatedUserCount</span></span>|<span data-ttu-id="c8002-134">Int32</span><span class="sxs-lookup"><span data-stu-id="c8002-134">Int32</span></span>|<span data-ttu-id="c8002-135">已修正用户的数量</span><span class="sxs-lookup"><span data-stu-id="c8002-135">Number of remediated users</span></span>|
|<span data-ttu-id="c8002-136">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="c8002-136">nonCompliantUserCount</span></span>|<span data-ttu-id="c8002-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c8002-137">Int32</span></span>|<span data-ttu-id="c8002-138">不符合的用户数</span><span class="sxs-lookup"><span data-stu-id="c8002-138">Number of NonCompliant users</span></span>|
|<span data-ttu-id="c8002-139">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="c8002-139">errorUserCount</span></span>|<span data-ttu-id="c8002-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c8002-140">Int32</span></span>|<span data-ttu-id="c8002-141">错误用户数</span><span class="sxs-lookup"><span data-stu-id="c8002-141">Number of error users</span></span>|
|<span data-ttu-id="c8002-142">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="c8002-142">conflictUserCount</span></span>|<span data-ttu-id="c8002-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c8002-143">Int32</span></span>|<span data-ttu-id="c8002-144">冲突用户数</span><span class="sxs-lookup"><span data-stu-id="c8002-144">Number of conflict users</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8002-145">关系</span><span class="sxs-lookup"><span data-stu-id="c8002-145">Relationships</span></span>
<span data-ttu-id="c8002-146">无</span><span class="sxs-lookup"><span data-stu-id="c8002-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8002-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c8002-147">JSON Representation</span></span>
<span data-ttu-id="c8002-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8002-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationUserStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "id": "String (identifier)",
  "unknownUserCount": 1024,
  "notApplicableUserCount": 1024,
  "compliantUserCount": 1024,
  "remediatedUserCount": 1024,
  "nonCompliantUserCount": 1024,
  "errorUserCount": 1024,
  "conflictUserCount": 1024
}
```





