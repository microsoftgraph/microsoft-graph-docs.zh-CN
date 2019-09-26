---
title: policySet 资源类型
description: 包含用于 PolicySet 的属性的类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5aa43500fc2adf9f44ba3bec00cb6c1315fab574
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199961"
---
# <a name="policyset-resource-type"></a><span data-ttu-id="0fe4d-103">policySet 资源类型</span><span class="sxs-lookup"><span data-stu-id="0fe4d-103">policySet resource type</span></span>

> <span data-ttu-id="0fe4d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0fe4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fe4d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0fe4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fe4d-106">包含用于 PolicySet 的属性的类。</span><span class="sxs-lookup"><span data-stu-id="0fe4d-106">A class containing the properties used for PolicySet.</span></span>

## <a name="methods"></a><span data-ttu-id="0fe4d-107">方法</span><span class="sxs-lookup"><span data-stu-id="0fe4d-107">Methods</span></span>
|<span data-ttu-id="0fe4d-108">方法</span><span class="sxs-lookup"><span data-stu-id="0fe4d-108">Method</span></span>|<span data-ttu-id="0fe4d-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="0fe4d-109">Return Type</span></span>|<span data-ttu-id="0fe4d-110">说明</span><span class="sxs-lookup"><span data-stu-id="0fe4d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0fe4d-111">列出 policySets</span><span class="sxs-lookup"><span data-stu-id="0fe4d-111">List policySets</span></span>](../api/intune-policyset-policyset-list.md)|<span data-ttu-id="0fe4d-112">[policySet](../resources/intune-policyset-policyset.md)集合</span><span class="sxs-lookup"><span data-stu-id="0fe4d-112">[policySet](../resources/intune-policyset-policyset.md) collection</span></span>|<span data-ttu-id="0fe4d-113">列出[policySet](../resources/intune-policyset-policyset.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0fe4d-113">List properties and relationships of the [policySet](../resources/intune-policyset-policyset.md) objects.</span></span>|
|[<span data-ttu-id="0fe4d-114">获取 policySet</span><span class="sxs-lookup"><span data-stu-id="0fe4d-114">Get policySet</span></span>](../api/intune-policyset-policyset-get.md)|[<span data-ttu-id="0fe4d-115">policySet</span><span class="sxs-lookup"><span data-stu-id="0fe4d-115">policySet</span></span>](../resources/intune-policyset-policyset.md)|<span data-ttu-id="0fe4d-116">读取[policySet](../resources/intune-policyset-policyset.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0fe4d-116">Read properties and relationships of the [policySet](../resources/intune-policyset-policyset.md) object.</span></span>|
|[<span data-ttu-id="0fe4d-117">创建 policySet</span><span class="sxs-lookup"><span data-stu-id="0fe4d-117">Create policySet</span></span>](../api/intune-policyset-policyset-create.md)|[<span data-ttu-id="0fe4d-118">policySet</span><span class="sxs-lookup"><span data-stu-id="0fe4d-118">policySet</span></span>](../resources/intune-policyset-policyset.md)|<span data-ttu-id="0fe4d-119">创建新的[policySet](../resources/intune-policyset-policyset.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0fe4d-119">Create a new [policySet](../resources/intune-policyset-policyset.md) object.</span></span>|
|[<span data-ttu-id="0fe4d-120">删除 policySet</span><span class="sxs-lookup"><span data-stu-id="0fe4d-120">Delete policySet</span></span>](../api/intune-policyset-policyset-delete.md)|<span data-ttu-id="0fe4d-121">无</span><span class="sxs-lookup"><span data-stu-id="0fe4d-121">None</span></span>|<span data-ttu-id="0fe4d-122">删除[policySet](../resources/intune-policyset-policyset.md)。</span><span class="sxs-lookup"><span data-stu-id="0fe4d-122">Deletes a [policySet](../resources/intune-policyset-policyset.md).</span></span>|
|[<span data-ttu-id="0fe4d-123">更新 policySet</span><span class="sxs-lookup"><span data-stu-id="0fe4d-123">Update policySet</span></span>](../api/intune-policyset-policyset-update.md)|[<span data-ttu-id="0fe4d-124">policySet</span><span class="sxs-lookup"><span data-stu-id="0fe4d-124">policySet</span></span>](../resources/intune-policyset-policyset.md)|<span data-ttu-id="0fe4d-125">更新[policySet](../resources/intune-policyset-policyset.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0fe4d-125">Update the properties of a [policySet](../resources/intune-policyset-policyset.md) object.</span></span>|
|[<span data-ttu-id="0fe4d-126">更新操作</span><span class="sxs-lookup"><span data-stu-id="0fe4d-126">update action</span></span>](../api/intune-policyset-policyset-update.md)|<span data-ttu-id="0fe4d-127">无</span><span class="sxs-lookup"><span data-stu-id="0fe4d-127">None</span></span>|<span data-ttu-id="0fe4d-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0fe4d-128">Not yet documented</span></span>|
|[<span data-ttu-id="0fe4d-129">getPolicySets 操作</span><span class="sxs-lookup"><span data-stu-id="0fe4d-129">getPolicySets action</span></span>](../api/intune-policyset-policyset-getpolicysets.md)|<span data-ttu-id="0fe4d-130">[policySet](../resources/intune-policyset-policyset.md)集合</span><span class="sxs-lookup"><span data-stu-id="0fe4d-130">[policySet](../resources/intune-policyset-policyset.md) collection</span></span>|<span data-ttu-id="0fe4d-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0fe4d-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="0fe4d-132">属性</span><span class="sxs-lookup"><span data-stu-id="0fe4d-132">Properties</span></span>
|<span data-ttu-id="0fe4d-133">属性</span><span class="sxs-lookup"><span data-stu-id="0fe4d-133">Property</span></span>|<span data-ttu-id="0fe4d-134">类型</span><span class="sxs-lookup"><span data-stu-id="0fe4d-134">Type</span></span>|<span data-ttu-id="0fe4d-135">说明</span><span class="sxs-lookup"><span data-stu-id="0fe4d-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fe4d-136">id</span><span class="sxs-lookup"><span data-stu-id="0fe4d-136">id</span></span>|<span data-ttu-id="0fe4d-137">字符串</span><span class="sxs-lookup"><span data-stu-id="0fe4d-137">String</span></span>|<span data-ttu-id="0fe4d-138">PolicySet 的键。</span><span class="sxs-lookup"><span data-stu-id="0fe4d-138">Key of the PolicySet.</span></span>|
|<span data-ttu-id="0fe4d-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0fe4d-139">createdDateTime</span></span>|<span data-ttu-id="0fe4d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fe4d-140">DateTimeOffset</span></span>|<span data-ttu-id="0fe4d-141">PolicySet 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="0fe4d-141">Creation time of the PolicySet.</span></span>|
|<span data-ttu-id="0fe4d-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0fe4d-142">lastModifiedDateTime</span></span>|<span data-ttu-id="0fe4d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fe4d-143">DateTimeOffset</span></span>|<span data-ttu-id="0fe4d-144">PolicySet 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="0fe4d-144">Last modified time of the PolicySet.</span></span>|
|<span data-ttu-id="0fe4d-145">displayName</span><span class="sxs-lookup"><span data-stu-id="0fe4d-145">displayName</span></span>|<span data-ttu-id="0fe4d-146">String</span><span class="sxs-lookup"><span data-stu-id="0fe4d-146">String</span></span>|<span data-ttu-id="0fe4d-147">PolicySet 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="0fe4d-147">DisplayName of the PolicySet.</span></span>|
|<span data-ttu-id="0fe4d-148">说明</span><span class="sxs-lookup"><span data-stu-id="0fe4d-148">description</span></span>|<span data-ttu-id="0fe4d-149">String</span><span class="sxs-lookup"><span data-stu-id="0fe4d-149">String</span></span>|<span data-ttu-id="0fe4d-150">PolicySet 的说明。</span><span class="sxs-lookup"><span data-stu-id="0fe4d-150">Description of the PolicySet.</span></span>|
|<span data-ttu-id="0fe4d-151">status</span><span class="sxs-lookup"><span data-stu-id="0fe4d-151">status</span></span>|[<span data-ttu-id="0fe4d-152">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="0fe4d-152">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="0fe4d-153">PolicySet 的验证/分配状态。</span><span class="sxs-lookup"><span data-stu-id="0fe4d-153">Validation/assignment status of the PolicySet.</span></span> <span data-ttu-id="0fe4d-154">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="0fe4d-154">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="0fe4d-155">errorCode</span><span class="sxs-lookup"><span data-stu-id="0fe4d-155">errorCode</span></span>|[<span data-ttu-id="0fe4d-156">错误</span><span class="sxs-lookup"><span data-stu-id="0fe4d-156">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="0fe4d-157">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="0fe4d-157">Error code if any occured.</span></span> <span data-ttu-id="0fe4d-158">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="0fe4d-158">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="0fe4d-159">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="0fe4d-159">guidedDeploymentTags</span></span>|<span data-ttu-id="0fe4d-160">String collection</span><span class="sxs-lookup"><span data-stu-id="0fe4d-160">String collection</span></span>|<span data-ttu-id="0fe4d-161">引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="0fe4d-161">Tags of the guided deployment</span></span>|
|<span data-ttu-id="0fe4d-162">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="0fe4d-162">roleScopeTags</span></span>|<span data-ttu-id="0fe4d-163">String collection</span><span class="sxs-lookup"><span data-stu-id="0fe4d-163">String collection</span></span>|<span data-ttu-id="0fe4d-164">PolicySet 的 RoleScopeTags</span><span class="sxs-lookup"><span data-stu-id="0fe4d-164">RoleScopeTags of the PolicySet</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fe4d-165">关系</span><span class="sxs-lookup"><span data-stu-id="0fe4d-165">Relationships</span></span>
|<span data-ttu-id="0fe4d-166">关系</span><span class="sxs-lookup"><span data-stu-id="0fe4d-166">Relationship</span></span>|<span data-ttu-id="0fe4d-167">类型</span><span class="sxs-lookup"><span data-stu-id="0fe4d-167">Type</span></span>|<span data-ttu-id="0fe4d-168">说明</span><span class="sxs-lookup"><span data-stu-id="0fe4d-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fe4d-169">assignments</span><span class="sxs-lookup"><span data-stu-id="0fe4d-169">assignments</span></span>|<span data-ttu-id="0fe4d-170">[policySetAssignment](../resources/intune-policyset-policysetassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="0fe4d-170">[policySetAssignment](../resources/intune-policyset-policysetassignment.md) collection</span></span>|<span data-ttu-id="0fe4d-171">PolicySet 的分配。</span><span class="sxs-lookup"><span data-stu-id="0fe4d-171">Assignments of the PolicySet.</span></span>|
|<span data-ttu-id="0fe4d-172">items</span><span class="sxs-lookup"><span data-stu-id="0fe4d-172">items</span></span>|<span data-ttu-id="0fe4d-173">[policySetItem](../resources/intune-policyset-policysetitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="0fe4d-173">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="0fe4d-174">PolicySet 的项目，最大计数为100。</span><span class="sxs-lookup"><span data-stu-id="0fe4d-174">Items of the PolicySet with maximum count 100.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0fe4d-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0fe4d-175">JSON Representation</span></span>
<span data-ttu-id="0fe4d-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fe4d-176">Here is a JSON representation of the resource.</span></span>
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



