---
title: ediscoveryCase 资源类型
description: 电子数据展示事例是包含保管人、保留、集合、审阅集和导出的容器。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 12d2901ff6a61213affd14d681c0ec7b6a74470c
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597401"
---
# <a name="ediscoverycase-resource-type"></a><span data-ttu-id="d876e-103">ediscoveryCase 资源类型</span><span class="sxs-lookup"><span data-stu-id="d876e-103">ediscoveryCase resource type</span></span>

<span data-ttu-id="d876e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d876e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d876e-105">电子数据展示事例是包含保管人、保留、集合、审阅集和导出的容器。</span><span class="sxs-lookup"><span data-stu-id="d876e-105">eDiscovery cases are containers that contain custodians, holds, collections, review sets, and exports.</span></span>  <span data-ttu-id="d876e-106">了解有关案例和 [高级电子数据展示](/microsoft-365/compliance/overview-ediscovery-20)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d876e-106">Learn more about cases and [Advanced eDiscovery](/microsoft-365/compliance/overview-ediscovery-20).</span></span>

## <a name="methods"></a><span data-ttu-id="d876e-107">方法</span><span class="sxs-lookup"><span data-stu-id="d876e-107">Methods</span></span>

| <span data-ttu-id="d876e-108">方法</span><span class="sxs-lookup"><span data-stu-id="d876e-108">Method</span></span>       | <span data-ttu-id="d876e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d876e-109">Return Type</span></span> | <span data-ttu-id="d876e-110">Description</span><span class="sxs-lookup"><span data-stu-id="d876e-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d876e-111">列出 ediscoveryCases</span><span class="sxs-lookup"><span data-stu-id="d876e-111">List ediscoveryCases</span></span>](../api/ediscoverycase-list.md)          | <span data-ttu-id="d876e-112">[ediscoveryCase](ediscoverycase.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d876e-112">[ediscoveryCase](ediscoverycase.md) collection</span></span>   | <span data-ttu-id="d876e-113">获取电子数据展示事例的列表。</span><span class="sxs-lookup"><span data-stu-id="d876e-113">Get a list of eDiscovery cases.</span></span>|
| [<span data-ttu-id="d876e-114">获取 ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="d876e-114">Get ediscoveryCase</span></span>](../api/ediscoverycase-get.md)            | [<span data-ttu-id="d876e-115">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="d876e-115">ediscoveryCase</span></span>](ediscoverycase.md)               | <span data-ttu-id="d876e-116">阅读电子数据展示事例属性。</span><span class="sxs-lookup"><span data-stu-id="d876e-116">Read eDiscovery case properties.</span></span> |
| [<span data-ttu-id="d876e-117">创建 ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="d876e-117">Create ediscoveryCase</span></span>](../api/ediscoverycase-post.md)        | [<span data-ttu-id="d876e-118">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="d876e-118">ediscoveryCase</span></span>](ediscoverycase.md)               | <span data-ttu-id="d876e-119">通过发布到事例集合创建新的 **ediscoveryCase** 。</span><span class="sxs-lookup"><span data-stu-id="d876e-119">Create a new **ediscoveryCase** by posting to the cases collection.</span></span> |
| [<span data-ttu-id="d876e-120">更新 ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="d876e-120">Update ediscoveryCase</span></span>](../api/ediscoverycase-update.md)      | [<span data-ttu-id="d876e-121">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="d876e-121">ediscoveryCase</span></span>](ediscoverycase.md)               | <span data-ttu-id="d876e-122">更新电子数据展示事例。</span><span class="sxs-lookup"><span data-stu-id="d876e-122">Update an eDiscovery case.</span></span> |
| [<span data-ttu-id="d876e-123">删除 ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="d876e-123">Delete ediscoveryCase</span></span>](../api/ediscoverycase-delete.md)      | <span data-ttu-id="d876e-124">无</span><span class="sxs-lookup"><span data-stu-id="d876e-124">None</span></span>                                              | <span data-ttu-id="d876e-125">删除电子数据展示事例。</span><span class="sxs-lookup"><span data-stu-id="d876e-125">Delete an eDiscovery case.</span></span> |
| [<span data-ttu-id="d876e-126">关闭 ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="d876e-126">Close ediscoveryCase</span></span>](../api/ediscoverycase-close.md)        | <span data-ttu-id="d876e-127">无</span><span class="sxs-lookup"><span data-stu-id="d876e-127">None</span></span>                                              | <span data-ttu-id="d876e-128">关闭电子数据展示事例。</span><span class="sxs-lookup"><span data-stu-id="d876e-128">Close an eDiscovery case.</span></span> |
| [<span data-ttu-id="d876e-129">重新打开 ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="d876e-129">Reopen ediscoveryCase</span></span>](../api/ediscoverycase-reopen.md)      | <span data-ttu-id="d876e-130">无</span><span class="sxs-lookup"><span data-stu-id="d876e-130">None</span></span>                                              | <span data-ttu-id="d876e-131">重新打开已关闭的电子数据展示事例。</span><span class="sxs-lookup"><span data-stu-id="d876e-131">Reopen a closed eDiscovery case.</span></span>|
| [<span data-ttu-id="d876e-132">列出保管人</span><span class="sxs-lookup"><span data-stu-id="d876e-132">List custodians</span></span>](../api/custodian-get.md)   | <span data-ttu-id="d876e-133">[保管人](../resources/custodian.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d876e-133">[custodian](../resources/custodian.md) collection</span></span> |<span data-ttu-id="d876e-134">从保管人导航属性中获取保管人资源。</span><span class="sxs-lookup"><span data-stu-id="d876e-134">Get the custodian resources from the custodians navigation property.</span></span>|
| [<span data-ttu-id="d876e-135">创建保管人</span><span class="sxs-lookup"><span data-stu-id="d876e-135">Create custodians</span></span>](../api/ediscoverycase-post-custodians.md)  | [<span data-ttu-id="d876e-136">保管人</span><span class="sxs-lookup"><span data-stu-id="d876e-136">custodian</span></span>](../resources/custodian.md)           |<span data-ttu-id="d876e-137">创建新的保管人对象。</span><span class="sxs-lookup"><span data-stu-id="d876e-137">Create a new custodian object.</span></span>|
| [<span data-ttu-id="d876e-138">列出 reviewSets</span><span class="sxs-lookup"><span data-stu-id="d876e-138">List reviewSets</span></span>](../api/reviewset-list.md)   | <span data-ttu-id="d876e-139">[reviewSet](../resources/reviewset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d876e-139">[reviewSet](../resources/reviewset.md) collection</span></span> | <span data-ttu-id="d876e-140">从 reviewSets 导航属性中获取 reviewSet 资源。</span><span class="sxs-lookup"><span data-stu-id="d876e-140">Get the reviewSet resources from the reviewSets navigation property.</span></span>|
| [<span data-ttu-id="d876e-141">创建 reviewSets</span><span class="sxs-lookup"><span data-stu-id="d876e-141">Create reviewSets</span></span>](../api/reviewset-post.md)  | [<span data-ttu-id="d876e-142">reviewSet</span><span class="sxs-lookup"><span data-stu-id="d876e-142">reviewSet</span></span>](../resources/reviewset.md)           | <span data-ttu-id="d876e-143">创建新的 reviewSet 对象。</span><span class="sxs-lookup"><span data-stu-id="d876e-143">Create a new reviewSet object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d876e-144">属性</span><span class="sxs-lookup"><span data-stu-id="d876e-144">Properties</span></span>

| <span data-ttu-id="d876e-145">属性</span><span class="sxs-lookup"><span data-stu-id="d876e-145">Property</span></span>     | <span data-ttu-id="d876e-146">类型</span><span class="sxs-lookup"><span data-stu-id="d876e-146">Type</span></span>        | <span data-ttu-id="d876e-147">Description</span><span class="sxs-lookup"><span data-stu-id="d876e-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d876e-148">closedBy</span><span class="sxs-lookup"><span data-stu-id="d876e-148">closedBy</span></span>|[<span data-ttu-id="d876e-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="d876e-149">identitySet</span></span>](/graph/api/resources/identityset)|<span data-ttu-id="d876e-150">关闭该事例的用户。</span><span class="sxs-lookup"><span data-stu-id="d876e-150">The user who closed the case.</span></span>|
|<span data-ttu-id="d876e-151">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="d876e-151">closedDateTime</span></span>|<span data-ttu-id="d876e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d876e-152">DateTimeOffset</span></span>|<span data-ttu-id="d876e-153">关闭事例的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d876e-153">The date and time when the case was closed.</span></span> <span data-ttu-id="d876e-154">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="d876e-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d876e-155">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d876e-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d876e-156">createdBy</span><span class="sxs-lookup"><span data-stu-id="d876e-156">createdBy</span></span>|[<span data-ttu-id="d876e-157">identitySet</span><span class="sxs-lookup"><span data-stu-id="d876e-157">identitySet</span></span>](/graph/api/resources/identityset)|<span data-ttu-id="d876e-158">创建案例的用户。</span><span class="sxs-lookup"><span data-stu-id="d876e-158">The user who created the case.</span></span>|
|<span data-ttu-id="d876e-159">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d876e-159">createdDateTime</span></span>|<span data-ttu-id="d876e-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d876e-160">DateTimeOffset</span></span>|<span data-ttu-id="d876e-161">实体的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d876e-161">The date and time when the entity was created.</span></span> <span data-ttu-id="d876e-162">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="d876e-162">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d876e-163">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d876e-163">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d876e-164">说明</span><span class="sxs-lookup"><span data-stu-id="d876e-164">description</span></span>|<span data-ttu-id="d876e-165">String</span><span class="sxs-lookup"><span data-stu-id="d876e-165">String</span></span>|<span data-ttu-id="d876e-166">事例说明。</span><span class="sxs-lookup"><span data-stu-id="d876e-166">The case description.</span></span>|
|<span data-ttu-id="d876e-167">displayName</span><span class="sxs-lookup"><span data-stu-id="d876e-167">displayName</span></span>|<span data-ttu-id="d876e-168">String</span><span class="sxs-lookup"><span data-stu-id="d876e-168">String</span></span>|<span data-ttu-id="d876e-169">事例名称。</span><span class="sxs-lookup"><span data-stu-id="d876e-169">The case name.</span></span>|
|<span data-ttu-id="d876e-170">externalId</span><span class="sxs-lookup"><span data-stu-id="d876e-170">externalId</span></span>|<span data-ttu-id="d876e-171">String</span><span class="sxs-lookup"><span data-stu-id="d876e-171">String</span></span>|<span data-ttu-id="d876e-172">Customer reference 的外部事例编号。</span><span class="sxs-lookup"><span data-stu-id="d876e-172">The external case number for customer reference.</span></span>|
|<span data-ttu-id="d876e-173">id</span><span class="sxs-lookup"><span data-stu-id="d876e-173">id</span></span>|<span data-ttu-id="d876e-174">String</span><span class="sxs-lookup"><span data-stu-id="d876e-174">String</span></span>| <span data-ttu-id="d876e-175">电子数据展示事例的 ID。</span><span class="sxs-lookup"><span data-stu-id="d876e-175">The ID for the eDiscovery case.</span></span> <span data-ttu-id="d876e-176">只读。</span><span class="sxs-lookup"><span data-stu-id="d876e-176">Read-only.</span></span> |
|<span data-ttu-id="d876e-177">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d876e-177">lastModifiedBy</span></span>|[<span data-ttu-id="d876e-178">identitySet</span><span class="sxs-lookup"><span data-stu-id="d876e-178">identitySet</span></span>](/graph/api/resources/identityset)|<span data-ttu-id="d876e-179">上次修改实体的用户。</span><span class="sxs-lookup"><span data-stu-id="d876e-179">The last user who modified the entity.</span></span>|
|<span data-ttu-id="d876e-180">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d876e-180">lastModifiedDateTime</span></span>|<span data-ttu-id="d876e-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d876e-181">DateTimeOffset</span></span>| <span data-ttu-id="d876e-182">修改事例的最新日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d876e-182">The latest date and time when the case was modified.</span></span> <span data-ttu-id="d876e-183">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="d876e-183">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d876e-184">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d876e-184">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d876e-185">status</span><span class="sxs-lookup"><span data-stu-id="d876e-185">status</span></span>|<span data-ttu-id="d876e-186">String</span><span class="sxs-lookup"><span data-stu-id="d876e-186">String</span></span>| <span data-ttu-id="d876e-187">案例状态。</span><span class="sxs-lookup"><span data-stu-id="d876e-187">The case status.</span></span> <span data-ttu-id="d876e-188">可能的值为、、、、 `unknown` `active` `pendingDelete` `closing` `closed` 和 `closedWithError` 。</span><span class="sxs-lookup"><span data-stu-id="d876e-188">Possible values are `unknown`, `active`, `pendingDelete`, `closing`, `closed`, and `closedWithError`.</span></span> <span data-ttu-id="d876e-189">有关详细信息，请参阅下表。</span><span class="sxs-lookup"><span data-stu-id="d876e-189">For details see the following table.</span></span>|

### <a name="casestatus-values"></a><span data-ttu-id="d876e-190">caseStatus 值</span><span class="sxs-lookup"><span data-stu-id="d876e-190">caseStatus values</span></span>

|<span data-ttu-id="d876e-191">成员</span><span class="sxs-lookup"><span data-stu-id="d876e-191">Member</span></span>|<span data-ttu-id="d876e-192">说明</span><span class="sxs-lookup"><span data-stu-id="d876e-192">Description</span></span>|
|:----|-----------|
| <span data-ttu-id="d876e-193">unknown</span><span class="sxs-lookup"><span data-stu-id="d876e-193">unknown</span></span> | <span data-ttu-id="d876e-194">未知的案例状态。</span><span class="sxs-lookup"><span data-stu-id="d876e-194">Case status is unknown.</span></span> |
| <span data-ttu-id="d876e-195">工作</span><span class="sxs-lookup"><span data-stu-id="d876e-195">active</span></span> | <span data-ttu-id="d876e-196">案例处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="d876e-196">Case is active.</span></span> |
| <span data-ttu-id="d876e-197">pendingDelete</span><span class="sxs-lookup"><span data-stu-id="d876e-197">pendingDelete</span></span> | <span data-ttu-id="d876e-198">已删除事例，但尚未完全处理该删除。</span><span class="sxs-lookup"><span data-stu-id="d876e-198">Case was deleted, but the delete has not been fully transacted.</span></span> |
| <span data-ttu-id="d876e-199">结束语</span><span class="sxs-lookup"><span data-stu-id="d876e-199">closing</span></span> | <span data-ttu-id="d876e-200">事例已关闭，但操作尚未完全进行事务处理。</span><span class="sxs-lookup"><span data-stu-id="d876e-200">Case was closed, but the operation has not been fully transacted.</span></span> |
| <span data-ttu-id="d876e-201">停止</span><span class="sxs-lookup"><span data-stu-id="d876e-201">closed</span></span> | <span data-ttu-id="d876e-202">事例已关闭。</span><span class="sxs-lookup"><span data-stu-id="d876e-202">The case is closed.</span></span> |
| <span data-ttu-id="d876e-203">closedWithError</span><span class="sxs-lookup"><span data-stu-id="d876e-203">closedWithError</span></span> | <span data-ttu-id="d876e-204">事例已关闭，但在这种情况下释放保留时出现错误。</span><span class="sxs-lookup"><span data-stu-id="d876e-204">The case is closed, but there were errors releasing holds in the case.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d876e-205">关系</span><span class="sxs-lookup"><span data-stu-id="d876e-205">Relationships</span></span>

| <span data-ttu-id="d876e-206">关系</span><span class="sxs-lookup"><span data-stu-id="d876e-206">Relationship</span></span> | <span data-ttu-id="d876e-207">类型</span><span class="sxs-lookup"><span data-stu-id="d876e-207">Type</span></span>        | <span data-ttu-id="d876e-208">Description</span><span class="sxs-lookup"><span data-stu-id="d876e-208">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d876e-209">保管人</span><span class="sxs-lookup"><span data-stu-id="d876e-209">custodians</span></span>|<span data-ttu-id="d876e-210">[保管人](../resources/custodian.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d876e-210">[custodian](../resources/custodian.md) collection</span></span>| <span data-ttu-id="d876e-211">组织中可能拥有与案例相关的数据的人员。</span><span class="sxs-lookup"><span data-stu-id="d876e-211">People in an organization who may possess data relevant to the case.</span></span> |
|<span data-ttu-id="d876e-212">reviewSets</span><span class="sxs-lookup"><span data-stu-id="d876e-212">reviewSets</span></span>|<span data-ttu-id="d876e-213">[reviewSet](reviewset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d876e-213">[reviewSet](reviewset.md) collection</span></span>| <span data-ttu-id="d876e-214">案例中的审阅集集合。</span><span class="sxs-lookup"><span data-stu-id="d876e-214">Collection of review sets in the case.</span></span> <span data-ttu-id="d876e-215">只读。</span><span class="sxs-lookup"><span data-stu-id="d876e-215">Read-only.</span></span> <span data-ttu-id="d876e-216">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d876e-216">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d876e-217">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d876e-217">JSON representation</span></span>

<span data-ttu-id="d876e-218">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d876e-218">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
 
  ],
  "@odata.type": "microsoft.graph.ediscoveryCase"
}-->

```json
{
  "@odata.type": "#microsoft.graph.ediscoveryCase",
  "description": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "closedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "closedDateTime": "String (timestamp)",
  "externalId": "String",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ediscoveryCase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
