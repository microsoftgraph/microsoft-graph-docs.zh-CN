---
title: ediscoveryCase 资源类型
description: 电子数据展示事例是包含保管人、保留、集合、审阅集和导出的容器。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 8fac6cfa8de0533c936c9d8d03a6173f06d0886f
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404789"
---
# <a name="ediscoverycase-resource-type"></a><span data-ttu-id="90a7d-103">ediscoveryCase 资源类型</span><span class="sxs-lookup"><span data-stu-id="90a7d-103">ediscoveryCase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90a7d-104">电子数据展示事例是包含保管人、保留、集合、审阅集和导出的容器。</span><span class="sxs-lookup"><span data-stu-id="90a7d-104">eDiscovery cases are containers that contain custodians, holds, collections, review sets, and exports.</span></span>  <span data-ttu-id="90a7d-105">了解有关案例和 [高级电子数据展示](/microsoft-365/compliance/overview-ediscovery-20)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="90a7d-105">Learn more about cases and [Advanced eDiscovery](/microsoft-365/compliance/overview-ediscovery-20).</span></span>

## <a name="methods"></a><span data-ttu-id="90a7d-106">方法</span><span class="sxs-lookup"><span data-stu-id="90a7d-106">Methods</span></span>

| <span data-ttu-id="90a7d-107">方法</span><span class="sxs-lookup"><span data-stu-id="90a7d-107">Method</span></span>       | <span data-ttu-id="90a7d-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="90a7d-108">Return Type</span></span> | <span data-ttu-id="90a7d-109">Description</span><span class="sxs-lookup"><span data-stu-id="90a7d-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="90a7d-110">List</span><span class="sxs-lookup"><span data-stu-id="90a7d-110">List</span></span>](../api/ediscoverycase-list.md) | <span data-ttu-id="90a7d-111">[ediscoveryCase](ediscoverycase.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90a7d-111">[ediscoveryCase](ediscoverycase.md) collection</span></span> | <span data-ttu-id="90a7d-112">获取电子数据展示事例的列表。</span><span class="sxs-lookup"><span data-stu-id="90a7d-112">Get a list of eDiscovery cases.</span></span>|
| [<span data-ttu-id="90a7d-113">获取</span><span class="sxs-lookup"><span data-stu-id="90a7d-113">Get</span></span>](../api/ediscoverycase-get.md) | [<span data-ttu-id="90a7d-114">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="90a7d-114">ediscoveryCase</span></span>](ediscoverycase.md) | <span data-ttu-id="90a7d-115">阅读电子数据展示事例属性。</span><span class="sxs-lookup"><span data-stu-id="90a7d-115">Read eDiscovery case properties.</span></span> |
| [<span data-ttu-id="90a7d-116">创建</span><span class="sxs-lookup"><span data-stu-id="90a7d-116">Create</span></span>](../api/ediscoverycase-post.md) | [<span data-ttu-id="90a7d-117">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="90a7d-117">ediscoveryCase</span></span>](ediscoverycase.md) | <span data-ttu-id="90a7d-118">通过发布到事例集合创建新的 **ediscoveryCase** 。</span><span class="sxs-lookup"><span data-stu-id="90a7d-118">Create a new **ediscoveryCase** by posting to the cases collection.</span></span> |
| [<span data-ttu-id="90a7d-119">更新</span><span class="sxs-lookup"><span data-stu-id="90a7d-119">Update</span></span>](../api/ediscoverycase-update.md) | [<span data-ttu-id="90a7d-120">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="90a7d-120">ediscoveryCase</span></span>](ediscoverycase.md) | <span data-ttu-id="90a7d-121">更新电子数据展示事例。</span><span class="sxs-lookup"><span data-stu-id="90a7d-121">Update an eDiscovery case.</span></span> |
| [<span data-ttu-id="90a7d-122">删除</span><span class="sxs-lookup"><span data-stu-id="90a7d-122">Delete</span></span>](../api/ediscoverycase-delete.md) | <span data-ttu-id="90a7d-123">无</span><span class="sxs-lookup"><span data-stu-id="90a7d-123">None</span></span> | <span data-ttu-id="90a7d-124">删除电子数据展示事例。</span><span class="sxs-lookup"><span data-stu-id="90a7d-124">Delete an eDiscovery case.</span></span> |

## <a name="properties"></a><span data-ttu-id="90a7d-125">属性</span><span class="sxs-lookup"><span data-stu-id="90a7d-125">Properties</span></span>

| <span data-ttu-id="90a7d-126">属性</span><span class="sxs-lookup"><span data-stu-id="90a7d-126">Property</span></span>     | <span data-ttu-id="90a7d-127">类型</span><span class="sxs-lookup"><span data-stu-id="90a7d-127">Type</span></span>        | <span data-ttu-id="90a7d-128">说明</span><span class="sxs-lookup"><span data-stu-id="90a7d-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="90a7d-129">closedBy</span><span class="sxs-lookup"><span data-stu-id="90a7d-129">closedBy</span></span>|[<span data-ttu-id="90a7d-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="90a7d-130">identitySet</span></span>](/graph/api/resources/identityset)|<span data-ttu-id="90a7d-131">关闭该事例的用户。</span><span class="sxs-lookup"><span data-stu-id="90a7d-131">The user who closed the case.</span></span>|
|<span data-ttu-id="90a7d-132">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="90a7d-132">closedDateTime</span></span>|<span data-ttu-id="90a7d-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90a7d-133">DateTimeOffset</span></span>|<span data-ttu-id="90a7d-134">关闭事例的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="90a7d-134">The date and time when the case was closed.</span></span> <span data-ttu-id="90a7d-135">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="90a7d-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="90a7d-136">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="90a7d-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="90a7d-137">createdBy</span><span class="sxs-lookup"><span data-stu-id="90a7d-137">createdBy</span></span>|[<span data-ttu-id="90a7d-138">identitySet</span><span class="sxs-lookup"><span data-stu-id="90a7d-138">identitySet</span></span>](/graph/api/resources/identityset)|<span data-ttu-id="90a7d-139">创建案例的用户。</span><span class="sxs-lookup"><span data-stu-id="90a7d-139">The user who created the case.</span></span>|
|<span data-ttu-id="90a7d-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90a7d-140">createdDateTime</span></span>|<span data-ttu-id="90a7d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90a7d-141">DateTimeOffset</span></span>|<span data-ttu-id="90a7d-142">实体的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="90a7d-142">The date and time when the entity was created.</span></span> <span data-ttu-id="90a7d-143">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="90a7d-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="90a7d-144">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="90a7d-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="90a7d-145">说明</span><span class="sxs-lookup"><span data-stu-id="90a7d-145">description</span></span>|<span data-ttu-id="90a7d-146">字符串</span><span class="sxs-lookup"><span data-stu-id="90a7d-146">String</span></span>|<span data-ttu-id="90a7d-147">事例说明。</span><span class="sxs-lookup"><span data-stu-id="90a7d-147">The case description.</span></span>|
|<span data-ttu-id="90a7d-148">displayName</span><span class="sxs-lookup"><span data-stu-id="90a7d-148">displayName</span></span>|<span data-ttu-id="90a7d-149">字符串</span><span class="sxs-lookup"><span data-stu-id="90a7d-149">String</span></span>|<span data-ttu-id="90a7d-150">事例名称。</span><span class="sxs-lookup"><span data-stu-id="90a7d-150">The case name.</span></span>|
|<span data-ttu-id="90a7d-151">externalId</span><span class="sxs-lookup"><span data-stu-id="90a7d-151">externalId</span></span>|<span data-ttu-id="90a7d-152">String</span><span class="sxs-lookup"><span data-stu-id="90a7d-152">String</span></span>|<span data-ttu-id="90a7d-153">Customer reference 的外部事例编号。</span><span class="sxs-lookup"><span data-stu-id="90a7d-153">The external case number for customer reference.</span></span>|
|<span data-ttu-id="90a7d-154">id</span><span class="sxs-lookup"><span data-stu-id="90a7d-154">id</span></span>|<span data-ttu-id="90a7d-155">字符串</span><span class="sxs-lookup"><span data-stu-id="90a7d-155">String</span></span>| <span data-ttu-id="90a7d-156">电子数据展示事例的 ID。</span><span class="sxs-lookup"><span data-stu-id="90a7d-156">The ID for the eDiscovery case.</span></span> <span data-ttu-id="90a7d-157">只读。</span><span class="sxs-lookup"><span data-stu-id="90a7d-157">Read-only.</span></span> |
|<span data-ttu-id="90a7d-158">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="90a7d-158">lastModifiedBy</span></span>|[<span data-ttu-id="90a7d-159">identitySet</span><span class="sxs-lookup"><span data-stu-id="90a7d-159">identitySet</span></span>](/graph/api/resources/identityset)|<span data-ttu-id="90a7d-160">上次修改实体的用户。</span><span class="sxs-lookup"><span data-stu-id="90a7d-160">The last user who modified the entity.</span></span>|
|<span data-ttu-id="90a7d-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90a7d-161">lastModifiedDateTime</span></span>|<span data-ttu-id="90a7d-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90a7d-162">DateTimeOffset</span></span>| <span data-ttu-id="90a7d-163">修改事例的最新日期和时间。</span><span class="sxs-lookup"><span data-stu-id="90a7d-163">The latest date and time when the case was modified.</span></span> <span data-ttu-id="90a7d-164">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="90a7d-164">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="90a7d-165">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="90a7d-165">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="90a7d-166">状态</span><span class="sxs-lookup"><span data-stu-id="90a7d-166">status</span></span>|<span data-ttu-id="90a7d-167">字符串</span><span class="sxs-lookup"><span data-stu-id="90a7d-167">String</span></span>| <span data-ttu-id="90a7d-168">案例状态。</span><span class="sxs-lookup"><span data-stu-id="90a7d-168">The case status.</span></span> <span data-ttu-id="90a7d-169">可能的值为、、、、 `unknown` `active` `pendingDelete` `closing` `closed` 和 `closedWithError` 。</span><span class="sxs-lookup"><span data-stu-id="90a7d-169">Possible values are `unknown`, `active`, `pendingDelete`, `closing`, `closed`, and `closedWithError`.</span></span> <span data-ttu-id="90a7d-170">有关详细信息，请参阅下表。</span><span class="sxs-lookup"><span data-stu-id="90a7d-170">For details see the following table.</span></span>|

