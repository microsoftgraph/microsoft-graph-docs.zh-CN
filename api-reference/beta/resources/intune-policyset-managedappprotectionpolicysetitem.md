---
title: managedAppProtectionPolicySetItem 资源类型
description: 包含用于托管应用程序保护 PolicySetItem 的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4d9f46c55550559408b32b8d6788fb66cb463616
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993474"
---
# <a name="managedappprotectionpolicysetitem-resource-type"></a><span data-ttu-id="ea0fe-103">managedAppProtectionPolicySetItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="ea0fe-103">managedAppProtectionPolicySetItem resource type</span></span>

<span data-ttu-id="ea0fe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea0fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea0fe-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea0fe-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea0fe-107">包含用于托管应用程序保护 PolicySetItem 的属性的类。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-107">A class containing the properties used for managed app protection PolicySetItem.</span></span>


<span data-ttu-id="ea0fe-108">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ea0fe-108">Inherits from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ea0fe-109">方法</span><span class="sxs-lookup"><span data-stu-id="ea0fe-109">Methods</span></span>
|<span data-ttu-id="ea0fe-110">方法</span><span class="sxs-lookup"><span data-stu-id="ea0fe-110">Method</span></span>|<span data-ttu-id="ea0fe-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="ea0fe-111">Return Type</span></span>|<span data-ttu-id="ea0fe-112">说明</span><span class="sxs-lookup"><span data-stu-id="ea0fe-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ea0fe-113">列出 managedAppProtectionPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="ea0fe-113">List managedAppProtectionPolicySetItems</span></span>](../api/intune-policyset-managedappprotectionpolicysetitem-list.md)|<span data-ttu-id="ea0fe-114">[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ea0fe-114">[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) collection</span></span>|<span data-ttu-id="ea0fe-115">列出 [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-115">List properties and relationships of the [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) objects.</span></span>|
|[<span data-ttu-id="ea0fe-116">获取 managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="ea0fe-116">Get managedAppProtectionPolicySetItem</span></span>](../api/intune-policyset-managedappprotectionpolicysetitem-get.md)|[<span data-ttu-id="ea0fe-117">managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="ea0fe-117">managedAppProtectionPolicySetItem</span></span>](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|<span data-ttu-id="ea0fe-118">读取 [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-118">Read properties and relationships of the [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>|
|[<span data-ttu-id="ea0fe-119">创建 managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="ea0fe-119">Create managedAppProtectionPolicySetItem</span></span>](../api/intune-policyset-managedappprotectionpolicysetitem-create.md)|[<span data-ttu-id="ea0fe-120">managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="ea0fe-120">managedAppProtectionPolicySetItem</span></span>](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|<span data-ttu-id="ea0fe-121">创建新的 [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-121">Create a new [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>|
|[<span data-ttu-id="ea0fe-122">删除 managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="ea0fe-122">Delete managedAppProtectionPolicySetItem</span></span>](../api/intune-policyset-managedappprotectionpolicysetitem-delete.md)|<span data-ttu-id="ea0fe-123">无</span><span class="sxs-lookup"><span data-stu-id="ea0fe-123">None</span></span>|<span data-ttu-id="ea0fe-124">删除 [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-124">Deletes a [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md).</span></span>|
|[<span data-ttu-id="ea0fe-125">更新 managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="ea0fe-125">Update managedAppProtectionPolicySetItem</span></span>](../api/intune-policyset-managedappprotectionpolicysetitem-update.md)|[<span data-ttu-id="ea0fe-126">managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="ea0fe-126">managedAppProtectionPolicySetItem</span></span>](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|<span data-ttu-id="ea0fe-127">更新 [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-127">Update the properties of a [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ea0fe-128">属性</span><span class="sxs-lookup"><span data-stu-id="ea0fe-128">Properties</span></span>
|<span data-ttu-id="ea0fe-129">属性</span><span class="sxs-lookup"><span data-stu-id="ea0fe-129">Property</span></span>|<span data-ttu-id="ea0fe-130">类型</span><span class="sxs-lookup"><span data-stu-id="ea0fe-130">Type</span></span>|<span data-ttu-id="ea0fe-131">说明</span><span class="sxs-lookup"><span data-stu-id="ea0fe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea0fe-132">id</span><span class="sxs-lookup"><span data-stu-id="ea0fe-132">id</span></span>|<span data-ttu-id="ea0fe-133">String</span><span class="sxs-lookup"><span data-stu-id="ea0fe-133">String</span></span>|<span data-ttu-id="ea0fe-134">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="ea0fe-135">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ea0fe-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="ea0fe-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ea0fe-136">createdDateTime</span></span>|<span data-ttu-id="ea0fe-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea0fe-137">DateTimeOffset</span></span>|<span data-ttu-id="ea0fe-138">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="ea0fe-139">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ea0fe-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="ea0fe-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea0fe-140">lastModifiedDateTime</span></span>|<span data-ttu-id="ea0fe-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea0fe-141">DateTimeOffset</span></span>|<span data-ttu-id="ea0fe-142">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="ea0fe-143">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ea0fe-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="ea0fe-144">payloadId</span><span class="sxs-lookup"><span data-stu-id="ea0fe-144">payloadId</span></span>|<span data-ttu-id="ea0fe-145">String</span><span class="sxs-lookup"><span data-stu-id="ea0fe-145">String</span></span>|<span data-ttu-id="ea0fe-146">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="ea0fe-147">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ea0fe-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="ea0fe-148">itemType</span><span class="sxs-lookup"><span data-stu-id="ea0fe-148">itemType</span></span>|<span data-ttu-id="ea0fe-149">String</span><span class="sxs-lookup"><span data-stu-id="ea0fe-149">String</span></span>|<span data-ttu-id="ea0fe-150">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="ea0fe-151">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ea0fe-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="ea0fe-152">displayName</span><span class="sxs-lookup"><span data-stu-id="ea0fe-152">displayName</span></span>|<span data-ttu-id="ea0fe-153">String</span><span class="sxs-lookup"><span data-stu-id="ea0fe-153">String</span></span>|<span data-ttu-id="ea0fe-154">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="ea0fe-155">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ea0fe-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="ea0fe-156">状态</span><span class="sxs-lookup"><span data-stu-id="ea0fe-156">status</span></span>|[<span data-ttu-id="ea0fe-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="ea0fe-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="ea0fe-158">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="ea0fe-159">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="ea0fe-160">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="ea0fe-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="ea0fe-161">errorCode</span></span>|[<span data-ttu-id="ea0fe-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="ea0fe-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="ea0fe-163">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-163">Error code if any occured.</span></span> <span data-ttu-id="ea0fe-164">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="ea0fe-165">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="ea0fe-166">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="ea0fe-166">guidedDeploymentTags</span></span>|<span data-ttu-id="ea0fe-167">String collection</span><span class="sxs-lookup"><span data-stu-id="ea0fe-167">String collection</span></span>|<span data-ttu-id="ea0fe-168">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)的引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="ea0fe-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="ea0fe-169">targetedAppManagementLevels</span><span class="sxs-lookup"><span data-stu-id="ea0fe-169">targetedAppManagementLevels</span></span>|<span data-ttu-id="ea0fe-170">String</span><span class="sxs-lookup"><span data-stu-id="ea0fe-170">String</span></span>|<span data-ttu-id="ea0fe-171">ManagedAppPolicySetItem 的 TargetedAppManagementLevels。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-171">TargetedAppManagementLevels of the ManagedAppPolicySetItem.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea0fe-172">关系</span><span class="sxs-lookup"><span data-stu-id="ea0fe-172">Relationships</span></span>
<span data-ttu-id="ea0fe-173">无</span><span class="sxs-lookup"><span data-stu-id="ea0fe-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea0fe-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ea0fe-174">JSON Representation</span></span>
<span data-ttu-id="ea0fe-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea0fe-175">Here is a JSON representation of the resource.</span></span>
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






