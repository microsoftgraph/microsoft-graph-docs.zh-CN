---
title: managedAppProtectionPolicySetItem 资源类型
description: 包含用于托管应用程序保护 PolicySetItem 的属性的类。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4e8bdc277f92d30f6506b5528bc00816d8639e65
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42775736"
---
# <a name="managedappprotectionpolicysetitem-resource-type"></a><span data-ttu-id="99af3-103">managedAppProtectionPolicySetItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="99af3-103">managedAppProtectionPolicySetItem resource type</span></span>

> <span data-ttu-id="99af3-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="99af3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99af3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="99af3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99af3-106">包含用于托管应用程序保护 PolicySetItem 的属性的类。</span><span class="sxs-lookup"><span data-stu-id="99af3-106">A class containing the properties used for managed app protection PolicySetItem.</span></span>


<span data-ttu-id="99af3-107">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="99af3-107">Inherits from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>

## <a name="methods"></a><span data-ttu-id="99af3-108">方法</span><span class="sxs-lookup"><span data-stu-id="99af3-108">Methods</span></span>
|<span data-ttu-id="99af3-109">方法</span><span class="sxs-lookup"><span data-stu-id="99af3-109">Method</span></span>|<span data-ttu-id="99af3-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="99af3-110">Return Type</span></span>|<span data-ttu-id="99af3-111">说明</span><span class="sxs-lookup"><span data-stu-id="99af3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="99af3-112">列出 managedAppProtectionPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="99af3-112">List managedAppProtectionPolicySetItems</span></span>](../api/intune-policyset-managedappprotectionpolicysetitem-list.md)|<span data-ttu-id="99af3-113">[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="99af3-113">[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) collection</span></span>|<span data-ttu-id="99af3-114">列出[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="99af3-114">List properties and relationships of the [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) objects.</span></span>|
|[<span data-ttu-id="99af3-115">获取 managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="99af3-115">Get managedAppProtectionPolicySetItem</span></span>](../api/intune-policyset-managedappprotectionpolicysetitem-get.md)|[<span data-ttu-id="99af3-116">managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="99af3-116">managedAppProtectionPolicySetItem</span></span>](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|<span data-ttu-id="99af3-117">读取[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="99af3-117">Read properties and relationships of the [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>|
|[<span data-ttu-id="99af3-118">创建 managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="99af3-118">Create managedAppProtectionPolicySetItem</span></span>](../api/intune-policyset-managedappprotectionpolicysetitem-create.md)|[<span data-ttu-id="99af3-119">managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="99af3-119">managedAppProtectionPolicySetItem</span></span>](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|<span data-ttu-id="99af3-120">创建新的[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="99af3-120">Create a new [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>|
|[<span data-ttu-id="99af3-121">删除 managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="99af3-121">Delete managedAppProtectionPolicySetItem</span></span>](../api/intune-policyset-managedappprotectionpolicysetitem-delete.md)|<span data-ttu-id="99af3-122">None</span><span class="sxs-lookup"><span data-stu-id="99af3-122">None</span></span>|<span data-ttu-id="99af3-123">删除[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="99af3-123">Deletes a [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md).</span></span>|
|[<span data-ttu-id="99af3-124">更新 managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="99af3-124">Update managedAppProtectionPolicySetItem</span></span>](../api/intune-policyset-managedappprotectionpolicysetitem-update.md)|[<span data-ttu-id="99af3-125">managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="99af3-125">managedAppProtectionPolicySetItem</span></span>](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|<span data-ttu-id="99af3-126">更新[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="99af3-126">Update the properties of a [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="99af3-127">属性</span><span class="sxs-lookup"><span data-stu-id="99af3-127">Properties</span></span>
|<span data-ttu-id="99af3-128">属性</span><span class="sxs-lookup"><span data-stu-id="99af3-128">Property</span></span>|<span data-ttu-id="99af3-129">类型</span><span class="sxs-lookup"><span data-stu-id="99af3-129">Type</span></span>|<span data-ttu-id="99af3-130">说明</span><span class="sxs-lookup"><span data-stu-id="99af3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99af3-131">id</span><span class="sxs-lookup"><span data-stu-id="99af3-131">id</span></span>|<span data-ttu-id="99af3-132">String</span><span class="sxs-lookup"><span data-stu-id="99af3-132">String</span></span>|<span data-ttu-id="99af3-133">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="99af3-133">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="99af3-134">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="99af3-134">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="99af3-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99af3-135">createdDateTime</span></span>|<span data-ttu-id="99af3-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99af3-136">DateTimeOffset</span></span>|<span data-ttu-id="99af3-137">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="99af3-137">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="99af3-138">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="99af3-138">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="99af3-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99af3-139">lastModifiedDateTime</span></span>|<span data-ttu-id="99af3-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99af3-140">DateTimeOffset</span></span>|<span data-ttu-id="99af3-141">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="99af3-141">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="99af3-142">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="99af3-142">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="99af3-143">payloadId</span><span class="sxs-lookup"><span data-stu-id="99af3-143">payloadId</span></span>|<span data-ttu-id="99af3-144">String</span><span class="sxs-lookup"><span data-stu-id="99af3-144">String</span></span>|<span data-ttu-id="99af3-145">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="99af3-145">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="99af3-146">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="99af3-146">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="99af3-147">itemType</span><span class="sxs-lookup"><span data-stu-id="99af3-147">itemType</span></span>|<span data-ttu-id="99af3-148">String</span><span class="sxs-lookup"><span data-stu-id="99af3-148">String</span></span>|<span data-ttu-id="99af3-149">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="99af3-149">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="99af3-150">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="99af3-150">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="99af3-151">displayName</span><span class="sxs-lookup"><span data-stu-id="99af3-151">displayName</span></span>|<span data-ttu-id="99af3-152">String</span><span class="sxs-lookup"><span data-stu-id="99af3-152">String</span></span>|<span data-ttu-id="99af3-153">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="99af3-153">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="99af3-154">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="99af3-154">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="99af3-155">状态</span><span class="sxs-lookup"><span data-stu-id="99af3-155">status</span></span>|[<span data-ttu-id="99af3-156">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="99af3-156">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="99af3-157">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="99af3-157">Status of the PolicySetItem.</span></span> <span data-ttu-id="99af3-158">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="99af3-158">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="99af3-159">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="99af3-159">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="99af3-160">errorCode</span><span class="sxs-lookup"><span data-stu-id="99af3-160">errorCode</span></span>|[<span data-ttu-id="99af3-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="99af3-161">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="99af3-162">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="99af3-162">Error code if any occured.</span></span> <span data-ttu-id="99af3-163">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="99af3-163">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="99af3-164">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="99af3-164">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="99af3-165">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="99af3-165">guidedDeploymentTags</span></span>|<span data-ttu-id="99af3-166">String collection</span><span class="sxs-lookup"><span data-stu-id="99af3-166">String collection</span></span>|<span data-ttu-id="99af3-167">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)的引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="99af3-167">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="99af3-168">targetedAppManagementLevels</span><span class="sxs-lookup"><span data-stu-id="99af3-168">targetedAppManagementLevels</span></span>|<span data-ttu-id="99af3-169">String</span><span class="sxs-lookup"><span data-stu-id="99af3-169">String</span></span>|<span data-ttu-id="99af3-170">ManagedAppPolicySetItem 的 TargetedAppManagementLevels。</span><span class="sxs-lookup"><span data-stu-id="99af3-170">TargetedAppManagementLevels of the ManagedAppPolicySetItem.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99af3-171">关系</span><span class="sxs-lookup"><span data-stu-id="99af3-171">Relationships</span></span>
<span data-ttu-id="99af3-172">无</span><span class="sxs-lookup"><span data-stu-id="99af3-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99af3-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99af3-173">JSON Representation</span></span>
<span data-ttu-id="99af3-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99af3-174">Here is a JSON representation of the resource.</span></span>
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



