---
title: accessPackageAssignment 资源类型
description: 访问包分配是一段时间内特定主题的访问包的分配。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 234aad48e11a2b6c5c2a47c494216fa15fbc139b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939213"
---
# <a name="accesspackageassignment-resource-type"></a><span data-ttu-id="cfa7a-103">accessPackageAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="cfa7a-103">accessPackageAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfa7a-104">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配是一段时间内特定主题的访问包分配。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment is an assignment of an access package to a particular subject, for a period of time.</span></span>  <span data-ttu-id="cfa7a-105">例如，访问包分配可能表明用户 "Alice" 已通过访问包 "Sales" 在2019年1月到7月2019的阶段分配了访问权限。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-105">For example, an access package assignment could state that user 'Alice' has the been assigned access via the access package 'Sales' for the period January 2019 through July 2019.</span></span>

## <a name="methods"></a><span data-ttu-id="cfa7a-106">方法</span><span class="sxs-lookup"><span data-stu-id="cfa7a-106">Methods</span></span>

| <span data-ttu-id="cfa7a-107">方法</span><span class="sxs-lookup"><span data-stu-id="cfa7a-107">Method</span></span>       | <span data-ttu-id="cfa7a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="cfa7a-108">Return Type</span></span> | <span data-ttu-id="cfa7a-109">说明</span><span class="sxs-lookup"><span data-stu-id="cfa7a-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cfa7a-110">列出 accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="cfa7a-110">List accessPackageAssignments</span></span>](../api/accesspackageassignment-list.md) | <span data-ttu-id="cfa7a-111">[accessPackageAssignment](accesspackageassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="cfa7a-111">[accessPackageAssignment](accesspackageassignment.md) collection</span></span> | <span data-ttu-id="cfa7a-112">检索**accesspackageassignment**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-112">Retrieve a list of **accesspackageassignment** objects.</span></span> |

