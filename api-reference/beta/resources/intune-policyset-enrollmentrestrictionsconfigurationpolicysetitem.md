---
title: enrollmentRestrictionsConfigurationPolicySetItem 资源类型
description: 包含用于注册限制 PolicySetItem 的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9377854bb4c543147938ca785f87f539bca59de1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458438"
---
# <a name="enrollmentrestrictionsconfigurationpolicysetitem-resource-type"></a><span data-ttu-id="009e7-103">enrollmentRestrictionsConfigurationPolicySetItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="009e7-103">enrollmentRestrictionsConfigurationPolicySetItem resource type</span></span>

<span data-ttu-id="009e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="009e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="009e7-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="009e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="009e7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="009e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="009e7-107">包含用于注册限制 PolicySetItem 的属性的类。</span><span class="sxs-lookup"><span data-stu-id="009e7-107">A class containing the properties used for enrollment restriction PolicySetItem.</span></span>


<span data-ttu-id="009e7-108">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="009e7-108">Inherits from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>

## <a name="methods"></a><span data-ttu-id="009e7-109">方法</span><span class="sxs-lookup"><span data-stu-id="009e7-109">Methods</span></span>
|<span data-ttu-id="009e7-110">方法</span><span class="sxs-lookup"><span data-stu-id="009e7-110">Method</span></span>|<span data-ttu-id="009e7-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="009e7-111">Return Type</span></span>|<span data-ttu-id="009e7-112">说明</span><span class="sxs-lookup"><span data-stu-id="009e7-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="009e7-113">列出 enrollmentRestrictionsConfigurationPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="009e7-113">List enrollmentRestrictionsConfigurationPolicySetItems</span></span>](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-list.md)|<span data-ttu-id="009e7-114">[enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="009e7-114">[enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) collection</span></span>|<span data-ttu-id="009e7-115">列出[enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="009e7-115">List properties and relationships of the [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) objects.</span></span>|
|[<span data-ttu-id="009e7-116">获取 enrollmentRestrictionsConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="009e7-116">Get enrollmentRestrictionsConfigurationPolicySetItem</span></span>](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-get.md)|[<span data-ttu-id="009e7-117">enrollmentRestrictionsConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="009e7-117">enrollmentRestrictionsConfigurationPolicySetItem</span></span>](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)|<span data-ttu-id="009e7-118">读取[enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="009e7-118">Read properties and relationships of the [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) object.</span></span>|
|[<span data-ttu-id="009e7-119">创建 enrollmentRestrictionsConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="009e7-119">Create enrollmentRestrictionsConfigurationPolicySetItem</span></span>](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-create.md)|[<span data-ttu-id="009e7-120">enrollmentRestrictionsConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="009e7-120">enrollmentRestrictionsConfigurationPolicySetItem</span></span>](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)|<span data-ttu-id="009e7-121">创建新的[enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="009e7-121">Create a new [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) object.</span></span>|
|[<span data-ttu-id="009e7-122">删除 enrollmentRestrictionsConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="009e7-122">Delete enrollmentRestrictionsConfigurationPolicySetItem</span></span>](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-delete.md)|<span data-ttu-id="009e7-123">无</span><span class="sxs-lookup"><span data-stu-id="009e7-123">None</span></span>|<span data-ttu-id="009e7-124">删除[enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="009e7-124">Deletes a [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md).</span></span>|
|[<span data-ttu-id="009e7-125">更新 enrollmentRestrictionsConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="009e7-125">Update enrollmentRestrictionsConfigurationPolicySetItem</span></span>](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-update.md)|[<span data-ttu-id="009e7-126">enrollmentRestrictionsConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="009e7-126">enrollmentRestrictionsConfigurationPolicySetItem</span></span>](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)|<span data-ttu-id="009e7-127">更新[enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="009e7-127">Update the properties of a [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="009e7-128">属性</span><span class="sxs-lookup"><span data-stu-id="009e7-128">Properties</span></span>
|<span data-ttu-id="009e7-129">属性</span><span class="sxs-lookup"><span data-stu-id="009e7-129">Property</span></span>|<span data-ttu-id="009e7-130">类型</span><span class="sxs-lookup"><span data-stu-id="009e7-130">Type</span></span>|<span data-ttu-id="009e7-131">说明</span><span class="sxs-lookup"><span data-stu-id="009e7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="009e7-132">id</span><span class="sxs-lookup"><span data-stu-id="009e7-132">id</span></span>|<span data-ttu-id="009e7-133">String</span><span class="sxs-lookup"><span data-stu-id="009e7-133">String</span></span>|<span data-ttu-id="009e7-134">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="009e7-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="009e7-135">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="009e7-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="009e7-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="009e7-136">createdDateTime</span></span>|<span data-ttu-id="009e7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="009e7-137">DateTimeOffset</span></span>|<span data-ttu-id="009e7-138">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="009e7-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="009e7-139">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="009e7-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="009e7-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="009e7-140">lastModifiedDateTime</span></span>|<span data-ttu-id="009e7-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="009e7-141">DateTimeOffset</span></span>|<span data-ttu-id="009e7-142">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="009e7-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="009e7-143">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="009e7-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="009e7-144">payloadId</span><span class="sxs-lookup"><span data-stu-id="009e7-144">payloadId</span></span>|<span data-ttu-id="009e7-145">String</span><span class="sxs-lookup"><span data-stu-id="009e7-145">String</span></span>|<span data-ttu-id="009e7-146">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="009e7-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="009e7-147">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="009e7-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="009e7-148">itemType</span><span class="sxs-lookup"><span data-stu-id="009e7-148">itemType</span></span>|<span data-ttu-id="009e7-149">String</span><span class="sxs-lookup"><span data-stu-id="009e7-149">String</span></span>|<span data-ttu-id="009e7-150">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="009e7-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="009e7-151">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="009e7-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="009e7-152">displayName</span><span class="sxs-lookup"><span data-stu-id="009e7-152">displayName</span></span>|<span data-ttu-id="009e7-153">String</span><span class="sxs-lookup"><span data-stu-id="009e7-153">String</span></span>|<span data-ttu-id="009e7-154">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="009e7-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="009e7-155">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="009e7-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="009e7-156">状态</span><span class="sxs-lookup"><span data-stu-id="009e7-156">status</span></span>|[<span data-ttu-id="009e7-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="009e7-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="009e7-158">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="009e7-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="009e7-159">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="009e7-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="009e7-160">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="009e7-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="009e7-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="009e7-161">errorCode</span></span>|[<span data-ttu-id="009e7-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="009e7-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="009e7-163">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="009e7-163">Error code if any occured.</span></span> <span data-ttu-id="009e7-164">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="009e7-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="009e7-165">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="009e7-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="009e7-166">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="009e7-166">guidedDeploymentTags</span></span>|<span data-ttu-id="009e7-167">String 集合</span><span class="sxs-lookup"><span data-stu-id="009e7-167">String collection</span></span>|<span data-ttu-id="009e7-168">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)的引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="009e7-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="009e7-169">priority</span><span class="sxs-lookup"><span data-stu-id="009e7-169">priority</span></span>|<span data-ttu-id="009e7-170">Int32</span><span class="sxs-lookup"><span data-stu-id="009e7-170">Int32</span></span>|<span data-ttu-id="009e7-171">EnrollmentRestrictionsConfigurationPolicySetItem 的优先级。</span><span class="sxs-lookup"><span data-stu-id="009e7-171">Priority of the EnrollmentRestrictionsConfigurationPolicySetItem.</span></span>|
|<span data-ttu-id="009e7-172">limit</span><span class="sxs-lookup"><span data-stu-id="009e7-172">limit</span></span>|<span data-ttu-id="009e7-173">Int32</span><span class="sxs-lookup"><span data-stu-id="009e7-173">Int32</span></span>|<span data-ttu-id="009e7-174">EnrollmentRestrictionsConfigurationPolicySetItem 的限制。</span><span class="sxs-lookup"><span data-stu-id="009e7-174">Limit of the EnrollmentRestrictionsConfigurationPolicySetItem.</span></span>|

## <a name="relationships"></a><span data-ttu-id="009e7-175">关系</span><span class="sxs-lookup"><span data-stu-id="009e7-175">Relationships</span></span>
<span data-ttu-id="009e7-176">无</span><span class="sxs-lookup"><span data-stu-id="009e7-176">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="009e7-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="009e7-177">JSON Representation</span></span>
<span data-ttu-id="009e7-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="009e7-178">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem",
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
  ],
  "priority": 1024,
  "limit": 1024
}
```



