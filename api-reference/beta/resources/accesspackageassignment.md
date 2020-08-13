---
title: accessPackageAssignment 资源类型
description: 访问包分配是一段时间内特定主题的访问包的分配。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2b52b9dbd7b2b76df34ab6c55a46b69718d4a0e2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508560"
---
# <a name="accesspackageassignment-resource-type"></a><span data-ttu-id="edb6a-103">accessPackageAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="edb6a-103">accessPackageAssignment resource type</span></span>

<span data-ttu-id="edb6a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edb6a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edb6a-105">在 [AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配是一段时间内特定主题的访问包分配。</span><span class="sxs-lookup"><span data-stu-id="edb6a-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment is an assignment of an access package to a particular subject, for a period of time.</span></span>  <span data-ttu-id="edb6a-106">例如，访问包分配可能表明用户 "Alice" 已通过访问包 "Sales" 在2019年1月到7月2019的阶段分配了访问权限。</span><span class="sxs-lookup"><span data-stu-id="edb6a-106">For example, an access package assignment could state that user 'Alice' has the been assigned access via the access package 'Sales' for the period January 2019 through July 2019.</span></span>

## <a name="methods"></a><span data-ttu-id="edb6a-107">方法</span><span class="sxs-lookup"><span data-stu-id="edb6a-107">Methods</span></span>

| <span data-ttu-id="edb6a-108">方法</span><span class="sxs-lookup"><span data-stu-id="edb6a-108">Method</span></span>       | <span data-ttu-id="edb6a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="edb6a-109">Return Type</span></span> | <span data-ttu-id="edb6a-110">说明</span><span class="sxs-lookup"><span data-stu-id="edb6a-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="edb6a-111">列出 accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="edb6a-111">List accessPackageAssignments</span></span>](../api/accesspackageassignment-list.md) | <span data-ttu-id="edb6a-112">[accessPackageAssignment](accesspackageassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="edb6a-112">[accessPackageAssignment](accesspackageassignment.md) collection</span></span> | <span data-ttu-id="edb6a-113">检索 **accesspackageassignment** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="edb6a-113">Retrieve a list of **accesspackageassignment** objects.</span></span> |

><span data-ttu-id="edb6a-114">**注意：** 不能使用方法来创建或删除访问包分配。</span><span class="sxs-lookup"><span data-stu-id="edb6a-114">**Note:** You can't use a method to create or remove an access package assignment.</span></span> <span data-ttu-id="edb6a-115">相反，要为用户请求访问包分配或从用户中删除访问包分配的客户端，可以 [创建 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md)。</span><span class="sxs-lookup"><span data-stu-id="edb6a-115">Instead, a client that wants to request an access package assignment for a user, or remove an access package assignment from a user, can [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span></span>

## <a name="properties"></a><span data-ttu-id="edb6a-116">属性</span><span class="sxs-lookup"><span data-stu-id="edb6a-116">Properties</span></span>

| <span data-ttu-id="edb6a-117">属性</span><span class="sxs-lookup"><span data-stu-id="edb6a-117">Property</span></span>     | <span data-ttu-id="edb6a-118">类型</span><span class="sxs-lookup"><span data-stu-id="edb6a-118">Type</span></span>        | <span data-ttu-id="edb6a-119">说明</span><span class="sxs-lookup"><span data-stu-id="edb6a-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="edb6a-120">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="edb6a-120">accessPackageId</span></span>|<span data-ttu-id="edb6a-121">String</span><span class="sxs-lookup"><span data-stu-id="edb6a-121">String</span></span>|<span data-ttu-id="edb6a-122">访问包的标识符。</span><span class="sxs-lookup"><span data-stu-id="edb6a-122">The identifier of the access package.</span></span> <span data-ttu-id="edb6a-123">只读。</span><span class="sxs-lookup"><span data-stu-id="edb6a-123">Read-only.</span></span>|
|<span data-ttu-id="edb6a-124">assignmentPolicyId</span><span class="sxs-lookup"><span data-stu-id="edb6a-124">assignmentPolicyId</span></span>|<span data-ttu-id="edb6a-125">String</span><span class="sxs-lookup"><span data-stu-id="edb6a-125">String</span></span>|<span data-ttu-id="edb6a-126">访问包分配策略的标识符。</span><span class="sxs-lookup"><span data-stu-id="edb6a-126">The identifier of the access package assignment policy.</span></span> <span data-ttu-id="edb6a-127">只读。</span><span class="sxs-lookup"><span data-stu-id="edb6a-127">Read-only.</span></span>|
|<span data-ttu-id="edb6a-128">assignmentState</span><span class="sxs-lookup"><span data-stu-id="edb6a-128">assignmentState</span></span>|<span data-ttu-id="edb6a-129">String</span><span class="sxs-lookup"><span data-stu-id="edb6a-129">String</span></span>|<span data-ttu-id="edb6a-130">访问程序包的状态。</span><span class="sxs-lookup"><span data-stu-id="edb6a-130">The state of the access package.</span></span> <span data-ttu-id="edb6a-131">可能的值为 `Delivered` 或 `Expired` 。</span><span class="sxs-lookup"><span data-stu-id="edb6a-131">Possible values are `Delivered` or `Expired`.</span></span> <span data-ttu-id="edb6a-132">只读。</span><span class="sxs-lookup"><span data-stu-id="edb6a-132">Read-only.</span></span>|
|<span data-ttu-id="edb6a-133">assignmentStatus</span><span class="sxs-lookup"><span data-stu-id="edb6a-133">assignmentStatus</span></span>|<span data-ttu-id="edb6a-134">String</span><span class="sxs-lookup"><span data-stu-id="edb6a-134">String</span></span>|<span data-ttu-id="edb6a-135">只读。</span><span class="sxs-lookup"><span data-stu-id="edb6a-135">Read-only.</span></span>|
|<span data-ttu-id="edb6a-136">catalogId</span><span class="sxs-lookup"><span data-stu-id="edb6a-136">catalogId</span></span>|<span data-ttu-id="edb6a-137">String</span><span class="sxs-lookup"><span data-stu-id="edb6a-137">String</span></span>|<span data-ttu-id="edb6a-138">包含访问包的目录的标识符。</span><span class="sxs-lookup"><span data-stu-id="edb6a-138">The identifier of the catalog containing the access package.</span></span> <span data-ttu-id="edb6a-139">只读。</span><span class="sxs-lookup"><span data-stu-id="edb6a-139">Read-only.</span></span>|
|<span data-ttu-id="edb6a-140">expiredDateTime</span><span class="sxs-lookup"><span data-stu-id="edb6a-140">expiredDateTime</span></span>|<span data-ttu-id="edb6a-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edb6a-141">DateTimeOffset</span></span>|<span data-ttu-id="edb6a-p107">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="edb6a-p107">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="edb6a-144">id</span><span class="sxs-lookup"><span data-stu-id="edb6a-144">id</span></span>|<span data-ttu-id="edb6a-145">String</span><span class="sxs-lookup"><span data-stu-id="edb6a-145">String</span></span>| <span data-ttu-id="edb6a-146">只读。</span><span class="sxs-lookup"><span data-stu-id="edb6a-146">Read-only.</span></span>|
|<span data-ttu-id="edb6a-147">isExtended</span><span class="sxs-lookup"><span data-stu-id="edb6a-147">isExtended</span></span>|<span data-ttu-id="edb6a-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="edb6a-148">Boolean</span></span>|<span data-ttu-id="edb6a-149">指示访问包分配是否已扩展。</span><span class="sxs-lookup"><span data-stu-id="edb6a-149">Indicates whether the access package assignment is extended.</span></span> <span data-ttu-id="edb6a-150">只读。</span><span class="sxs-lookup"><span data-stu-id="edb6a-150">Read-only.</span></span>|
|<span data-ttu-id="edb6a-151">targetId</span><span class="sxs-lookup"><span data-stu-id="edb6a-151">targetId</span></span>|<span data-ttu-id="edb6a-152">String</span><span class="sxs-lookup"><span data-stu-id="edb6a-152">String</span></span>| <span data-ttu-id="edb6a-153">包含工作分配的主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="edb6a-153">The ID of the subject with the assignment.</span></span> <span data-ttu-id="edb6a-154">只读。</span><span class="sxs-lookup"><span data-stu-id="edb6a-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="edb6a-155">关系</span><span class="sxs-lookup"><span data-stu-id="edb6a-155">Relationships</span></span>

| <span data-ttu-id="edb6a-156">关系</span><span class="sxs-lookup"><span data-stu-id="edb6a-156">Relationship</span></span> | <span data-ttu-id="edb6a-157">类型</span><span class="sxs-lookup"><span data-stu-id="edb6a-157">Type</span></span>        | <span data-ttu-id="edb6a-158">说明</span><span class="sxs-lookup"><span data-stu-id="edb6a-158">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="edb6a-159">accessPackage</span><span class="sxs-lookup"><span data-stu-id="edb6a-159">accessPackage</span></span>|[<span data-ttu-id="edb6a-160">accessPackage</span><span class="sxs-lookup"><span data-stu-id="edb6a-160">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="edb6a-161">只读。</span><span class="sxs-lookup"><span data-stu-id="edb6a-161">Read-only.</span></span> <span data-ttu-id="edb6a-162">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="edb6a-162">Nullable.</span></span>|
|<span data-ttu-id="edb6a-163">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="edb6a-163">accessPackageAssignmentPolicy</span></span>|[<span data-ttu-id="edb6a-164">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="edb6a-164">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md)| <span data-ttu-id="edb6a-165">只读。</span><span class="sxs-lookup"><span data-stu-id="edb6a-165">Read-only.</span></span> <span data-ttu-id="edb6a-166">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="edb6a-166">Nullable.</span></span>|
|<span data-ttu-id="edb6a-167">accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="edb6a-167">accessPackageAssignmentResourceRoles</span></span>|<span data-ttu-id="edb6a-168">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="edb6a-168">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span>| <span data-ttu-id="edb6a-169">只读。</span><span class="sxs-lookup"><span data-stu-id="edb6a-169">Read-only.</span></span> <span data-ttu-id="edb6a-170">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="edb6a-170">Nullable.</span></span>|
|<span data-ttu-id="edb6a-171">target</span><span class="sxs-lookup"><span data-stu-id="edb6a-171">target</span></span>|[<span data-ttu-id="edb6a-172">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="edb6a-172">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="edb6a-173">访问包分配的主题。</span><span class="sxs-lookup"><span data-stu-id="edb6a-173">The subject of the access package assignment.</span></span> <span data-ttu-id="edb6a-174">只读。</span><span class="sxs-lookup"><span data-stu-id="edb6a-174">Read-only.</span></span> <span data-ttu-id="edb6a-175">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="edb6a-175">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="edb6a-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="edb6a-176">JSON representation</span></span>

<span data-ttu-id="edb6a-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="edb6a-177">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
            "id": "9bdae7b4-6ece-487b-9eb8-9679dbd67aa2",
            "catalogId": "cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
            "accessPackageId": "e3f47362-993f-4fcb-8a38-532ffca16150",
            "assignmentPolicyId": "63ebd106-8116-40e7-a0ab-01ae475d11bb",
            "targetId": "ab4291f6-66b7-42bf-b597-a05b29414f5c",
            "assignmentStatus": "ExpiredNotificationTriggered",
            "assignmentState": "Expired",
            "isExtended": false,
            "expiredDateTime": "2019-04-25T23:45:40.42Z"
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