><span data-ttu-id="cfa7a-113">**注意：** 不能使用方法创建访问包分配。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-113">**Note:** You can't use a method to create an access package assignment.</span></span> <span data-ttu-id="cfa7a-114">相反，要请求用户的访问包分配的客户端可以[创建 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md)。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-114">Instead, a client that wants to request an access package assignment for a user can [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cfa7a-115">属性</span><span class="sxs-lookup"><span data-stu-id="cfa7a-115">Properties</span></span>

| <span data-ttu-id="cfa7a-116">属性</span><span class="sxs-lookup"><span data-stu-id="cfa7a-116">Property</span></span>     | <span data-ttu-id="cfa7a-117">类型</span><span class="sxs-lookup"><span data-stu-id="cfa7a-117">Type</span></span>        | <span data-ttu-id="cfa7a-118">描述</span><span class="sxs-lookup"><span data-stu-id="cfa7a-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cfa7a-119">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="cfa7a-119">accessPackageId</span></span>|<span data-ttu-id="cfa7a-120">字符串</span><span class="sxs-lookup"><span data-stu-id="cfa7a-120">String</span></span>|<span data-ttu-id="cfa7a-121">访问包的标识符。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-121">The identifier of the access package.</span></span> <span data-ttu-id="cfa7a-122">只读。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-122">Read-only.</span></span>|
|<span data-ttu-id="cfa7a-123">assignmentPolicyId</span><span class="sxs-lookup"><span data-stu-id="cfa7a-123">assignmentPolicyId</span></span>|<span data-ttu-id="cfa7a-124">字符串</span><span class="sxs-lookup"><span data-stu-id="cfa7a-124">String</span></span>|<span data-ttu-id="cfa7a-125">访问包分配策略的标识符。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-125">The identifier of the access package assignment policy.</span></span> <span data-ttu-id="cfa7a-126">只读。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-126">Read-only.</span></span>|
|<span data-ttu-id="cfa7a-127">assignmentState</span><span class="sxs-lookup"><span data-stu-id="cfa7a-127">assignmentState</span></span>|<span data-ttu-id="cfa7a-128">字符串</span><span class="sxs-lookup"><span data-stu-id="cfa7a-128">String</span></span>|<span data-ttu-id="cfa7a-129">只读。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-129">Read-only.</span></span>|
|<span data-ttu-id="cfa7a-130">assignmentStatus</span><span class="sxs-lookup"><span data-stu-id="cfa7a-130">assignmentStatus</span></span>|<span data-ttu-id="cfa7a-131">字符串</span><span class="sxs-lookup"><span data-stu-id="cfa7a-131">String</span></span>|<span data-ttu-id="cfa7a-132">只读。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-132">Read-only.</span></span>|
|<span data-ttu-id="cfa7a-133">catalogId</span><span class="sxs-lookup"><span data-stu-id="cfa7a-133">catalogId</span></span>|<span data-ttu-id="cfa7a-134">字符串</span><span class="sxs-lookup"><span data-stu-id="cfa7a-134">String</span></span>|<span data-ttu-id="cfa7a-135">包含访问包的目录的标识符。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-135">The identifier of the catalog containing the access package.</span></span> <span data-ttu-id="cfa7a-136">只读。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-136">Read-only.</span></span>|
|<span data-ttu-id="cfa7a-137">expiredDateTime</span><span class="sxs-lookup"><span data-stu-id="cfa7a-137">expiredDateTime</span></span>|<span data-ttu-id="cfa7a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfa7a-138">DateTimeOffset</span></span>|<span data-ttu-id="cfa7a-p106">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="cfa7a-p106">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="cfa7a-141">id</span><span class="sxs-lookup"><span data-stu-id="cfa7a-141">id</span></span>|<span data-ttu-id="cfa7a-142">字符串</span><span class="sxs-lookup"><span data-stu-id="cfa7a-142">String</span></span>| <span data-ttu-id="cfa7a-143">只读。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-143">Read-only.</span></span>|
|<span data-ttu-id="cfa7a-144">isExtended</span><span class="sxs-lookup"><span data-stu-id="cfa7a-144">isExtended</span></span>|<span data-ttu-id="cfa7a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfa7a-145">Boolean</span></span>|<span data-ttu-id="cfa7a-146">指示访问包分配是否已扩展。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-146">Indicates whether the access package assignment is extended.</span></span> <span data-ttu-id="cfa7a-147">只读。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-147">Read-only.</span></span>|
|<span data-ttu-id="cfa7a-148">targetId</span><span class="sxs-lookup"><span data-stu-id="cfa7a-148">targetId</span></span>|<span data-ttu-id="cfa7a-149">字符串</span><span class="sxs-lookup"><span data-stu-id="cfa7a-149">String</span></span>| <span data-ttu-id="cfa7a-150">包含工作分配的主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-150">The ID of the subject with the assignment.</span></span> <span data-ttu-id="cfa7a-151">只读。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfa7a-152">关系</span><span class="sxs-lookup"><span data-stu-id="cfa7a-152">Relationships</span></span>

| <span data-ttu-id="cfa7a-153">关系</span><span class="sxs-lookup"><span data-stu-id="cfa7a-153">Relationship</span></span> | <span data-ttu-id="cfa7a-154">类型</span><span class="sxs-lookup"><span data-stu-id="cfa7a-154">Type</span></span>        | <span data-ttu-id="cfa7a-155">描述</span><span class="sxs-lookup"><span data-stu-id="cfa7a-155">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cfa7a-156">accessPackage</span><span class="sxs-lookup"><span data-stu-id="cfa7a-156">accessPackage</span></span>|[<span data-ttu-id="cfa7a-157">accessPackage</span><span class="sxs-lookup"><span data-stu-id="cfa7a-157">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="cfa7a-158">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-158">Read-only.</span></span> <span data-ttu-id="cfa7a-159">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-159">Nullable.</span></span>|
|<span data-ttu-id="cfa7a-160">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="cfa7a-160">accessPackageAssignmentPolicy</span></span>|[<span data-ttu-id="cfa7a-161">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="cfa7a-161">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md)| <span data-ttu-id="cfa7a-162">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-162">Read-only.</span></span> <span data-ttu-id="cfa7a-163">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-163">Nullable.</span></span>|
|<span data-ttu-id="cfa7a-164">accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="cfa7a-164">accessPackageAssignmentResourceRoles</span></span>|<span data-ttu-id="cfa7a-165">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)集合</span><span class="sxs-lookup"><span data-stu-id="cfa7a-165">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span>| <span data-ttu-id="cfa7a-166">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-166">Read-only.</span></span> <span data-ttu-id="cfa7a-167">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-167">Nullable.</span></span>|
|<span data-ttu-id="cfa7a-168">target</span><span class="sxs-lookup"><span data-stu-id="cfa7a-168">target</span></span>|[<span data-ttu-id="cfa7a-169">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="cfa7a-169">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="cfa7a-170">访问包分配的主题。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-170">The subject of the access package assignment.</span></span> <span data-ttu-id="cfa7a-171">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-171">Read-only.</span></span> <span data-ttu-id="cfa7a-172">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-172">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cfa7a-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cfa7a-173">JSON representation</span></span>

<span data-ttu-id="cfa7a-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cfa7a-174">The following is a JSON representation of the resource.</span></span>

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
