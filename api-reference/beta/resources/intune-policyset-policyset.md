---
title: policySet 资源类型
description: 包含用于 PolicySet 的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 845f353a7eb1f5fd95e460a68f23404b88b7a0b5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458326"
---
# <a name="policyset-resource-type"></a><span data-ttu-id="b9f2f-103">policySet 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9f2f-103">policySet resource type</span></span>

<span data-ttu-id="b9f2f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9f2f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9f2f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b9f2f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9f2f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9f2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9f2f-107">包含用于 PolicySet 的属性的类。</span><span class="sxs-lookup"><span data-stu-id="b9f2f-107">A class containing the properties used for PolicySet.</span></span>

## <a name="methods"></a><span data-ttu-id="b9f2f-108">方法</span><span class="sxs-lookup"><span data-stu-id="b9f2f-108">Methods</span></span>
|<span data-ttu-id="b9f2f-109">方法</span><span class="sxs-lookup"><span data-stu-id="b9f2f-109">Method</span></span>|<span data-ttu-id="b9f2f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b9f2f-110">Return Type</span></span>|<span data-ttu-id="b9f2f-111">说明</span><span class="sxs-lookup"><span data-stu-id="b9f2f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b9f2f-112">列出 policySets</span><span class="sxs-lookup"><span data-stu-id="b9f2f-112">List policySets</span></span>](../api/intune-policyset-policyset-list.md)|<span data-ttu-id="b9f2f-113">[policySet](../resources/intune-policyset-policyset.md)集合</span><span class="sxs-lookup"><span data-stu-id="b9f2f-113">[policySet](../resources/intune-policyset-policyset.md) collection</span></span>|<span data-ttu-id="b9f2f-114">列出[policySet](../resources/intune-policyset-policyset.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b9f2f-114">List properties and relationships of the [policySet](../resources/intune-policyset-policyset.md) objects.</span></span>|
|[<span data-ttu-id="b9f2f-115">获取 policySet</span><span class="sxs-lookup"><span data-stu-id="b9f2f-115">Get policySet</span></span>](../api/intune-policyset-policyset-get.md)|[<span data-ttu-id="b9f2f-116">policySet</span><span class="sxs-lookup"><span data-stu-id="b9f2f-116">policySet</span></span>](../resources/intune-policyset-policyset.md)|<span data-ttu-id="b9f2f-117">读取[policySet](../resources/intune-policyset-policyset.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b9f2f-117">Read properties and relationships of the [policySet](../resources/intune-policyset-policyset.md) object.</span></span>|
|[<span data-ttu-id="b9f2f-118">创建 policySet</span><span class="sxs-lookup"><span data-stu-id="b9f2f-118">Create policySet</span></span>](../api/intune-policyset-policyset-create.md)|[<span data-ttu-id="b9f2f-119">policySet</span><span class="sxs-lookup"><span data-stu-id="b9f2f-119">policySet</span></span>](../resources/intune-policyset-policyset.md)|<span data-ttu-id="b9f2f-120">创建新的[policySet](../resources/intune-policyset-policyset.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b9f2f-120">Create a new [policySet](../resources/intune-policyset-policyset.md) object.</span></span>|
|[<span data-ttu-id="b9f2f-121">删除 policySet</span><span class="sxs-lookup"><span data-stu-id="b9f2f-121">Delete policySet</span></span>](../api/intune-policyset-policyset-delete.md)|<span data-ttu-id="b9f2f-122">无</span><span class="sxs-lookup"><span data-stu-id="b9f2f-122">None</span></span>|<span data-ttu-id="b9f2f-123">删除[policySet](../resources/intune-policyset-policyset.md)。</span><span class="sxs-lookup"><span data-stu-id="b9f2f-123">Deletes a [policySet](../resources/intune-policyset-policyset.md).</span></span>|
|[<span data-ttu-id="b9f2f-124">更新 policySet</span><span class="sxs-lookup"><span data-stu-id="b9f2f-124">Update policySet</span></span>](../api/intune-policyset-policyset-update.md)|[<span data-ttu-id="b9f2f-125">policySet</span><span class="sxs-lookup"><span data-stu-id="b9f2f-125">policySet</span></span>](../resources/intune-policyset-policyset.md)|<span data-ttu-id="b9f2f-126">更新[policySet](../resources/intune-policyset-policyset.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b9f2f-126">Update the properties of a [policySet](../resources/intune-policyset-policyset.md) object.</span></span>|
|[<span data-ttu-id="b9f2f-127">更新操作</span><span class="sxs-lookup"><span data-stu-id="b9f2f-127">update action</span></span>](../api/intune-policyset-policyset-update.md)|<span data-ttu-id="b9f2f-128">无</span><span class="sxs-lookup"><span data-stu-id="b9f2f-128">None</span></span>|<span data-ttu-id="b9f2f-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b9f2f-129">Not yet documented</span></span>|
|[<span data-ttu-id="b9f2f-130">getPolicySets 操作</span><span class="sxs-lookup"><span data-stu-id="b9f2f-130">getPolicySets action</span></span>](../api/intune-policyset-policyset-getpolicysets.md)|<span data-ttu-id="b9f2f-131">[policySet](../resources/intune-policyset-policyset.md)集合</span><span class="sxs-lookup"><span data-stu-id="b9f2f-131">[policySet](../resources/intune-policyset-policyset.md) collection</span></span>|<span data-ttu-id="b9f2f-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b9f2f-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="b9f2f-133">属性</span><span class="sxs-lookup"><span data-stu-id="b9f2f-133">Properties</span></span>
|<span data-ttu-id="b9f2f-134">属性</span><span class="sxs-lookup"><span data-stu-id="b9f2f-134">Property</span></span>|<span data-ttu-id="b9f2f-135">类型</span><span class="sxs-lookup"><span data-stu-id="b9f2f-135">Type</span></span>|<span data-ttu-id="b9f2f-136">说明</span><span class="sxs-lookup"><span data-stu-id="b9f2f-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9f2f-137">id</span><span class="sxs-lookup"><span data-stu-id="b9f2f-137">id</span></span>|<span data-ttu-id="b9f2f-138">字符串</span><span class="sxs-lookup"><span data-stu-id="b9f2f-138">String</span></span>|<span data-ttu-id="b9f2f-139">PolicySet 的键。</span><span class="sxs-lookup"><span data-stu-id="b9f2f-139">Key of the PolicySet.</span></span>|
|<span data-ttu-id="b9f2f-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9f2f-140">createdDateTime</span></span>|<span data-ttu-id="b9f2f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9f2f-141">DateTimeOffset</span></span>|<span data-ttu-id="b9f2f-142">PolicySet 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="b9f2f-142">Creation time of the PolicySet.</span></span>|
|<span data-ttu-id="b9f2f-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9f2f-143">lastModifiedDateTime</span></span>|<span data-ttu-id="b9f2f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9f2f-144">DateTimeOffset</span></span>|<span data-ttu-id="b9f2f-145">PolicySet 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="b9f2f-145">Last modified time of the PolicySet.</span></span>|
|<span data-ttu-id="b9f2f-146">displayName</span><span class="sxs-lookup"><span data-stu-id="b9f2f-146">displayName</span></span>|<span data-ttu-id="b9f2f-147">String</span><span class="sxs-lookup"><span data-stu-id="b9f2f-147">String</span></span>|<span data-ttu-id="b9f2f-148">PolicySet 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="b9f2f-148">DisplayName of the PolicySet.</span></span>|
|<span data-ttu-id="b9f2f-149">description</span><span class="sxs-lookup"><span data-stu-id="b9f2f-149">description</span></span>|<span data-ttu-id="b9f2f-150">String</span><span class="sxs-lookup"><span data-stu-id="b9f2f-150">String</span></span>|<span data-ttu-id="b9f2f-151">PolicySet 的说明。</span><span class="sxs-lookup"><span data-stu-id="b9f2f-151">Description of the PolicySet.</span></span>|
|<span data-ttu-id="b9f2f-152">状态</span><span class="sxs-lookup"><span data-stu-id="b9f2f-152">status</span></span>|[<span data-ttu-id="b9f2f-153">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="b9f2f-153">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="b9f2f-154">PolicySet 的验证/分配状态。</span><span class="sxs-lookup"><span data-stu-id="b9f2f-154">Validation/assignment status of the PolicySet.</span></span> <span data-ttu-id="b9f2f-155">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="b9f2f-155">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="b9f2f-156">errorCode</span><span class="sxs-lookup"><span data-stu-id="b9f2f-156">errorCode</span></span>|[<span data-ttu-id="b9f2f-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="b9f2f-157">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="b9f2f-158">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="b9f2f-158">Error code if any occured.</span></span> <span data-ttu-id="b9f2f-159">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="b9f2f-159">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="b9f2f-160">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="b9f2f-160">guidedDeploymentTags</span></span>|<span data-ttu-id="b9f2f-161">String 集合</span><span class="sxs-lookup"><span data-stu-id="b9f2f-161">String collection</span></span>|<span data-ttu-id="b9f2f-162">引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="b9f2f-162">Tags of the guided deployment</span></span>|
|<span data-ttu-id="b9f2f-163">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="b9f2f-163">roleScopeTags</span></span>|<span data-ttu-id="b9f2f-164">String 集合</span><span class="sxs-lookup"><span data-stu-id="b9f2f-164">String collection</span></span>|<span data-ttu-id="b9f2f-165">PolicySet 的 RoleScopeTags</span><span class="sxs-lookup"><span data-stu-id="b9f2f-165">RoleScopeTags of the PolicySet</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9f2f-166">关系</span><span class="sxs-lookup"><span data-stu-id="b9f2f-166">Relationships</span></span>
|<span data-ttu-id="b9f2f-167">关系</span><span class="sxs-lookup"><span data-stu-id="b9f2f-167">Relationship</span></span>|<span data-ttu-id="b9f2f-168">类型</span><span class="sxs-lookup"><span data-stu-id="b9f2f-168">Type</span></span>|<span data-ttu-id="b9f2f-169">说明</span><span class="sxs-lookup"><span data-stu-id="b9f2f-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9f2f-170">assignments</span><span class="sxs-lookup"><span data-stu-id="b9f2f-170">assignments</span></span>|<span data-ttu-id="b9f2f-171">[policySetAssignment](../resources/intune-policyset-policysetassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="b9f2f-171">[policySetAssignment](../resources/intune-policyset-policysetassignment.md) collection</span></span>|<span data-ttu-id="b9f2f-172">PolicySet 的分配。</span><span class="sxs-lookup"><span data-stu-id="b9f2f-172">Assignments of the PolicySet.</span></span>|
|<span data-ttu-id="b9f2f-173">items</span><span class="sxs-lookup"><span data-stu-id="b9f2f-173">items</span></span>|<span data-ttu-id="b9f2f-174">[policySetItem](../resources/intune-policyset-policysetitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="b9f2f-174">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="b9f2f-175">PolicySet 的项目，最大计数为100。</span><span class="sxs-lookup"><span data-stu-id="b9f2f-175">Items of the PolicySet with maximum count 100.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9f2f-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9f2f-176">JSON Representation</span></span>
<span data-ttu-id="b9f2f-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9f2f-177">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policySet",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ],
  "roleScopeTags": [
    "String"
  ]
}
```



