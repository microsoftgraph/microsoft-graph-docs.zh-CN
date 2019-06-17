---
title: securityBaselineCategoryStateSummary 资源类型
description: 帐户安全基准的每个类别合规性状态摘要的安全基准。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00735cb51952ec9cc8104a1d2f142d74cb773e05
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983447"
---
# <a name="securitybaselinecategorystatesummary-resource-type"></a><span data-ttu-id="4b75f-103">securityBaselineCategoryStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b75f-103">securityBaselineCategoryStateSummary resource type</span></span>

> <span data-ttu-id="4b75f-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4b75f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b75f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4b75f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b75f-106">帐户安全基准的每个类别合规性状态摘要的安全基准。</span><span class="sxs-lookup"><span data-stu-id="4b75f-106">The security baseline per category compliance state summary for the security baseline of the account.</span></span>


<span data-ttu-id="4b75f-107">继承自[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="4b75f-107">Inherits from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>

## <a name="methods"></a><span data-ttu-id="4b75f-108">方法</span><span class="sxs-lookup"><span data-stu-id="4b75f-108">Methods</span></span>
|<span data-ttu-id="4b75f-109">方法</span><span class="sxs-lookup"><span data-stu-id="4b75f-109">Method</span></span>|<span data-ttu-id="4b75f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="4b75f-110">Return Type</span></span>|<span data-ttu-id="4b75f-111">说明</span><span class="sxs-lookup"><span data-stu-id="4b75f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4b75f-112">列出 securityBaselineCategoryStateSummaries</span><span class="sxs-lookup"><span data-stu-id="4b75f-112">List securityBaselineCategoryStateSummaries</span></span>](../api/intune-deviceintent-securitybaselinecategorystatesummary-list.md)|<span data-ttu-id="4b75f-113">[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)集合</span><span class="sxs-lookup"><span data-stu-id="4b75f-113">[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) collection</span></span>|<span data-ttu-id="4b75f-114">列出[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4b75f-114">List properties and relationships of the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) objects.</span></span>|
|[<span data-ttu-id="4b75f-115">获取 securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="4b75f-115">Get securityBaselineCategoryStateSummary</span></span>](../api/intune-deviceintent-securitybaselinecategorystatesummary-get.md)|[<span data-ttu-id="4b75f-116">securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="4b75f-116">securityBaselineCategoryStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|<span data-ttu-id="4b75f-117">读取[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4b75f-117">Read properties and relationships of the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>|
|[<span data-ttu-id="4b75f-118">创建 securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="4b75f-118">Create securityBaselineCategoryStateSummary</span></span>](../api/intune-deviceintent-securitybaselinecategorystatesummary-create.md)|[<span data-ttu-id="4b75f-119">securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="4b75f-119">securityBaselineCategoryStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|<span data-ttu-id="4b75f-120">创建新的[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4b75f-120">Create a new [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>|
|[<span data-ttu-id="4b75f-121">删除 securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="4b75f-121">Delete securityBaselineCategoryStateSummary</span></span>](../api/intune-deviceintent-securitybaselinecategorystatesummary-delete.md)|<span data-ttu-id="4b75f-122">无</span><span class="sxs-lookup"><span data-stu-id="4b75f-122">None</span></span>|<span data-ttu-id="4b75f-123">删除[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="4b75f-123">Deletes a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).</span></span>|
|[<span data-ttu-id="4b75f-124">更新 securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="4b75f-124">Update securityBaselineCategoryStateSummary</span></span>](../api/intune-deviceintent-securitybaselinecategorystatesummary-update.md)|[<span data-ttu-id="4b75f-125">securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="4b75f-125">securityBaselineCategoryStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|<span data-ttu-id="4b75f-126">更新[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4b75f-126">Update the properties of a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4b75f-127">属性</span><span class="sxs-lookup"><span data-stu-id="4b75f-127">Properties</span></span>
|<span data-ttu-id="4b75f-128">属性</span><span class="sxs-lookup"><span data-stu-id="4b75f-128">Property</span></span>|<span data-ttu-id="4b75f-129">类型</span><span class="sxs-lookup"><span data-stu-id="4b75f-129">Type</span></span>|<span data-ttu-id="4b75f-130">说明</span><span class="sxs-lookup"><span data-stu-id="4b75f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b75f-131">id</span><span class="sxs-lookup"><span data-stu-id="4b75f-131">id</span></span>|<span data-ttu-id="4b75f-132">String</span><span class="sxs-lookup"><span data-stu-id="4b75f-132">String</span></span>|<span data-ttu-id="4b75f-133">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4b75f-133">Unique identifier of the entity.</span></span> <span data-ttu-id="4b75f-134">继承自[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="4b75f-134">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="4b75f-135">secureCount</span><span class="sxs-lookup"><span data-stu-id="4b75f-135">secureCount</span></span>|<span data-ttu-id="4b75f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4b75f-136">Int32</span></span>|<span data-ttu-id="4b75f-137">继承自[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)的安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="4b75f-137">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="4b75f-138">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="4b75f-138">notSecureCount</span></span>|<span data-ttu-id="4b75f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="4b75f-139">Int32</span></span>|<span data-ttu-id="4b75f-140">从[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)继承的不安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="4b75f-140">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="4b75f-141">unknownCount</span><span class="sxs-lookup"><span data-stu-id="4b75f-141">unknownCount</span></span>|<span data-ttu-id="4b75f-142">Int32</span><span class="sxs-lookup"><span data-stu-id="4b75f-142">Int32</span></span>|<span data-ttu-id="4b75f-143">从[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)继承的未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="4b75f-143">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="4b75f-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="4b75f-144">errorCount</span></span>|<span data-ttu-id="4b75f-145">Int32</span><span class="sxs-lookup"><span data-stu-id="4b75f-145">Int32</span></span>|<span data-ttu-id="4b75f-146">继承自[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)的错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="4b75f-146">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="4b75f-147">conflictCount</span><span class="sxs-lookup"><span data-stu-id="4b75f-147">conflictCount</span></span>|<span data-ttu-id="4b75f-148">Int32</span><span class="sxs-lookup"><span data-stu-id="4b75f-148">Int32</span></span>|<span data-ttu-id="4b75f-149">继承自[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)的冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="4b75f-149">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="4b75f-150">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="4b75f-150">notApplicableCount</span></span>|<span data-ttu-id="4b75f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="4b75f-151">Int32</span></span>|<span data-ttu-id="4b75f-152">从[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)继承的不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="4b75f-152">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="4b75f-153">displayName</span><span class="sxs-lookup"><span data-stu-id="4b75f-153">displayName</span></span>|<span data-ttu-id="4b75f-154">String</span><span class="sxs-lookup"><span data-stu-id="4b75f-154">String</span></span>|<span data-ttu-id="4b75f-155">类别名称</span><span class="sxs-lookup"><span data-stu-id="4b75f-155">The category name</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b75f-156">关系</span><span class="sxs-lookup"><span data-stu-id="4b75f-156">Relationships</span></span>
<span data-ttu-id="4b75f-157">无</span><span class="sxs-lookup"><span data-stu-id="4b75f-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b75f-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b75f-158">JSON Representation</span></span>
<span data-ttu-id="4b75f-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b75f-159">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineCategoryStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "id": "String (identifier)",
  "secureCount": 1024,
  "notSecureCount": 1024,
  "unknownCount": 1024,
  "errorCount": 1024,
  "conflictCount": 1024,
  "notApplicableCount": 1024,
  "displayName": "String"
}
```





