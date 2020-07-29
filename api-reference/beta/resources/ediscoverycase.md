---
title: ediscoveryCase 资源类型
description: 电子数据展示事例是包含保管人、保留、集合、审阅集和导出的容器。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 930d04449f24d05d8c9225869506bfc1ed2720aa
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510025"
---
# <a name="ediscoverycase-resource-type"></a><span data-ttu-id="f7958-103">ediscoveryCase 资源类型</span><span class="sxs-lookup"><span data-stu-id="f7958-103">ediscoveryCase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7958-104">电子数据展示事例是包含保管人、保留、集合、审阅集和导出的容器。</span><span class="sxs-lookup"><span data-stu-id="f7958-104">eDiscovery cases are containers that contain custodians, holds, collections, review sets, and exports.</span></span>  <span data-ttu-id="f7958-105">了解有关案例和[高级电子数据展示](https://docs.microsoft.com/microsoft-365/compliance/overview-ediscovery-20)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f7958-105">Learn more about cases and [Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/overview-ediscovery-20).</span></span>

## <a name="methods"></a><span data-ttu-id="f7958-106">方法</span><span class="sxs-lookup"><span data-stu-id="f7958-106">Methods</span></span>

| <span data-ttu-id="f7958-107">方法</span><span class="sxs-lookup"><span data-stu-id="f7958-107">Method</span></span>       | <span data-ttu-id="f7958-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f7958-108">Return Type</span></span> | <span data-ttu-id="f7958-109">说明</span><span class="sxs-lookup"><span data-stu-id="f7958-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f7958-110">List</span><span class="sxs-lookup"><span data-stu-id="f7958-110">List</span></span>](../api/ediscoverycase-list.md) | <span data-ttu-id="f7958-111">[ediscoveryCase](ediscoverycase.md)集合</span><span class="sxs-lookup"><span data-stu-id="f7958-111">[ediscoveryCase](ediscoverycase.md) collection</span></span> | <span data-ttu-id="f7958-112">获取电子数据展示事例的列表。</span><span class="sxs-lookup"><span data-stu-id="f7958-112">Get a list of eDiscovery cases.</span></span>|
| [<span data-ttu-id="f7958-113">获取</span><span class="sxs-lookup"><span data-stu-id="f7958-113">Get</span></span>](../api/ediscoverycase-get.md) | [<span data-ttu-id="f7958-114">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="f7958-114">ediscoveryCase</span></span>](ediscoverycase.md) | <span data-ttu-id="f7958-115">阅读电子数据展示事例属性。</span><span class="sxs-lookup"><span data-stu-id="f7958-115">Read eDiscovery case properties.</span></span> |
| [<span data-ttu-id="f7958-116">创建</span><span class="sxs-lookup"><span data-stu-id="f7958-116">Create</span></span>](../api/ediscoverycase-post.md) | [<span data-ttu-id="f7958-117">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="f7958-117">ediscoveryCase</span></span>](ediscoverycase.md) | <span data-ttu-id="f7958-118">通过发布到事例集合创建新的**ediscoveryCase** 。</span><span class="sxs-lookup"><span data-stu-id="f7958-118">Create a new **ediscoveryCase** by posting to the cases collection.</span></span> |
| [<span data-ttu-id="f7958-119">更新</span><span class="sxs-lookup"><span data-stu-id="f7958-119">Update</span></span>](../api/ediscoverycase-update.md) | [<span data-ttu-id="f7958-120">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="f7958-120">ediscoveryCase</span></span>](ediscoverycase.md) | <span data-ttu-id="f7958-121">更新电子数据展示事例。</span><span class="sxs-lookup"><span data-stu-id="f7958-121">Update an eDiscovery case.</span></span> |
| [<span data-ttu-id="f7958-122">删除</span><span class="sxs-lookup"><span data-stu-id="f7958-122">Delete</span></span>](../api/ediscoverycase-delete.md) | <span data-ttu-id="f7958-123">无</span><span class="sxs-lookup"><span data-stu-id="f7958-123">None</span></span> | <span data-ttu-id="f7958-124">删除电子数据展示事例。</span><span class="sxs-lookup"><span data-stu-id="f7958-124">Delete an eDiscovery case.</span></span> |

## <a name="properties"></a><span data-ttu-id="f7958-125">属性</span><span class="sxs-lookup"><span data-stu-id="f7958-125">Properties</span></span>

