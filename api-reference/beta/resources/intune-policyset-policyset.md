---
title: policySet 资源类型
description: 包含用于 PolicySet 的属性的类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4e671d20c0beb8087fcc057a8f115350e0602812
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523983"
---
# <a name="policyset-resource-type"></a><span data-ttu-id="a766d-103">policySet 资源类型</span><span class="sxs-lookup"><span data-stu-id="a766d-103">policySet resource type</span></span>

<span data-ttu-id="a766d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a766d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a766d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a766d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a766d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a766d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a766d-107">包含用于 PolicySet 的属性的类。</span><span class="sxs-lookup"><span data-stu-id="a766d-107">A class containing the properties used for PolicySet.</span></span>

## <a name="methods"></a><span data-ttu-id="a766d-108">方法</span><span class="sxs-lookup"><span data-stu-id="a766d-108">Methods</span></span>
|<span data-ttu-id="a766d-109">方法</span><span class="sxs-lookup"><span data-stu-id="a766d-109">Method</span></span>|<span data-ttu-id="a766d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a766d-110">Return Type</span></span>|<span data-ttu-id="a766d-111">说明</span><span class="sxs-lookup"><span data-stu-id="a766d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a766d-112">列出 policySets</span><span class="sxs-lookup"><span data-stu-id="a766d-112">List policySets</span></span>](../api/intune-policyset-policyset-list.md)|<span data-ttu-id="a766d-113">[policySet](../resources/intune-policyset-policyset.md)集合</span><span class="sxs-lookup"><span data-stu-id="a766d-113">[policySet](../resources/intune-policyset-policyset.md) collection</span></span>|<span data-ttu-id="a766d-114">列出[policySet](../resources/intune-policyset-policyset.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a766d-114">List properties and relationships of the [policySet](../resources/intune-policyset-policyset.md) objects.</span></span>|
|[<span data-ttu-id="a766d-115">获取 policySet</span><span class="sxs-lookup"><span data-stu-id="a766d-115">Get policySet</span></span>](../api/intune-policyset-policyset-get.md)|[<span data-ttu-id="a766d-116">policySet</span><span class="sxs-lookup"><span data-stu-id="a766d-116">policySet</span></span>](../resources/intune-policyset-policyset.md)|<span data-ttu-id="a766d-117">读取[policySet](../resources/intune-policyset-policyset.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a766d-117">Read properties and relationships of the [policySet](../resources/intune-policyset-policyset.md) object.</span></span>|
|[<span data-ttu-id="a766d-118">创建 policySet</span><span class="sxs-lookup"><span data-stu-id="a766d-118">Create policySet</span></span>](../api/intune-policyset-policyset-create.md)|[<span data-ttu-id="a766d-119">policySet</span><span class="sxs-lookup"><span data-stu-id="a766d-119">policySet</span></span>](../resources/intune-policyset-policyset.md)|<span data-ttu-id="a766d-120">创建新的[policySet](../resources/intune-policyset-policyset.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a766d-120">Create a new [policySet](../resources/intune-policyset-policyset.md) object.</span></span>|
|[<span data-ttu-id="a766d-121">删除 policySet</span><span class="sxs-lookup"><span data-stu-id="a766d-121">Delete policySet</span></span>](../api/intune-policyset-policyset-delete.md)|<span data-ttu-id="a766d-122">无</span><span class="sxs-lookup"><span data-stu-id="a766d-122">None</span></span>|<span data-ttu-id="a766d-123">删除[policySet](../resources/intune-policyset-policyset.md)。</span><span class="sxs-lookup"><span data-stu-id="a766d-123">Deletes a [policySet](../resources/intune-policyset-policyset.md).</span></span>|
|[<span data-ttu-id="a766d-124">更新 policySet</span><span class="sxs-lookup"><span data-stu-id="a766d-124">Update policySet</span></span>](../api/intune-policyset-policyset-update.md)|[<span data-ttu-id="a766d-125">policySet</span><span class="sxs-lookup"><span data-stu-id="a766d-125">policySet</span></span>](../resources/intune-policyset-policyset.md)|<span data-ttu-id="a766d-126">更新[policySet](../resources/intune-policyset-policyset.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a766d-126">Update the properties of a [policySet](../resources/intune-policyset-policyset.md) object.</span></span>|
|[<span data-ttu-id="a766d-127">更新操作</span><span class="sxs-lookup"><span data-stu-id="a766d-127">update action</span></span>](../api/intune-policyset-policyset-update.md)|<span data-ttu-id="a766d-128">无</span><span class="sxs-lookup"><span data-stu-id="a766d-128">None</span></span>|<span data-ttu-id="a766d-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a766d-129">Not yet documented</span></span>|
|[<span data-ttu-id="a766d-130">getPolicySets 操作</span><span class="sxs-lookup"><span data-stu-id="a766d-130">getPolicySets action</span></span>](../api/intune-policyset-policyset-getpolicysets.md)|<span data-ttu-id="a766d-131">[policySet](../resources/intune-policyset-policyset.md)集合</span><span class="sxs-lookup"><span data-stu-id="a766d-131">[policySet](../resources/intune-policyset-policyset.md) collection</span></span>|<span data-ttu-id="a766d-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a766d-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a766d-133">属性</span><span class="sxs-lookup"><span data-stu-id="a766d-133">Properties</span></span>
|<span data-ttu-id="a766d-134">属性</span><span class="sxs-lookup"><span data-stu-id="a766d-134">Property</span></span>|<span data-ttu-id="a766d-135">类型</span><span class="sxs-lookup"><span data-stu-id="a766d-135">Type</span></span>|<span data-ttu-id="a766d-136">说明</span><span class="sxs-lookup"><span data-stu-id="a766d-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a766d-137">id</span><span class="sxs-lookup"><span data-stu-id="a766d-137">id</span></span>|<span data-ttu-id="a766d-138">字符串</span><span class="sxs-lookup"><span data-stu-id="a766d-138">String</span></span>|<span data-ttu-id="a766d-139">PolicySet 的键。</span><span class="sxs-lookup"><span data-stu-id="a766d-139">Key of the PolicySet.</span></span>|
|<span data-ttu-id="a766d-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a766d-140">createdDateTime</span></span>|<span data-ttu-id="a766d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a766d-141">DateTimeOffset</span></span>|<span data-ttu-id="a766d-142">PolicySet 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="a766d-142">Creation time of the PolicySet.</span></span>|
|<span data-ttu-id="a766d-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a766d-143">lastModifiedDateTime</span></span>|<span data-ttu-id="a766d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a766d-144">DateTimeOffset</span></span>|<span data-ttu-id="a766d-145">PolicySet 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="a766d-145">Last modified time of the PolicySet.</span></span>|
|<span data-ttu-id="a766d-146">displayName</span><span class="sxs-lookup"><span data-stu-id="a766d-146">displayName</span></span>|<span data-ttu-id="a766d-147">String</span><span class="sxs-lookup"><span data-stu-id="a766d-147">String</span></span>|<span data-ttu-id="a766d-148">PolicySet 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="a766d-148">DisplayName of the PolicySet.</span></span>|
|<span data-ttu-id="a766d-149">说明</span><span class="sxs-lookup"><span data-stu-id="a766d-149">description</span></span>|<span data-ttu-id="a766d-150">String</span><span class="sxs-lookup"><span data-stu-id="a766d-150">String</span></span>|<span data-ttu-id="a766d-151">PolicySet 的说明。</span><span class="sxs-lookup"><span data-stu-id="a766d-151">Description of the PolicySet.</span></span>|
|<span data-ttu-id="a766d-152">status</span><span class="sxs-lookup"><span data-stu-id="a766d-152">status</span></span>|[<span data-ttu-id="a766d-153">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="a766d-153">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="a766d-154">PolicySet 的验证/分配状态。</span><span class="sxs-lookup"><span data-stu-id="a766d-154">Validation/assignment status of the PolicySet.</span></span> <span data-ttu-id="a766d-155">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="a766d-155">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="a766d-156">errorCode</span><span class="sxs-lookup"><span data-stu-id="a766d-156">errorCode</span></span>|[<span data-ttu-id="a766d-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="a766d-157">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="a766d-158">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="a766d-158">Error code if any occured.</span></span> <span data-ttu-id="a766d-159">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="a766d-159">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="a766d-160">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="a766d-160">guidedDeploymentTags</span></span>|<span data-ttu-id="a766d-161">String 集合</span><span class="sxs-lookup"><span data-stu-id="a766d-161">String collection</span></span>|<span data-ttu-id="a766d-162">引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="a766d-162">Tags of the guided deployment</span></span>|
|<span data-ttu-id="a766d-163">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="a766d-163">roleScopeTags</span></span>|<span data-ttu-id="a766d-164">String 集合</span><span class="sxs-lookup"><span data-stu-id="a766d-164">String collection</span></span>|<span data-ttu-id="a766d-165">PolicySet 的 RoleScopeTags</span><span class="sxs-lookup"><span data-stu-id="a766d-165">RoleScopeTags of the PolicySet</span></span>|

## <a name="relationships"></a><span data-ttu-id="a766d-166">关系</span><span class="sxs-lookup"><span data-stu-id="a766d-166">Relationships</span></span>
|<span data-ttu-id="a766d-167">关系</span><span class="sxs-lookup"><span data-stu-id="a766d-167">Relationship</span></span>|<span data-ttu-id="a766d-168">类型</span><span class="sxs-lookup"><span data-stu-id="a766d-168">Type</span></span>|<span data-ttu-id="a766d-169">说明</span><span class="sxs-lookup"><span data-stu-id="a766d-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a766d-170">assignments</span><span class="sxs-lookup"><span data-stu-id="a766d-170">assignments</span></span>|<span data-ttu-id="a766d-171">[policySetAssignment](../resources/intune-policyset-policysetassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="a766d-171">[policySetAssignment](../resources/intune-policyset-policysetassignment.md) collection</span></span>|<span data-ttu-id="a766d-172">PolicySet 的分配。</span><span class="sxs-lookup"><span data-stu-id="a766d-172">Assignments of the PolicySet.</span></span>|
|<span data-ttu-id="a766d-173">items</span><span class="sxs-lookup"><span data-stu-id="a766d-173">items</span></span>|<span data-ttu-id="a766d-174">[policySetItem](../resources/intune-policyset-policysetitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="a766d-174">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="a766d-175">PolicySet 的项目，最大计数为100。</span><span class="sxs-lookup"><span data-stu-id="a766d-175">Items of the PolicySet with maximum count 100.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a766d-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a766d-176">JSON Representation</span></span>
<span data-ttu-id="a766d-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a766d-177">Here is a JSON representation of the resource.</span></span>
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



