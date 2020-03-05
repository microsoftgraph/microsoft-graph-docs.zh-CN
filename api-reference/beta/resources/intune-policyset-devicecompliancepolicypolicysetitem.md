---
title: deviceCompliancePolicyPolicySetItem 资源类型
description: 包含用于设备合规性策略 PolicySetItem 的属性的类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 55019ee566c9f11b1a1c8edeaebc74b1abc9e914
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527647"
---
# <a name="devicecompliancepolicypolicysetitem-resource-type"></a><span data-ttu-id="13e77-103">deviceCompliancePolicyPolicySetItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="13e77-103">deviceCompliancePolicyPolicySetItem resource type</span></span>

<span data-ttu-id="13e77-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="13e77-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13e77-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="13e77-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13e77-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13e77-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13e77-107">包含用于设备合规性策略 PolicySetItem 的属性的类。</span><span class="sxs-lookup"><span data-stu-id="13e77-107">A class containing the properties used for device compliance policy PolicySetItem.</span></span>


<span data-ttu-id="13e77-108">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="13e77-108">Inherits from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>

## <a name="methods"></a><span data-ttu-id="13e77-109">方法</span><span class="sxs-lookup"><span data-stu-id="13e77-109">Methods</span></span>
|<span data-ttu-id="13e77-110">方法</span><span class="sxs-lookup"><span data-stu-id="13e77-110">Method</span></span>|<span data-ttu-id="13e77-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="13e77-111">Return Type</span></span>|<span data-ttu-id="13e77-112">说明</span><span class="sxs-lookup"><span data-stu-id="13e77-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="13e77-113">列出 deviceCompliancePolicyPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="13e77-113">List deviceCompliancePolicyPolicySetItems</span></span>](../api/intune-policyset-devicecompliancepolicypolicysetitem-list.md)|<span data-ttu-id="13e77-114">[deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="13e77-114">[deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) collection</span></span>|<span data-ttu-id="13e77-115">列出[deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="13e77-115">List properties and relationships of the [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) objects.</span></span>|
|[<span data-ttu-id="13e77-116">获取 deviceCompliancePolicyPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="13e77-116">Get deviceCompliancePolicyPolicySetItem</span></span>](../api/intune-policyset-devicecompliancepolicypolicysetitem-get.md)|[<span data-ttu-id="13e77-117">deviceCompliancePolicyPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="13e77-117">deviceCompliancePolicyPolicySetItem</span></span>](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)|<span data-ttu-id="13e77-118">读取[deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="13e77-118">Read properties and relationships of the [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object.</span></span>|
|[<span data-ttu-id="13e77-119">创建 deviceCompliancePolicyPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="13e77-119">Create deviceCompliancePolicyPolicySetItem</span></span>](../api/intune-policyset-devicecompliancepolicypolicysetitem-create.md)|[<span data-ttu-id="13e77-120">deviceCompliancePolicyPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="13e77-120">deviceCompliancePolicyPolicySetItem</span></span>](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)|<span data-ttu-id="13e77-121">创建新的[deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="13e77-121">Create a new [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object.</span></span>|
|[<span data-ttu-id="13e77-122">删除 deviceCompliancePolicyPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="13e77-122">Delete deviceCompliancePolicyPolicySetItem</span></span>](../api/intune-policyset-devicecompliancepolicypolicysetitem-delete.md)|<span data-ttu-id="13e77-123">无</span><span class="sxs-lookup"><span data-stu-id="13e77-123">None</span></span>|<span data-ttu-id="13e77-124">删除[deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="13e77-124">Deletes a [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md).</span></span>|
|[<span data-ttu-id="13e77-125">更新 deviceCompliancePolicyPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="13e77-125">Update deviceCompliancePolicyPolicySetItem</span></span>](../api/intune-policyset-devicecompliancepolicypolicysetitem-update.md)|[<span data-ttu-id="13e77-126">deviceCompliancePolicyPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="13e77-126">deviceCompliancePolicyPolicySetItem</span></span>](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)|<span data-ttu-id="13e77-127">更新[deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="13e77-127">Update the properties of a [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="13e77-128">属性</span><span class="sxs-lookup"><span data-stu-id="13e77-128">Properties</span></span>
|<span data-ttu-id="13e77-129">属性</span><span class="sxs-lookup"><span data-stu-id="13e77-129">Property</span></span>|<span data-ttu-id="13e77-130">类型</span><span class="sxs-lookup"><span data-stu-id="13e77-130">Type</span></span>|<span data-ttu-id="13e77-131">说明</span><span class="sxs-lookup"><span data-stu-id="13e77-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13e77-132">id</span><span class="sxs-lookup"><span data-stu-id="13e77-132">id</span></span>|<span data-ttu-id="13e77-133">String</span><span class="sxs-lookup"><span data-stu-id="13e77-133">String</span></span>|<span data-ttu-id="13e77-134">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="13e77-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="13e77-135">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="13e77-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="13e77-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13e77-136">createdDateTime</span></span>|<span data-ttu-id="13e77-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13e77-137">DateTimeOffset</span></span>|<span data-ttu-id="13e77-138">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="13e77-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="13e77-139">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="13e77-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="13e77-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13e77-140">lastModifiedDateTime</span></span>|<span data-ttu-id="13e77-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13e77-141">DateTimeOffset</span></span>|<span data-ttu-id="13e77-142">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="13e77-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="13e77-143">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="13e77-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="13e77-144">payloadId</span><span class="sxs-lookup"><span data-stu-id="13e77-144">payloadId</span></span>|<span data-ttu-id="13e77-145">String</span><span class="sxs-lookup"><span data-stu-id="13e77-145">String</span></span>|<span data-ttu-id="13e77-146">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="13e77-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="13e77-147">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="13e77-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="13e77-148">itemType</span><span class="sxs-lookup"><span data-stu-id="13e77-148">itemType</span></span>|<span data-ttu-id="13e77-149">String</span><span class="sxs-lookup"><span data-stu-id="13e77-149">String</span></span>|<span data-ttu-id="13e77-150">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="13e77-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="13e77-151">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="13e77-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="13e77-152">displayName</span><span class="sxs-lookup"><span data-stu-id="13e77-152">displayName</span></span>|<span data-ttu-id="13e77-153">String</span><span class="sxs-lookup"><span data-stu-id="13e77-153">String</span></span>|<span data-ttu-id="13e77-154">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="13e77-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="13e77-155">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="13e77-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="13e77-156">status</span><span class="sxs-lookup"><span data-stu-id="13e77-156">status</span></span>|[<span data-ttu-id="13e77-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="13e77-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="13e77-158">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="13e77-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="13e77-159">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="13e77-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="13e77-160">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="13e77-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="13e77-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="13e77-161">errorCode</span></span>|[<span data-ttu-id="13e77-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="13e77-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="13e77-163">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="13e77-163">Error code if any occured.</span></span> <span data-ttu-id="13e77-164">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="13e77-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="13e77-165">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="13e77-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="13e77-166">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="13e77-166">guidedDeploymentTags</span></span>|<span data-ttu-id="13e77-167">String 集合</span><span class="sxs-lookup"><span data-stu-id="13e77-167">String collection</span></span>|<span data-ttu-id="13e77-168">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)的引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="13e77-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="13e77-169">关系</span><span class="sxs-lookup"><span data-stu-id="13e77-169">Relationships</span></span>
<span data-ttu-id="13e77-170">无</span><span class="sxs-lookup"><span data-stu-id="13e77-170">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13e77-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13e77-171">JSON Representation</span></span>
<span data-ttu-id="13e77-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13e77-172">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyPolicySetItem",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "payloadId": "String",
  "itemType": "String",
  "displayName": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ]
}
```



