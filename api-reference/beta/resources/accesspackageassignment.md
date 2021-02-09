---
title: accessPackageAssignment 资源类型
description: 访问包分配是一个在一段时间内向特定主题分配访问包。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3a7d9a947490676b48a170130fac2bf9e776c183
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155620"
---
# <a name="accesspackageassignment-resource-type"></a><span data-ttu-id="d4778-103">accessPackageAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4778-103">accessPackageAssignment resource type</span></span>

<span data-ttu-id="d4778-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4778-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4778-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包分配是一个在一段时间内向特定主题分配访问包。</span><span class="sxs-lookup"><span data-stu-id="d4778-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment is an assignment of an access package to a particular subject, for a period of time.</span></span>  <span data-ttu-id="d4778-106">例如，访问包分配可以说明在 2019 年 1 月到 2019 年 7 月期间，用户 Alice 已通过访问包 Sales 分配访问权限。</span><span class="sxs-lookup"><span data-stu-id="d4778-106">For example, an access package assignment can state that user Alice has been assigned access via the access package Sales for the period January 2019 through July 2019.</span></span>

## <a name="methods"></a><span data-ttu-id="d4778-107">方法</span><span class="sxs-lookup"><span data-stu-id="d4778-107">Methods</span></span>

| <span data-ttu-id="d4778-108">方法</span><span class="sxs-lookup"><span data-stu-id="d4778-108">Method</span></span>       | <span data-ttu-id="d4778-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d4778-109">Return Type</span></span> | <span data-ttu-id="d4778-110">说明</span><span class="sxs-lookup"><span data-stu-id="d4778-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d4778-111">列出 accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="d4778-111">List accessPackageAssignments</span></span>](../api/accesspackageassignment-list.md) | <span data-ttu-id="d4778-112">[accessPackageAssignment](accesspackageassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d4778-112">[accessPackageAssignment](accesspackageassignment.md) collection</span></span> | <span data-ttu-id="d4778-113">检索 **accesspackageassignment 对象** 的列表。</span><span class="sxs-lookup"><span data-stu-id="d4778-113">Retrieve a list of **accesspackageassignment** objects.</span></span> |

><span data-ttu-id="d4778-114">**注意：** 不能使用此方法创建或删除访问包分配。</span><span class="sxs-lookup"><span data-stu-id="d4778-114">**Note:** You can't use a method to create or remove an access package assignment.</span></span> <span data-ttu-id="d4778-115">相反，希望请求为用户分配访问包，或者从用户中删除访问包分配的客户端可以创建[accessPackageAssignmentRequest。](../api/accesspackageassignmentrequest-post.md)</span><span class="sxs-lookup"><span data-stu-id="d4778-115">Instead, a client that wants to request an access package assignment for a user, or remove an access package assignment from a user, can [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d4778-116">属性</span><span class="sxs-lookup"><span data-stu-id="d4778-116">Properties</span></span>

| <span data-ttu-id="d4778-117">属性</span><span class="sxs-lookup"><span data-stu-id="d4778-117">Property</span></span>     | <span data-ttu-id="d4778-118">类型</span><span class="sxs-lookup"><span data-stu-id="d4778-118">Type</span></span>        | <span data-ttu-id="d4778-119">说明</span><span class="sxs-lookup"><span data-stu-id="d4778-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d4778-120">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="d4778-120">accessPackageId</span></span>|<span data-ttu-id="d4778-121">String</span><span class="sxs-lookup"><span data-stu-id="d4778-121">String</span></span>|<span data-ttu-id="d4778-122">访问包的标识符。</span><span class="sxs-lookup"><span data-stu-id="d4778-122">The identifier of the access package.</span></span> <span data-ttu-id="d4778-123">只读。</span><span class="sxs-lookup"><span data-stu-id="d4778-123">Read-only.</span></span>|
|<span data-ttu-id="d4778-124">assignmentPolicyId</span><span class="sxs-lookup"><span data-stu-id="d4778-124">assignmentPolicyId</span></span>|<span data-ttu-id="d4778-125">String</span><span class="sxs-lookup"><span data-stu-id="d4778-125">String</span></span>|<span data-ttu-id="d4778-126">访问包分配策略的标识符。</span><span class="sxs-lookup"><span data-stu-id="d4778-126">The identifier of the access package assignment policy.</span></span> <span data-ttu-id="d4778-127">只读。</span><span class="sxs-lookup"><span data-stu-id="d4778-127">Read-only.</span></span>|
|<span data-ttu-id="d4778-128">assignmentState</span><span class="sxs-lookup"><span data-stu-id="d4778-128">assignmentState</span></span>|<span data-ttu-id="d4778-129">String</span><span class="sxs-lookup"><span data-stu-id="d4778-129">String</span></span>|<span data-ttu-id="d4778-130">访问包分配的状态。</span><span class="sxs-lookup"><span data-stu-id="d4778-130">The state of the access package assignment.</span></span> <span data-ttu-id="d4778-131">可能的值是 `Delivering` ， `Delivered` 或 `Expired` 。</span><span class="sxs-lookup"><span data-stu-id="d4778-131">Possible values are `Delivering`, `Delivered`, or `Expired`.</span></span> <span data-ttu-id="d4778-132">只读。</span><span class="sxs-lookup"><span data-stu-id="d4778-132">Read-only.</span></span>|
|<span data-ttu-id="d4778-133">assignmentStatus</span><span class="sxs-lookup"><span data-stu-id="d4778-133">assignmentStatus</span></span>|<span data-ttu-id="d4778-134">String</span><span class="sxs-lookup"><span data-stu-id="d4778-134">String</span></span>|<span data-ttu-id="d4778-135">有关工作分配生命周期详细信息。</span><span class="sxs-lookup"><span data-stu-id="d4778-135">More information about the assignment lifecycle.</span></span>  <span data-ttu-id="d4778-136">可能的值包括 `Delivering` 、 `Delivered` 或 `NearExpiry1DayNotificationTriggered` `ExpiredNotificationTriggered` 。</span><span class="sxs-lookup"><span data-stu-id="d4778-136">Possible values include `Delivering`, `Delivered`, `NearExpiry1DayNotificationTriggered`, or `ExpiredNotificationTriggered`.</span></span>  <span data-ttu-id="d4778-137">只读。</span><span class="sxs-lookup"><span data-stu-id="d4778-137">Read-only.</span></span>|
|<span data-ttu-id="d4778-138">catalogId</span><span class="sxs-lookup"><span data-stu-id="d4778-138">catalogId</span></span>|<span data-ttu-id="d4778-139">String</span><span class="sxs-lookup"><span data-stu-id="d4778-139">String</span></span>|<span data-ttu-id="d4778-140">包含访问包的目录的标识符。</span><span class="sxs-lookup"><span data-stu-id="d4778-140">The identifier of the catalog containing the access package.</span></span> <span data-ttu-id="d4778-141">只读。</span><span class="sxs-lookup"><span data-stu-id="d4778-141">Read-only.</span></span>|
|<span data-ttu-id="d4778-142">expiredDateTime</span><span class="sxs-lookup"><span data-stu-id="d4778-142">expiredDateTime</span></span>|<span data-ttu-id="d4778-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4778-143">DateTimeOffset</span></span>|<span data-ttu-id="d4778-p108">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d4778-p108">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d4778-146">id</span><span class="sxs-lookup"><span data-stu-id="d4778-146">id</span></span>|<span data-ttu-id="d4778-147">String</span><span class="sxs-lookup"><span data-stu-id="d4778-147">String</span></span>| <span data-ttu-id="d4778-148">只读。</span><span class="sxs-lookup"><span data-stu-id="d4778-148">Read-only.</span></span>|
|<span data-ttu-id="d4778-149">isExtended</span><span class="sxs-lookup"><span data-stu-id="d4778-149">isExtended</span></span>|<span data-ttu-id="d4778-150">布尔</span><span class="sxs-lookup"><span data-stu-id="d4778-150">Boolean</span></span>|<span data-ttu-id="d4778-151">指示是否已扩展访问包分配。</span><span class="sxs-lookup"><span data-stu-id="d4778-151">Indicates whether the access package assignment is extended.</span></span> <span data-ttu-id="d4778-152">只读。</span><span class="sxs-lookup"><span data-stu-id="d4778-152">Read-only.</span></span>|
|<span data-ttu-id="d4778-153">targetId</span><span class="sxs-lookup"><span data-stu-id="d4778-153">targetId</span></span>|<span data-ttu-id="d4778-154">String</span><span class="sxs-lookup"><span data-stu-id="d4778-154">String</span></span>| <span data-ttu-id="d4778-155">工作分配的主题 ID。</span><span class="sxs-lookup"><span data-stu-id="d4778-155">The ID of the subject with the assignment.</span></span> <span data-ttu-id="d4778-156">只读。</span><span class="sxs-lookup"><span data-stu-id="d4778-156">Read-only.</span></span>|
|<span data-ttu-id="d4778-157">schedule</span><span class="sxs-lookup"><span data-stu-id="d4778-157">schedule</span></span>|[<span data-ttu-id="d4778-158">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="d4778-158">requestSchedule</span></span>](requestschedule.md)| <span data-ttu-id="d4778-159">当访问分配就位时。</span><span class="sxs-lookup"><span data-stu-id="d4778-159">When the access assignment is to be in place.</span></span> <span data-ttu-id="d4778-160">只读。</span><span class="sxs-lookup"><span data-stu-id="d4778-160">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4778-161">关系</span><span class="sxs-lookup"><span data-stu-id="d4778-161">Relationships</span></span>

| <span data-ttu-id="d4778-162">关系</span><span class="sxs-lookup"><span data-stu-id="d4778-162">Relationship</span></span> | <span data-ttu-id="d4778-163">类型</span><span class="sxs-lookup"><span data-stu-id="d4778-163">Type</span></span>        | <span data-ttu-id="d4778-164">说明</span><span class="sxs-lookup"><span data-stu-id="d4778-164">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d4778-165">accessPackage</span><span class="sxs-lookup"><span data-stu-id="d4778-165">accessPackage</span></span>|[<span data-ttu-id="d4778-166">accessPackage</span><span class="sxs-lookup"><span data-stu-id="d4778-166">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="d4778-167">只读。</span><span class="sxs-lookup"><span data-stu-id="d4778-167">Read-only.</span></span> <span data-ttu-id="d4778-168">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="d4778-168">Nullable.</span></span>|
|<span data-ttu-id="d4778-169">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="d4778-169">accessPackageAssignmentPolicy</span></span>|[<span data-ttu-id="d4778-170">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="d4778-170">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md)| <span data-ttu-id="d4778-171">只读。</span><span class="sxs-lookup"><span data-stu-id="d4778-171">Read-only.</span></span> <span data-ttu-id="d4778-172">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="d4778-172">Nullable.</span></span>|
|<span data-ttu-id="d4778-173">accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="d4778-173">accessPackageAssignmentResourceRoles</span></span>|<span data-ttu-id="d4778-174">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d4778-174">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span>| <span data-ttu-id="d4778-175">为此分配传递给目标用户的资源角色。</span><span class="sxs-lookup"><span data-stu-id="d4778-175">The resource roles delivered to the target user for this assignment.</span></span> <span data-ttu-id="d4778-176">只读。</span><span class="sxs-lookup"><span data-stu-id="d4778-176">Read-only.</span></span> <span data-ttu-id="d4778-177">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="d4778-177">Nullable.</span></span>|
|<span data-ttu-id="d4778-178">target</span><span class="sxs-lookup"><span data-stu-id="d4778-178">target</span></span>|[<span data-ttu-id="d4778-179">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="d4778-179">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="d4778-180">访问包分配的主题。</span><span class="sxs-lookup"><span data-stu-id="d4778-180">The subject of the access package assignment.</span></span> <span data-ttu-id="d4778-181">只读。</span><span class="sxs-lookup"><span data-stu-id="d4778-181">Read-only.</span></span> <span data-ttu-id="d4778-182">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d4778-182">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4778-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4778-183">JSON representation</span></span>

<span data-ttu-id="d4778-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4778-184">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "keyProperty": "id"
}-->

```json
{
   "id":"9bdae7b4-6ece-487b-9eb8-9679dbd67aa2",
   "catalogId":"cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
   "accessPackageId":"e3f47362-993f-4fcb-8a38-532ffca16150",
   "assignmentPolicyId":"63ebd106-8116-40e7-a0ab-01ae475d11bb",
   "targetId":"ab4291f6-66b7-42bf-b597-a05b29414f5c",
   "assignmentStatus":"ExpiredNotificationTriggered",
   "assignmentState":"Expired",
   "isExtended":false,
   "expiredDateTime":"2019-04-25T23:45:40.42Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


