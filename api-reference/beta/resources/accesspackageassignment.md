---
title: accessPackageAssignment 资源类型
description: 访问包分配是一种在一段时间内向特定主题分配访问包。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fd352fe67c3afabb1819ffc58d7081dbdae1525c
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298510"
---
# <a name="accesspackageassignment-resource-type"></a><span data-ttu-id="b0470-103">accessPackageAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="b0470-103">accessPackageAssignment resource type</span></span>

<span data-ttu-id="b0470-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0470-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0470-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包分配是一个在一段时间内向特定主题分配访问包。</span><span class="sxs-lookup"><span data-stu-id="b0470-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), an access package assignment is an assignment of an access package to a particular subject, for a period of time.</span></span>  <span data-ttu-id="b0470-106">例如，访问包分配可以说明在 2019 年 1 月到 2019 年 7 月期间，用户 Alice 已通过访问包 Sales 获得访问权限。</span><span class="sxs-lookup"><span data-stu-id="b0470-106">For example, an access package assignment can state that user Alice has been assigned access via the access package Sales for the period January 2019 through July 2019.</span></span>

## <a name="methods"></a><span data-ttu-id="b0470-107">方法</span><span class="sxs-lookup"><span data-stu-id="b0470-107">Methods</span></span>

| <span data-ttu-id="b0470-108">方法</span><span class="sxs-lookup"><span data-stu-id="b0470-108">Method</span></span>       | <span data-ttu-id="b0470-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b0470-109">Return Type</span></span> | <span data-ttu-id="b0470-110">说明</span><span class="sxs-lookup"><span data-stu-id="b0470-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b0470-111">列出 accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="b0470-111">List accessPackageAssignments</span></span>](../api/accesspackageassignment-list.md) | <span data-ttu-id="b0470-112">[accessPackageAssignment](accesspackageassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b0470-112">[accessPackageAssignment](accesspackageassignment.md) collection</span></span> | <span data-ttu-id="b0470-113">检索 **accessPackageAssignment 对象** 的列表。</span><span class="sxs-lookup"><span data-stu-id="b0470-113">Retrieve a list of **accessPackageAssignment** objects.</span></span> |
|[<span data-ttu-id="b0470-114">filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="b0470-114">filterByCurrentUser</span></span>](../api/accesspackageassignment-filterbycurrentuser.md)|<span data-ttu-id="b0470-115">[accessPackageAssignment](../resources/accesspackageassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b0470-115">[accessPackageAssignment](../resources/accesspackageassignment.md) collection</span></span>|<span data-ttu-id="b0470-116">检索在登录用户上筛选的 **accessPackageAssignment** 对象列表。</span><span class="sxs-lookup"><span data-stu-id="b0470-116">Retrieve the list of **accessPackageAssignment** objects filtered on the signed-in user.</span></span>|

><span data-ttu-id="b0470-117">**注意：** 你无法使用此方法创建或删除访问包分配。</span><span class="sxs-lookup"><span data-stu-id="b0470-117">**Note:** You can't use a method to create or remove an access package assignment.</span></span> <span data-ttu-id="b0470-118">相反，希望为用户请求访问包分配或者从用户删除访问包分配的客户端可以创建 [accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md)。</span><span class="sxs-lookup"><span data-stu-id="b0470-118">Instead, a client that wants to request an access package assignment for a user, or remove an access package assignment from a user, can [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b0470-119">属性</span><span class="sxs-lookup"><span data-stu-id="b0470-119">Properties</span></span>

| <span data-ttu-id="b0470-120">属性</span><span class="sxs-lookup"><span data-stu-id="b0470-120">Property</span></span>     | <span data-ttu-id="b0470-121">类型</span><span class="sxs-lookup"><span data-stu-id="b0470-121">Type</span></span>        | <span data-ttu-id="b0470-122">说明</span><span class="sxs-lookup"><span data-stu-id="b0470-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b0470-123">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="b0470-123">accessPackageId</span></span>|<span data-ttu-id="b0470-124">String</span><span class="sxs-lookup"><span data-stu-id="b0470-124">String</span></span>|<span data-ttu-id="b0470-125">访问包的标识符。</span><span class="sxs-lookup"><span data-stu-id="b0470-125">The identifier of the access package.</span></span> <span data-ttu-id="b0470-126">只读。</span><span class="sxs-lookup"><span data-stu-id="b0470-126">Read-only.</span></span>|
|<span data-ttu-id="b0470-127">assignmentPolicyId</span><span class="sxs-lookup"><span data-stu-id="b0470-127">assignmentPolicyId</span></span>|<span data-ttu-id="b0470-128">String</span><span class="sxs-lookup"><span data-stu-id="b0470-128">String</span></span>|<span data-ttu-id="b0470-129">访问包分配策略的标识符。</span><span class="sxs-lookup"><span data-stu-id="b0470-129">The identifier of the access package assignment policy.</span></span> <span data-ttu-id="b0470-130">只读。</span><span class="sxs-lookup"><span data-stu-id="b0470-130">Read-only.</span></span>|
|<span data-ttu-id="b0470-131">assignmentState</span><span class="sxs-lookup"><span data-stu-id="b0470-131">assignmentState</span></span>|<span data-ttu-id="b0470-132">String</span><span class="sxs-lookup"><span data-stu-id="b0470-132">String</span></span>|<span data-ttu-id="b0470-133">访问包分配的状态。</span><span class="sxs-lookup"><span data-stu-id="b0470-133">The state of the access package assignment.</span></span> <span data-ttu-id="b0470-134">可能的值是 `Delivering` 、 `Delivered` 或 `Expired` 。</span><span class="sxs-lookup"><span data-stu-id="b0470-134">Possible values are `Delivering`, `Delivered`, or `Expired`.</span></span> <span data-ttu-id="b0470-135">只读。</span><span class="sxs-lookup"><span data-stu-id="b0470-135">Read-only.</span></span>|
|<span data-ttu-id="b0470-136">assignmentStatus</span><span class="sxs-lookup"><span data-stu-id="b0470-136">assignmentStatus</span></span>|<span data-ttu-id="b0470-137">String</span><span class="sxs-lookup"><span data-stu-id="b0470-137">String</span></span>|<span data-ttu-id="b0470-138">有关分配生命周期详细信息。</span><span class="sxs-lookup"><span data-stu-id="b0470-138">More information about the assignment lifecycle.</span></span>  <span data-ttu-id="b0470-139">可能的值包括 `Delivering` `Delivered` 、、 `NearExpiry1DayNotificationTriggered` 或 `ExpiredNotificationTriggered` 。</span><span class="sxs-lookup"><span data-stu-id="b0470-139">Possible values include `Delivering`, `Delivered`, `NearExpiry1DayNotificationTriggered`, or `ExpiredNotificationTriggered`.</span></span>  <span data-ttu-id="b0470-140">只读。</span><span class="sxs-lookup"><span data-stu-id="b0470-140">Read-only.</span></span>|
|<span data-ttu-id="b0470-141">catalogId</span><span class="sxs-lookup"><span data-stu-id="b0470-141">catalogId</span></span>|<span data-ttu-id="b0470-142">String</span><span class="sxs-lookup"><span data-stu-id="b0470-142">String</span></span>|<span data-ttu-id="b0470-143">包含访问包的目录的标识符。</span><span class="sxs-lookup"><span data-stu-id="b0470-143">The identifier of the catalog containing the access package.</span></span> <span data-ttu-id="b0470-144">只读。</span><span class="sxs-lookup"><span data-stu-id="b0470-144">Read-only.</span></span>|
|<span data-ttu-id="b0470-145">expiredDateTime</span><span class="sxs-lookup"><span data-stu-id="b0470-145">expiredDateTime</span></span>|<span data-ttu-id="b0470-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0470-146">DateTimeOffset</span></span>|<span data-ttu-id="b0470-147">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="b0470-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b0470-148">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="b0470-148">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="b0470-149">id</span><span class="sxs-lookup"><span data-stu-id="b0470-149">id</span></span>|<span data-ttu-id="b0470-150">String</span><span class="sxs-lookup"><span data-stu-id="b0470-150">String</span></span>| <span data-ttu-id="b0470-151">只读。</span><span class="sxs-lookup"><span data-stu-id="b0470-151">Read-only.</span></span>|
|<span data-ttu-id="b0470-152">isExtended</span><span class="sxs-lookup"><span data-stu-id="b0470-152">isExtended</span></span>|<span data-ttu-id="b0470-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0470-153">Boolean</span></span>|<span data-ttu-id="b0470-154">指示是否已扩展访问包分配。</span><span class="sxs-lookup"><span data-stu-id="b0470-154">Indicates whether the access package assignment is extended.</span></span> <span data-ttu-id="b0470-155">只读。</span><span class="sxs-lookup"><span data-stu-id="b0470-155">Read-only.</span></span>|
|<span data-ttu-id="b0470-156">targetId</span><span class="sxs-lookup"><span data-stu-id="b0470-156">targetId</span></span>|<span data-ttu-id="b0470-157">String</span><span class="sxs-lookup"><span data-stu-id="b0470-157">String</span></span>| <span data-ttu-id="b0470-158">工作分配的主题 ID。</span><span class="sxs-lookup"><span data-stu-id="b0470-158">The ID of the subject with the assignment.</span></span> <span data-ttu-id="b0470-159">只读。</span><span class="sxs-lookup"><span data-stu-id="b0470-159">Read-only.</span></span>|
|<span data-ttu-id="b0470-160">schedule</span><span class="sxs-lookup"><span data-stu-id="b0470-160">schedule</span></span>|[<span data-ttu-id="b0470-161">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="b0470-161">requestSchedule</span></span>](requestschedule.md)| <span data-ttu-id="b0470-162">当访问分配就位时。</span><span class="sxs-lookup"><span data-stu-id="b0470-162">When the access assignment is to be in place.</span></span> <span data-ttu-id="b0470-163">只读。</span><span class="sxs-lookup"><span data-stu-id="b0470-163">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0470-164">关系</span><span class="sxs-lookup"><span data-stu-id="b0470-164">Relationships</span></span>

| <span data-ttu-id="b0470-165">关系</span><span class="sxs-lookup"><span data-stu-id="b0470-165">Relationship</span></span> | <span data-ttu-id="b0470-166">类型</span><span class="sxs-lookup"><span data-stu-id="b0470-166">Type</span></span>        | <span data-ttu-id="b0470-167">说明</span><span class="sxs-lookup"><span data-stu-id="b0470-167">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b0470-168">accessPackage</span><span class="sxs-lookup"><span data-stu-id="b0470-168">accessPackage</span></span>|[<span data-ttu-id="b0470-169">accessPackage</span><span class="sxs-lookup"><span data-stu-id="b0470-169">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="b0470-p112">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="b0470-p112">Read-only. Nullable.</span></span>|
|<span data-ttu-id="b0470-172">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="b0470-172">accessPackageAssignmentPolicy</span></span>|[<span data-ttu-id="b0470-173">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="b0470-173">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md)| <span data-ttu-id="b0470-p113">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="b0470-p113">Read-only. Nullable.</span></span>|
|<span data-ttu-id="b0470-176">accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="b0470-176">accessPackageAssignmentResourceRoles</span></span>|<span data-ttu-id="b0470-177">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b0470-177">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span>| <span data-ttu-id="b0470-178">为此分配的目标用户传递的资源角色。</span><span class="sxs-lookup"><span data-stu-id="b0470-178">The resource roles delivered to the target user for this assignment.</span></span> <span data-ttu-id="b0470-179">只读。</span><span class="sxs-lookup"><span data-stu-id="b0470-179">Read-only.</span></span> <span data-ttu-id="b0470-180">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="b0470-180">Nullable.</span></span>|
|<span data-ttu-id="b0470-181">target</span><span class="sxs-lookup"><span data-stu-id="b0470-181">target</span></span>|[<span data-ttu-id="b0470-182">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="b0470-182">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="b0470-183">访问包分配的主题。</span><span class="sxs-lookup"><span data-stu-id="b0470-183">The subject of the access package assignment.</span></span> <span data-ttu-id="b0470-184">只读。</span><span class="sxs-lookup"><span data-stu-id="b0470-184">Read-only.</span></span> <span data-ttu-id="b0470-185">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="b0470-185">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0470-186">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0470-186">JSON representation</span></span>

<span data-ttu-id="b0470-187">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0470-187">The following is a JSON representation of the resource.</span></span>

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