| <span data-ttu-id="f7958-126">属性</span><span class="sxs-lookup"><span data-stu-id="f7958-126">Property</span></span>     | <span data-ttu-id="f7958-127">类型</span><span class="sxs-lookup"><span data-stu-id="f7958-127">Type</span></span>        | <span data-ttu-id="f7958-128">说明</span><span class="sxs-lookup"><span data-stu-id="f7958-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f7958-129">closedBy</span><span class="sxs-lookup"><span data-stu-id="f7958-129">closedBy</span></span>|[<span data-ttu-id="f7958-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="f7958-130">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset)|<span data-ttu-id="f7958-131">关闭该事例的用户。</span><span class="sxs-lookup"><span data-stu-id="f7958-131">The user who closed the case.</span></span>|
|<span data-ttu-id="f7958-132">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7958-132">closedDateTime</span></span>|<span data-ttu-id="f7958-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7958-133">DateTimeOffset</span></span>|<span data-ttu-id="f7958-134">关闭事例的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f7958-134">The date and time when the case was closed.</span></span> <span data-ttu-id="f7958-135">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="f7958-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f7958-136">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f7958-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f7958-137">createdBy</span><span class="sxs-lookup"><span data-stu-id="f7958-137">createdBy</span></span>|[<span data-ttu-id="f7958-138">identitySet</span><span class="sxs-lookup"><span data-stu-id="f7958-138">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset)|<span data-ttu-id="f7958-139">创建案例的用户。</span><span class="sxs-lookup"><span data-stu-id="f7958-139">The user who created the case.</span></span>|
|<span data-ttu-id="f7958-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f7958-140">createdDateTime</span></span>|<span data-ttu-id="f7958-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7958-141">DateTimeOffset</span></span>|<span data-ttu-id="f7958-142">实体的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f7958-142">The date and time when the entity was created.</span></span> <span data-ttu-id="f7958-143">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="f7958-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f7958-144">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f7958-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f7958-145">说明</span><span class="sxs-lookup"><span data-stu-id="f7958-145">description</span></span>|<span data-ttu-id="f7958-146">字符串</span><span class="sxs-lookup"><span data-stu-id="f7958-146">String</span></span>|<span data-ttu-id="f7958-147">事例说明。</span><span class="sxs-lookup"><span data-stu-id="f7958-147">The case description.</span></span>|
|<span data-ttu-id="f7958-148">displayName</span><span class="sxs-lookup"><span data-stu-id="f7958-148">displayName</span></span>|<span data-ttu-id="f7958-149">字符串</span><span class="sxs-lookup"><span data-stu-id="f7958-149">String</span></span>|<span data-ttu-id="f7958-150">事例名称。</span><span class="sxs-lookup"><span data-stu-id="f7958-150">The case name.</span></span>|
|<span data-ttu-id="f7958-151">externalId</span><span class="sxs-lookup"><span data-stu-id="f7958-151">externalId</span></span>|<span data-ttu-id="f7958-152">String</span><span class="sxs-lookup"><span data-stu-id="f7958-152">String</span></span>|<span data-ttu-id="f7958-153">Customer reference 的外部事例编号。</span><span class="sxs-lookup"><span data-stu-id="f7958-153">The external case number for customer reference.</span></span>|
|<span data-ttu-id="f7958-154">id</span><span class="sxs-lookup"><span data-stu-id="f7958-154">id</span></span>|<span data-ttu-id="f7958-155">String</span><span class="sxs-lookup"><span data-stu-id="f7958-155">String</span></span>| <span data-ttu-id="f7958-156">电子数据展示事例的 ID。</span><span class="sxs-lookup"><span data-stu-id="f7958-156">The ID for the eDiscovery case.</span></span> <span data-ttu-id="f7958-157">只读。</span><span class="sxs-lookup"><span data-stu-id="f7958-157">Read-only.</span></span> |
|<span data-ttu-id="f7958-158">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f7958-158">lastModifiedBy</span></span>|[<span data-ttu-id="f7958-159">identitySet</span><span class="sxs-lookup"><span data-stu-id="f7958-159">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset)|<span data-ttu-id="f7958-160">上次修改实体的用户。</span><span class="sxs-lookup"><span data-stu-id="f7958-160">The last user who modified the entity.</span></span>|
|<span data-ttu-id="f7958-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7958-161">lastModifiedDateTime</span></span>|<span data-ttu-id="f7958-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7958-162">DateTimeOffset</span></span>| <span data-ttu-id="f7958-163">修改事例的最新日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f7958-163">The latest date and time when the case was modified.</span></span> <span data-ttu-id="f7958-164">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="f7958-164">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f7958-165">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f7958-165">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f7958-166">状态</span><span class="sxs-lookup"><span data-stu-id="f7958-166">status</span></span>|<span data-ttu-id="f7958-167">字符串</span><span class="sxs-lookup"><span data-stu-id="f7958-167">String</span></span>| <span data-ttu-id="f7958-168">案例状态。</span><span class="sxs-lookup"><span data-stu-id="f7958-168">The case status.</span></span> <span data-ttu-id="f7958-169">可能的值为、、、、 `unknown` `active` `pendingDelete` `closing` `closed` 和 `closedWithError` 。</span><span class="sxs-lookup"><span data-stu-id="f7958-169">Possible values are `unknown`, `active`, `pendingDelete`, `closing`, `closed`, and `closedWithError`.</span></span> <span data-ttu-id="f7958-170">有关详细信息，请参阅下表。</span><span class="sxs-lookup"><span data-stu-id="f7958-170">For details see the following table.</span></span>|

### <a name="casestatus-values"></a><span data-ttu-id="f7958-171">caseStatus 值</span><span class="sxs-lookup"><span data-stu-id="f7958-171">caseStatus values</span></span>

|<span data-ttu-id="f7958-172">成员</span><span class="sxs-lookup"><span data-stu-id="f7958-172">Member</span></span>|<span data-ttu-id="f7958-173">说明</span><span class="sxs-lookup"><span data-stu-id="f7958-173">Description</span></span>|
|:----|-----------|
| <span data-ttu-id="f7958-174">unknown</span><span class="sxs-lookup"><span data-stu-id="f7958-174">unknown</span></span> | <span data-ttu-id="f7958-175">未知的案例状态。</span><span class="sxs-lookup"><span data-stu-id="f7958-175">Case status is unknown.</span></span> |
| <span data-ttu-id="f7958-176">工作</span><span class="sxs-lookup"><span data-stu-id="f7958-176">active</span></span> | <span data-ttu-id="f7958-177">案例处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="f7958-177">Case is active.</span></span> |
| <span data-ttu-id="f7958-178">pendingDelete</span><span class="sxs-lookup"><span data-stu-id="f7958-178">pendingDelete</span></span> | <span data-ttu-id="f7958-179">已删除事例，但尚未完全处理该删除。</span><span class="sxs-lookup"><span data-stu-id="f7958-179">Case was deleted, but the delete has not been fully transacted.</span></span> |
| <span data-ttu-id="f7958-180">结束语</span><span class="sxs-lookup"><span data-stu-id="f7958-180">closing</span></span> | <span data-ttu-id="f7958-181">事例已关闭，但操作尚未完全进行事务处理。</span><span class="sxs-lookup"><span data-stu-id="f7958-181">Case was closed, but the operation has not been fully transacted.</span></span> |
| <span data-ttu-id="f7958-182">停止</span><span class="sxs-lookup"><span data-stu-id="f7958-182">closed</span></span> | <span data-ttu-id="f7958-183">事例已关闭。</span><span class="sxs-lookup"><span data-stu-id="f7958-183">The case is closed.</span></span> |
| <span data-ttu-id="f7958-184">closedWithError</span><span class="sxs-lookup"><span data-stu-id="f7958-184">closedWithError</span></span> | <span data-ttu-id="f7958-185">事例已关闭，但在这种情况下释放保留时出现错误。</span><span class="sxs-lookup"><span data-stu-id="f7958-185">The case is closed, but there were errors releasing holds in the case.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f7958-186">关系</span><span class="sxs-lookup"><span data-stu-id="f7958-186">Relationships</span></span>

| <span data-ttu-id="f7958-187">关系</span><span class="sxs-lookup"><span data-stu-id="f7958-187">Relationship</span></span> | <span data-ttu-id="f7958-188">类型</span><span class="sxs-lookup"><span data-stu-id="f7958-188">Type</span></span>        | <span data-ttu-id="f7958-189">说明</span><span class="sxs-lookup"><span data-stu-id="f7958-189">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f7958-190">评审集</span><span class="sxs-lookup"><span data-stu-id="f7958-190">Review sets</span></span>|<span data-ttu-id="f7958-191">[reviewSet](reviewset.md)集合</span><span class="sxs-lookup"><span data-stu-id="f7958-191">[reviewSet](reviewset.md) collection</span></span>| <span data-ttu-id="f7958-192">案例中的审阅集集合。</span><span class="sxs-lookup"><span data-stu-id="f7958-192">Collection of review sets in the case.</span></span> <span data-ttu-id="f7958-193">只读。</span><span class="sxs-lookup"><span data-stu-id="f7958-193">Read-only.</span></span> <span data-ttu-id="f7958-194">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f7958-194">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f7958-195">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7958-195">JSON representation</span></span>

<span data-ttu-id="f7958-196">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7958-196">The following is a JSON representation of the resource.</span></span>

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