### <a name="casestatus-values"></a><span data-ttu-id="90a7d-171">caseStatus 值</span><span class="sxs-lookup"><span data-stu-id="90a7d-171">caseStatus values</span></span>

|<span data-ttu-id="90a7d-172">成员</span><span class="sxs-lookup"><span data-stu-id="90a7d-172">Member</span></span>|<span data-ttu-id="90a7d-173">说明</span><span class="sxs-lookup"><span data-stu-id="90a7d-173">Description</span></span>|
|:----|-----------|
| <span data-ttu-id="90a7d-174">unknown</span><span class="sxs-lookup"><span data-stu-id="90a7d-174">unknown</span></span> | <span data-ttu-id="90a7d-175">未知的案例状态。</span><span class="sxs-lookup"><span data-stu-id="90a7d-175">Case status is unknown.</span></span> |
| <span data-ttu-id="90a7d-176">工作</span><span class="sxs-lookup"><span data-stu-id="90a7d-176">active</span></span> | <span data-ttu-id="90a7d-177">案例处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="90a7d-177">Case is active.</span></span> |
| <span data-ttu-id="90a7d-178">pendingDelete</span><span class="sxs-lookup"><span data-stu-id="90a7d-178">pendingDelete</span></span> | <span data-ttu-id="90a7d-179">已删除事例，但尚未完全处理该删除。</span><span class="sxs-lookup"><span data-stu-id="90a7d-179">Case was deleted, but the delete has not been fully transacted.</span></span> |
| <span data-ttu-id="90a7d-180">结束语</span><span class="sxs-lookup"><span data-stu-id="90a7d-180">closing</span></span> | <span data-ttu-id="90a7d-181">事例已关闭，但操作尚未完全进行事务处理。</span><span class="sxs-lookup"><span data-stu-id="90a7d-181">Case was closed, but the operation has not been fully transacted.</span></span> |
| <span data-ttu-id="90a7d-182">停止</span><span class="sxs-lookup"><span data-stu-id="90a7d-182">closed</span></span> | <span data-ttu-id="90a7d-183">事例已关闭。</span><span class="sxs-lookup"><span data-stu-id="90a7d-183">The case is closed.</span></span> |
| <span data-ttu-id="90a7d-184">closedWithError</span><span class="sxs-lookup"><span data-stu-id="90a7d-184">closedWithError</span></span> | <span data-ttu-id="90a7d-185">事例已关闭，但在这种情况下释放保留时出现错误。</span><span class="sxs-lookup"><span data-stu-id="90a7d-185">The case is closed, but there were errors releasing holds in the case.</span></span> |

