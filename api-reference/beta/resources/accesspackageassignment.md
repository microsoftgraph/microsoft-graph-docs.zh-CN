---
title: accessPackageAssignment 资源类型
description: 访问包分配是一段时间内特定主题的访问包的分配。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7147378e308faac7ca1fea931a465e1ea54f22ef
ms.sourcegitcommit: f51ba08d604d93f5f6af9ee8979cbf76baa285ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/19/2020
ms.locfileid: "42108446"
---
# <a name="accesspackageassignment-resource-type"></a><span data-ttu-id="ade1a-103">accessPackageAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="ade1a-103">accessPackageAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ade1a-104">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配是一段时间内特定主题的访问包分配。</span><span class="sxs-lookup"><span data-stu-id="ade1a-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment is an assignment of an access package to a particular subject, for a period of time.</span></span>  <span data-ttu-id="ade1a-105">例如，访问包分配可能表明用户 "Alice" 已通过访问包 "Sales" 在2019年1月到7月2019的阶段分配了访问权限。</span><span class="sxs-lookup"><span data-stu-id="ade1a-105">For example, an access package assignment could state that user 'Alice' has the been assigned access via the access package 'Sales' for the period January 2019 through July 2019.</span></span>

## <a name="methods"></a><span data-ttu-id="ade1a-106">方法</span><span class="sxs-lookup"><span data-stu-id="ade1a-106">Methods</span></span>

| <span data-ttu-id="ade1a-107">方法</span><span class="sxs-lookup"><span data-stu-id="ade1a-107">Method</span></span>       | <span data-ttu-id="ade1a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="ade1a-108">Return Type</span></span> | <span data-ttu-id="ade1a-109">说明</span><span class="sxs-lookup"><span data-stu-id="ade1a-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ade1a-110">列出 accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="ade1a-110">List accessPackageAssignments</span></span>](../api/accesspackageassignment-list.md) | <span data-ttu-id="ade1a-111">[accessPackageAssignment](accesspackageassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="ade1a-111">[accessPackageAssignment](accesspackageassignment.md) collection</span></span> | <span data-ttu-id="ade1a-112">检索**accesspackageassignment**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="ade1a-112">Retrieve a list of **accesspackageassignment** objects.</span></span> |

><span data-ttu-id="ade1a-113">**注意：** 不能使用方法来创建或删除访问包分配。</span><span class="sxs-lookup"><span data-stu-id="ade1a-113">**Note:** You can't use a method to create or remove an access package assignment.</span></span> <span data-ttu-id="ade1a-114">相反，要为用户请求访问包分配或从用户中删除访问包分配的客户端，可以[创建 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md)。</span><span class="sxs-lookup"><span data-stu-id="ade1a-114">Instead, a client that wants to request an access package assignment for a user, or remove an access package assignment from a user, can [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ade1a-115">属性</span><span class="sxs-lookup"><span data-stu-id="ade1a-115">Properties</span></span>

