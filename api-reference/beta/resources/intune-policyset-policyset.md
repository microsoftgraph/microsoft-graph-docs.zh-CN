---
title: policySet 资源类型
description: 包含用于 PolicySet 的属性的类。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d50b59deb24bba2e10e6060a46b41e435b779f4a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42775203"
---
# <a name="policyset-resource-type"></a><span data-ttu-id="84fc4-103">policySet 资源类型</span><span class="sxs-lookup"><span data-stu-id="84fc4-103">policySet resource type</span></span>

> <span data-ttu-id="84fc4-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="84fc4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84fc4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="84fc4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84fc4-106">包含用于 PolicySet 的属性的类。</span><span class="sxs-lookup"><span data-stu-id="84fc4-106">A class containing the properties used for PolicySet.</span></span>

## <a name="methods"></a><span data-ttu-id="84fc4-107">方法</span><span class="sxs-lookup"><span data-stu-id="84fc4-107">Methods</span></span>
|<span data-ttu-id="84fc4-108">方法</span><span class="sxs-lookup"><span data-stu-id="84fc4-108">Method</span></span>|<span data-ttu-id="84fc4-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="84fc4-109">Return Type</span></span>|<span data-ttu-id="84fc4-110">说明</span><span class="sxs-lookup"><span data-stu-id="84fc4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="84fc4-111">列出 policySets</span><span class="sxs-lookup"><span data-stu-id="84fc4-111">List policySets</span></span>](../api/intune-policyset-policyset-list.md)|<span data-ttu-id="84fc4-112">[policySet](../resources/intune-policyset-policyset.md)集合</span><span class="sxs-lookup"><span data-stu-id="84fc4-112">[policySet](../resources/intune-policyset-policyset.md) collection</span></span>|<span data-ttu-id="84fc4-113">列出[policySet](../resources/intune-policyset-policyset.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="84fc4-113">List properties and relationships of the [policySet](../resources/intune-policyset-policyset.md) objects.</span></span>|
|[<span data-ttu-id="84fc4-114">获取 policySet</span><span class="sxs-lookup"><span data-stu-id="84fc4-114">Get policySet</span></span>](../api/intune-policyset-policyset-get.md)|[<span data-ttu-id="84fc4-115">policySet</span><span class="sxs-lookup"><span data-stu-id="84fc4-115">policySet</span></span>](../resources/intune-policyset-policyset.md)|<span data-ttu-id="84fc4-116">读取[policySet](../resources/intune-policyset-policyset.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="84fc4-116">Read properties and relationships of the [policySet](../resources/intune-policyset-policyset.md) object.</span></span>|
|[<span data-ttu-id="84fc4-117">创建 policySet</span><span class="sxs-lookup"><span data-stu-id="84fc4-117">Create policySet</span></span>](../api/intune-policyset-policyset-create.md)|[<span data-ttu-id="84fc4-118">policySet</span><span class="sxs-lookup"><span data-stu-id="84fc4-118">policySet</span></span>](../resources/intune-policyset-policyset.md)|<span data-ttu-id="84fc4-119">创建新的[policySet](../resources/intune-policyset-policyset.md)对象。</span><span class="sxs-lookup"><span data-stu-id="84fc4-119">Create a new [policySet](../resources/intune-policyset-policyset.md) object.</span></span>|
|[<span data-ttu-id="84fc4-120">删除 policySet</span><span class="sxs-lookup"><span data-stu-id="84fc4-120">Delete policySet</span></span>](../api/intune-policyset-policyset-delete.md)|<span data-ttu-id="84fc4-121">None</span><span class="sxs-lookup"><span data-stu-id="84fc4-121">None</span></span>|<span data-ttu-id="84fc4-122">删除[policySet](../resources/intune-policyset-policyset.md)。</span><span class="sxs-lookup"><span data-stu-id="84fc4-122">Deletes a [policySet](../resources/intune-policyset-policyset.md).</span></span>|
|[<span data-ttu-id="84fc4-123">更新 policySet</span><span class="sxs-lookup"><span data-stu-id="84fc4-123">Update policySet</span></span>](../api/intune-policyset-policyset-update.md)|[<span data-ttu-id="84fc4-124">policySet</span><span class="sxs-lookup"><span data-stu-id="84fc4-124">policySet</span></span>](../resources/intune-policyset-policyset.md)|<span data-ttu-id="84fc4-125">更新[policySet](../resources/intune-policyset-policyset.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="84fc4-125">Update the properties of a [policySet](../resources/intune-policyset-policyset.md) object.</span></span>|
|[<span data-ttu-id="84fc4-126">更新操作</span><span class="sxs-lookup"><span data-stu-id="84fc4-126">update action</span></span>](../api/intune-policyset-policyset-update.md)|<span data-ttu-id="84fc4-127">无</span><span class="sxs-lookup"><span data-stu-id="84fc4-127">None</span></span>|<span data-ttu-id="84fc4-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="84fc4-128">Not yet documented</span></span>|
|[<span data-ttu-id="84fc4-129">getPolicySets 操作</span><span class="sxs-lookup"><span data-stu-id="84fc4-129">getPolicySets action</span></span>](../api/intune-policyset-policyset-getpolicysets.md)|<span data-ttu-id="84fc4-130">[policySet](../resources/intune-policyset-policyset.md)集合</span><span class="sxs-lookup"><span data-stu-id="84fc4-130">[policySet](../resources/intune-policyset-policyset.md) collection</span></span>|<span data-ttu-id="84fc4-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="84fc4-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="84fc4-132">属性</span><span class="sxs-lookup"><span data-stu-id="84fc4-132">Properties</span></span>
|<span data-ttu-id="84fc4-133">属性</span><span class="sxs-lookup"><span data-stu-id="84fc4-133">Property</span></span>|<span data-ttu-id="84fc4-134">类型</span><span class="sxs-lookup"><span data-stu-id="84fc4-134">Type</span></span>|<span data-ttu-id="84fc4-135">说明</span><span class="sxs-lookup"><span data-stu-id="84fc4-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84fc4-136">id</span><span class="sxs-lookup"><span data-stu-id="84fc4-136">id</span></span>|<span data-ttu-id="84fc4-137">字符串</span><span class="sxs-lookup"><span data-stu-id="84fc4-137">String</span></span>|<span data-ttu-id="84fc4-138">PolicySet 的键。</span><span class="sxs-lookup"><span data-stu-id="84fc4-138">Key of the PolicySet.</span></span>|
|<span data-ttu-id="84fc4-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84fc4-139">createdDateTime</span></span>|<span data-ttu-id="84fc4-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84fc4-140">DateTimeOffset</span></span>|<span data-ttu-id="84fc4-141">PolicySet 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="84fc4-141">Creation time of the PolicySet.</span></span>|
|<span data-ttu-id="84fc4-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84fc4-142">lastModifiedDateTime</span></span>|<span data-ttu-id="84fc4-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84fc4-143">DateTimeOffset</span></span>|<span data-ttu-id="84fc4-144">PolicySet 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="84fc4-144">Last modified time of the PolicySet.</span></span>|
|<span data-ttu-id="84fc4-145">displayName</span><span class="sxs-lookup"><span data-stu-id="84fc4-145">displayName</span></span>|<span data-ttu-id="84fc4-146">String</span><span class="sxs-lookup"><span data-stu-id="84fc4-146">String</span></span>|<span data-ttu-id="84fc4-147">PolicySet 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="84fc4-147">DisplayName of the PolicySet.</span></span>|
|<span data-ttu-id="84fc4-148">说明</span><span class="sxs-lookup"><span data-stu-id="84fc4-148">description</span></span>|<span data-ttu-id="84fc4-149">String</span><span class="sxs-lookup"><span data-stu-id="84fc4-149">String</span></span>|<span data-ttu-id="84fc4-150">PolicySet 的说明。</span><span class="sxs-lookup"><span data-stu-id="84fc4-150">Description of the PolicySet.</span></span>|
|<span data-ttu-id="84fc4-151">状态</span><span class="sxs-lookup"><span data-stu-id="84fc4-151">status</span></span>|[<span data-ttu-id="84fc4-152">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="84fc4-152">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="84fc4-153">PolicySet 的验证/分配状态。</span><span class="sxs-lookup"><span data-stu-id="84fc4-153">Validation/assignment status of the PolicySet.</span></span> <span data-ttu-id="84fc4-154">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="84fc4-154">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="84fc4-155">errorCode</span><span class="sxs-lookup"><span data-stu-id="84fc4-155">errorCode</span></span>|[<span data-ttu-id="84fc4-156">errorCode</span><span class="sxs-lookup"><span data-stu-id="84fc4-156">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="84fc4-157">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="84fc4-157">Error code if any occured.</span></span> <span data-ttu-id="84fc4-158">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="84fc4-158">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="84fc4-159">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="84fc4-159">guidedDeploymentTags</span></span>|<span data-ttu-id="84fc4-160">String collection</span><span class="sxs-lookup"><span data-stu-id="84fc4-160">String collection</span></span>|<span data-ttu-id="84fc4-161">引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="84fc4-161">Tags of the guided deployment</span></span>|
|<span data-ttu-id="84fc4-162">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="84fc4-162">roleScopeTags</span></span>|<span data-ttu-id="84fc4-163">String collection</span><span class="sxs-lookup"><span data-stu-id="84fc4-163">String collection</span></span>|<span data-ttu-id="84fc4-164">PolicySet 的 RoleScopeTags</span><span class="sxs-lookup"><span data-stu-id="84fc4-164">RoleScopeTags of the PolicySet</span></span>|

## <a name="relationships"></a><span data-ttu-id="84fc4-165">关系</span><span class="sxs-lookup"><span data-stu-id="84fc4-165">Relationships</span></span>
|<span data-ttu-id="84fc4-166">关系</span><span class="sxs-lookup"><span data-stu-id="84fc4-166">Relationship</span></span>|<span data-ttu-id="84fc4-167">类型</span><span class="sxs-lookup"><span data-stu-id="84fc4-167">Type</span></span>|<span data-ttu-id="84fc4-168">说明</span><span class="sxs-lookup"><span data-stu-id="84fc4-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84fc4-169">assignments</span><span class="sxs-lookup"><span data-stu-id="84fc4-169">assignments</span></span>|<span data-ttu-id="84fc4-170">[policySetAssignment](../resources/intune-policyset-policysetassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="84fc4-170">[policySetAssignment](../resources/intune-policyset-policysetassignment.md) collection</span></span>|<span data-ttu-id="84fc4-171">PolicySet 的分配。</span><span class="sxs-lookup"><span data-stu-id="84fc4-171">Assignments of the PolicySet.</span></span>|
|<span data-ttu-id="84fc4-172">items</span><span class="sxs-lookup"><span data-stu-id="84fc4-172">items</span></span>|<span data-ttu-id="84fc4-173">[policySetItem](../resources/intune-policyset-policysetitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="84fc4-173">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="84fc4-174">PolicySet 的项目，最大计数为100。</span><span class="sxs-lookup"><span data-stu-id="84fc4-174">Items of the PolicySet with maximum count 100.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="84fc4-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84fc4-175">JSON Representation</span></span>
<span data-ttu-id="84fc4-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84fc4-176">Here is a JSON representation of the resource.</span></span>
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