## <a name="relationships"></a><span data-ttu-id="90a7d-186">关系</span><span class="sxs-lookup"><span data-stu-id="90a7d-186">Relationships</span></span>

| <span data-ttu-id="90a7d-187">关系</span><span class="sxs-lookup"><span data-stu-id="90a7d-187">Relationship</span></span> | <span data-ttu-id="90a7d-188">类型</span><span class="sxs-lookup"><span data-stu-id="90a7d-188">Type</span></span>        | <span data-ttu-id="90a7d-189">说明</span><span class="sxs-lookup"><span data-stu-id="90a7d-189">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="90a7d-190">评审集</span><span class="sxs-lookup"><span data-stu-id="90a7d-190">Review sets</span></span>|<span data-ttu-id="90a7d-191">[reviewSet](reviewset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90a7d-191">[reviewSet](reviewset.md) collection</span></span>| <span data-ttu-id="90a7d-192">案例中的审阅集集合。</span><span class="sxs-lookup"><span data-stu-id="90a7d-192">Collection of review sets in the case.</span></span> <span data-ttu-id="90a7d-193">只读。</span><span class="sxs-lookup"><span data-stu-id="90a7d-193">Read-only.</span></span> <span data-ttu-id="90a7d-194">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="90a7d-194">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="90a7d-195">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90a7d-195">JSON representation</span></span>

<span data-ttu-id="90a7d-196">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90a7d-196">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
 
  ],
  "@odata.type": "microsoft.graph.ediscoveryCase"
}-->

```json
{
  "closedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "closedDateTime": "String (timestamp)",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "id": "String (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "status": "string"
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