| <span data-ttu-id="ade1a-116">属性</span><span class="sxs-lookup"><span data-stu-id="ade1a-116">Property</span></span>     | <span data-ttu-id="ade1a-117">类型</span><span class="sxs-lookup"><span data-stu-id="ade1a-117">Type</span></span>        | <span data-ttu-id="ade1a-118">说明</span><span class="sxs-lookup"><span data-stu-id="ade1a-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ade1a-119">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="ade1a-119">accessPackageId</span></span>|<span data-ttu-id="ade1a-120">String</span><span class="sxs-lookup"><span data-stu-id="ade1a-120">String</span></span>|<span data-ttu-id="ade1a-121">访问包的标识符。</span><span class="sxs-lookup"><span data-stu-id="ade1a-121">The identifier of the access package.</span></span> <span data-ttu-id="ade1a-122">只读。</span><span class="sxs-lookup"><span data-stu-id="ade1a-122">Read-only.</span></span>|
|<span data-ttu-id="ade1a-123">assignmentPolicyId</span><span class="sxs-lookup"><span data-stu-id="ade1a-123">assignmentPolicyId</span></span>|<span data-ttu-id="ade1a-124">String</span><span class="sxs-lookup"><span data-stu-id="ade1a-124">String</span></span>|<span data-ttu-id="ade1a-125">访问包分配策略的标识符。</span><span class="sxs-lookup"><span data-stu-id="ade1a-125">The identifier of the access package assignment policy.</span></span> <span data-ttu-id="ade1a-126">只读。</span><span class="sxs-lookup"><span data-stu-id="ade1a-126">Read-only.</span></span>|
|<span data-ttu-id="ade1a-127">assignmentState</span><span class="sxs-lookup"><span data-stu-id="ade1a-127">assignmentState</span></span>|<span data-ttu-id="ade1a-128">String</span><span class="sxs-lookup"><span data-stu-id="ade1a-128">String</span></span>|<span data-ttu-id="ade1a-129">访问程序包的状态。</span><span class="sxs-lookup"><span data-stu-id="ade1a-129">The state of the access package.</span></span> <span data-ttu-id="ade1a-130">可能的值`Delivered`为`Expired`或。</span><span class="sxs-lookup"><span data-stu-id="ade1a-130">Possible values are `Delivered` or `Expired`.</span></span> <span data-ttu-id="ade1a-131">只读。</span><span class="sxs-lookup"><span data-stu-id="ade1a-131">Read-only.</span></span>|
|<span data-ttu-id="ade1a-132">assignmentStatus</span><span class="sxs-lookup"><span data-stu-id="ade1a-132">assignmentStatus</span></span>|<span data-ttu-id="ade1a-133">String</span><span class="sxs-lookup"><span data-stu-id="ade1a-133">String</span></span>|<span data-ttu-id="ade1a-134">只读。</span><span class="sxs-lookup"><span data-stu-id="ade1a-134">Read-only.</span></span>|
|<span data-ttu-id="ade1a-135">catalogId</span><span class="sxs-lookup"><span data-stu-id="ade1a-135">catalogId</span></span>|<span data-ttu-id="ade1a-136">String</span><span class="sxs-lookup"><span data-stu-id="ade1a-136">String</span></span>|<span data-ttu-id="ade1a-137">包含访问包的目录的标识符。</span><span class="sxs-lookup"><span data-stu-id="ade1a-137">The identifier of the catalog containing the access package.</span></span> <span data-ttu-id="ade1a-138">只读。</span><span class="sxs-lookup"><span data-stu-id="ade1a-138">Read-only.</span></span>|
|<span data-ttu-id="ade1a-139">expiredDateTime</span><span class="sxs-lookup"><span data-stu-id="ade1a-139">expiredDateTime</span></span>|<span data-ttu-id="ade1a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ade1a-140">DateTimeOffset</span></span>|<span data-ttu-id="ade1a-p107">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ade1a-p107">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ade1a-143">id</span><span class="sxs-lookup"><span data-stu-id="ade1a-143">id</span></span>|<span data-ttu-id="ade1a-144">String</span><span class="sxs-lookup"><span data-stu-id="ade1a-144">String</span></span>| <span data-ttu-id="ade1a-145">只读。</span><span class="sxs-lookup"><span data-stu-id="ade1a-145">Read-only.</span></span>|
|<span data-ttu-id="ade1a-146">isExtended</span><span class="sxs-lookup"><span data-stu-id="ade1a-146">isExtended</span></span>|<span data-ttu-id="ade1a-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="ade1a-147">Boolean</span></span>|<span data-ttu-id="ade1a-148">指示访问包分配是否已扩展。</span><span class="sxs-lookup"><span data-stu-id="ade1a-148">Indicates whether the access package assignment is extended.</span></span> <span data-ttu-id="ade1a-149">只读。</span><span class="sxs-lookup"><span data-stu-id="ade1a-149">Read-only.</span></span>|
|<span data-ttu-id="ade1a-150">targetId</span><span class="sxs-lookup"><span data-stu-id="ade1a-150">targetId</span></span>|<span data-ttu-id="ade1a-151">String</span><span class="sxs-lookup"><span data-stu-id="ade1a-151">String</span></span>| <span data-ttu-id="ade1a-152">包含工作分配的主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="ade1a-152">The ID of the subject with the assignment.</span></span> <span data-ttu-id="ade1a-153">只读。</span><span class="sxs-lookup"><span data-stu-id="ade1a-153">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ade1a-154">关系</span><span class="sxs-lookup"><span data-stu-id="ade1a-154">Relationships</span></span>

| <span data-ttu-id="ade1a-155">关系</span><span class="sxs-lookup"><span data-stu-id="ade1a-155">Relationship</span></span> | <span data-ttu-id="ade1a-156">类型</span><span class="sxs-lookup"><span data-stu-id="ade1a-156">Type</span></span>        | <span data-ttu-id="ade1a-157">说明</span><span class="sxs-lookup"><span data-stu-id="ade1a-157">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ade1a-158">accessPackage</span><span class="sxs-lookup"><span data-stu-id="ade1a-158">accessPackage</span></span>|[<span data-ttu-id="ade1a-159">accessPackage</span><span class="sxs-lookup"><span data-stu-id="ade1a-159">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="ade1a-160">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="ade1a-160">Read-only.</span></span> <span data-ttu-id="ade1a-161">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="ade1a-161">Nullable.</span></span>|
|<span data-ttu-id="ade1a-162">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="ade1a-162">accessPackageAssignmentPolicy</span></span>|[<span data-ttu-id="ade1a-163">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="ade1a-163">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md)| <span data-ttu-id="ade1a-164">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="ade1a-164">Read-only.</span></span> <span data-ttu-id="ade1a-165">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="ade1a-165">Nullable.</span></span>|
|<span data-ttu-id="ade1a-166">accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="ade1a-166">accessPackageAssignmentResourceRoles</span></span>|<span data-ttu-id="ade1a-167">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)集合</span><span class="sxs-lookup"><span data-stu-id="ade1a-167">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span>| <span data-ttu-id="ade1a-168">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="ade1a-168">Read-only.</span></span> <span data-ttu-id="ade1a-169">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="ade1a-169">Nullable.</span></span>|
|<span data-ttu-id="ade1a-170">target</span><span class="sxs-lookup"><span data-stu-id="ade1a-170">target</span></span>|[<span data-ttu-id="ade1a-171">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="ade1a-171">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="ade1a-172">访问包分配的主题。</span><span class="sxs-lookup"><span data-stu-id="ade1a-172">The subject of the access package assignment.</span></span> <span data-ttu-id="ade1a-173">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="ade1a-173">Read-only.</span></span> <span data-ttu-id="ade1a-174">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="ade1a-174">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ade1a-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ade1a-175">JSON representation</span></span>

<span data-ttu-id="ade1a-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ade1a-176">The following is a JSON representation of the resource.</span></span>

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
