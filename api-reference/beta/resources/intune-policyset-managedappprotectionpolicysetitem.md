---
title: managedAppProtectionPolicySetItem 资源类型
description: 包含用于托管应用程序保护 PolicySetItem 的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e160e88c54e7cc8d33e0c78090fbf06dfd52cab1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736049"
---
# <a name="managedappprotectionpolicysetitem-resource-type"></a><span data-ttu-id="74a58-103">managedAppProtectionPolicySetItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="74a58-103">managedAppProtectionPolicySetItem resource type</span></span>

<span data-ttu-id="74a58-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74a58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74a58-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="74a58-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74a58-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="74a58-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74a58-107">包含用于托管应用程序保护 PolicySetItem 的属性的类。</span><span class="sxs-lookup"><span data-stu-id="74a58-107">A class containing the properties used for managed app protection PolicySetItem.</span></span>


<span data-ttu-id="74a58-108">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="74a58-108">Inherits from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>

## <a name="methods"></a><span data-ttu-id="74a58-109">Methods</span><span class="sxs-lookup"><span data-stu-id="74a58-109">Methods</span></span>
|<span data-ttu-id="74a58-110">方法</span><span class="sxs-lookup"><span data-stu-id="74a58-110">Method</span></span>|<span data-ttu-id="74a58-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="74a58-111">Return Type</span></span>|<span data-ttu-id="74a58-112">说明</span><span class="sxs-lookup"><span data-stu-id="74a58-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="74a58-113">列出 managedAppProtectionPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="74a58-113">List managedAppProtectionPolicySetItems</span></span>](../api/intune-policyset-managedappprotectionpolicysetitem-list.md)|<span data-ttu-id="74a58-114">[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="74a58-114">[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) collection</span></span>|<span data-ttu-id="74a58-115">列出 [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="74a58-115">List properties and relationships of the [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) objects.</span></span>|
|[<span data-ttu-id="74a58-116">获取 managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="74a58-116">Get managedAppProtectionPolicySetItem</span></span>](../api/intune-policyset-managedappprotectionpolicysetitem-get.md)|[<span data-ttu-id="74a58-117">managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="74a58-117">managedAppProtectionPolicySetItem</span></span>](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|<span data-ttu-id="74a58-118">读取 [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="74a58-118">Read properties and relationships of the [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>|
|[<span data-ttu-id="74a58-119">创建 managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="74a58-119">Create managedAppProtectionPolicySetItem</span></span>](../api/intune-policyset-managedappprotectionpolicysetitem-create.md)|[<span data-ttu-id="74a58-120">managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="74a58-120">managedAppProtectionPolicySetItem</span></span>](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|<span data-ttu-id="74a58-121">创建新的 [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="74a58-121">Create a new [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>|
|[<span data-ttu-id="74a58-122">删除 managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="74a58-122">Delete managedAppProtectionPolicySetItem</span></span>](../api/intune-policyset-managedappprotectionpolicysetitem-delete.md)|<span data-ttu-id="74a58-123">无</span><span class="sxs-lookup"><span data-stu-id="74a58-123">None</span></span>|<span data-ttu-id="74a58-124">删除 [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="74a58-124">Deletes a [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md).</span></span>|
|[<span data-ttu-id="74a58-125">更新 managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="74a58-125">Update managedAppProtectionPolicySetItem</span></span>](../api/intune-policyset-managedappprotectionpolicysetitem-update.md)|[<span data-ttu-id="74a58-126">managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="74a58-126">managedAppProtectionPolicySetItem</span></span>](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|<span data-ttu-id="74a58-127">更新 [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="74a58-127">Update the properties of a [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="74a58-128">属性</span><span class="sxs-lookup"><span data-stu-id="74a58-128">Properties</span></span>
|<span data-ttu-id="74a58-129">属性</span><span class="sxs-lookup"><span data-stu-id="74a58-129">Property</span></span>|<span data-ttu-id="74a58-130">类型</span><span class="sxs-lookup"><span data-stu-id="74a58-130">Type</span></span>|<span data-ttu-id="74a58-131">说明</span><span class="sxs-lookup"><span data-stu-id="74a58-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74a58-132">id</span><span class="sxs-lookup"><span data-stu-id="74a58-132">id</span></span>|<span data-ttu-id="74a58-133">String</span><span class="sxs-lookup"><span data-stu-id="74a58-133">String</span></span>|<span data-ttu-id="74a58-134">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="74a58-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="74a58-135">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="74a58-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="74a58-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="74a58-136">createdDateTime</span></span>|<span data-ttu-id="74a58-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74a58-137">DateTimeOffset</span></span>|<span data-ttu-id="74a58-138">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="74a58-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="74a58-139">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="74a58-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="74a58-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74a58-140">lastModifiedDateTime</span></span>|<span data-ttu-id="74a58-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74a58-141">DateTimeOffset</span></span>|<span data-ttu-id="74a58-142">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="74a58-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="74a58-143">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="74a58-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="74a58-144">payloadId</span><span class="sxs-lookup"><span data-stu-id="74a58-144">payloadId</span></span>|<span data-ttu-id="74a58-145">String</span><span class="sxs-lookup"><span data-stu-id="74a58-145">String</span></span>|<span data-ttu-id="74a58-146">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="74a58-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="74a58-147">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="74a58-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="74a58-148">itemType</span><span class="sxs-lookup"><span data-stu-id="74a58-148">itemType</span></span>|<span data-ttu-id="74a58-149">String</span><span class="sxs-lookup"><span data-stu-id="74a58-149">String</span></span>|<span data-ttu-id="74a58-150">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="74a58-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="74a58-151">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="74a58-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="74a58-152">displayName</span><span class="sxs-lookup"><span data-stu-id="74a58-152">displayName</span></span>|<span data-ttu-id="74a58-153">String</span><span class="sxs-lookup"><span data-stu-id="74a58-153">String</span></span>|<span data-ttu-id="74a58-154">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="74a58-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="74a58-155">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="74a58-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="74a58-156">status</span><span class="sxs-lookup"><span data-stu-id="74a58-156">status</span></span>|[<span data-ttu-id="74a58-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="74a58-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="74a58-158">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="74a58-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="74a58-159">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="74a58-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="74a58-160">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="74a58-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="74a58-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="74a58-161">errorCode</span></span>|[<span data-ttu-id="74a58-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="74a58-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="74a58-163">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="74a58-163">Error code if any occured.</span></span> <span data-ttu-id="74a58-164">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="74a58-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="74a58-165">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="74a58-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="74a58-166">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="74a58-166">guidedDeploymentTags</span></span>|<span data-ttu-id="74a58-167">String collection</span><span class="sxs-lookup"><span data-stu-id="74a58-167">String collection</span></span>|<span data-ttu-id="74a58-168">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)的引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="74a58-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="74a58-169">targetedAppManagementLevels</span><span class="sxs-lookup"><span data-stu-id="74a58-169">targetedAppManagementLevels</span></span>|<span data-ttu-id="74a58-170">String</span><span class="sxs-lookup"><span data-stu-id="74a58-170">String</span></span>|<span data-ttu-id="74a58-171">ManagedAppPolicySetItem 的 TargetedAppManagementLevels。</span><span class="sxs-lookup"><span data-stu-id="74a58-171">TargetedAppManagementLevels of the ManagedAppPolicySetItem.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74a58-172">关系</span><span class="sxs-lookup"><span data-stu-id="74a58-172">Relationships</span></span>
<span data-ttu-id="74a58-173">无</span><span class="sxs-lookup"><span data-stu-id="74a58-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="74a58-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="74a58-174">JSON Representation</span></span>
<span data-ttu-id="74a58-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74a58-175">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppProtectionPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppProtectionPolicySetItem",
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
  "targetedAppManagementLevels": "String"
}
```





