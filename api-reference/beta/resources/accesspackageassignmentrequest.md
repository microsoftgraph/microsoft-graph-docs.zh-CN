---
title: accessPackageAssignmentRequest 资源类型
description: 访问包分配请求由要获取访问包分配的用户创建。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 11b3095bf54f6d5ffe1af4ca4926fe4409429b48
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319531"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="4c0b9-103">accessPackageAssignmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="4c0b9-103">accessPackageAssignmentRequest resource type</span></span>

<span data-ttu-id="4c0b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c0b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c0b9-105">在 [AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配请求是由要获取访问包分配的用户创建或代表的。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by or on behalf of a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="4c0b9-106">如果请求成功，并且具有必要的审批，则用户将收到访问包分配，并且是最终的访问包分配的主题。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-106">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>  <span data-ttu-id="4c0b9-107">Azure AD 还会自动创建访问包分配请求，以用于跟踪访问删除。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-107">Azure AD also creates access package assignment requests automatically for tracking access removal.</span></span>

## <a name="methods"></a><span data-ttu-id="4c0b9-108">方法</span><span class="sxs-lookup"><span data-stu-id="4c0b9-108">Methods</span></span>

| <span data-ttu-id="4c0b9-109">方法</span><span class="sxs-lookup"><span data-stu-id="4c0b9-109">Method</span></span>       | <span data-ttu-id="4c0b9-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="4c0b9-110">Return Type</span></span> | <span data-ttu-id="4c0b9-111">说明</span><span class="sxs-lookup"><span data-stu-id="4c0b9-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4c0b9-112">列出 accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="4c0b9-112">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="4c0b9-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4c0b9-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="4c0b9-114">检索 accesspackageassignmentrequest 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-114">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="4c0b9-115">创建 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="4c0b9-115">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="4c0b9-116">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="4c0b9-116">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="4c0b9-117">创建新的 accessPackageAssignmentRequest。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-117">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="4c0b9-118">获取 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="4c0b9-118">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="4c0b9-119">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="4c0b9-119">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="4c0b9-120">读取 accessPackageAssignmentRequest 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-120">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4c0b9-121">属性</span><span class="sxs-lookup"><span data-stu-id="4c0b9-121">Properties</span></span>

| <span data-ttu-id="4c0b9-122">属性</span><span class="sxs-lookup"><span data-stu-id="4c0b9-122">Property</span></span>     | <span data-ttu-id="4c0b9-123">类型</span><span class="sxs-lookup"><span data-stu-id="4c0b9-123">Type</span></span>        | <span data-ttu-id="4c0b9-124">说明</span><span class="sxs-lookup"><span data-stu-id="4c0b9-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4c0b9-125">completedDate</span><span class="sxs-lookup"><span data-stu-id="4c0b9-125">completedDate</span></span>|<span data-ttu-id="4c0b9-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c0b9-126">DateTimeOffset</span></span>|<span data-ttu-id="4c0b9-127">请求的处理结束日期（成功或失败）。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-127">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="4c0b9-128">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4c0b9-129">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="4c0b9-130">只读。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-130">Read-only.</span></span>|
|<span data-ttu-id="4c0b9-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4c0b9-131">createdDateTime</span></span>|<span data-ttu-id="4c0b9-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c0b9-132">DateTimeOffset</span></span>|<span data-ttu-id="4c0b9-133">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4c0b9-134">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="4c0b9-135">只读。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-135">Read-only.</span></span>|
|<span data-ttu-id="4c0b9-136">id</span><span class="sxs-lookup"><span data-stu-id="4c0b9-136">id</span></span>|<span data-ttu-id="4c0b9-137">String</span><span class="sxs-lookup"><span data-stu-id="4c0b9-137">String</span></span>| <span data-ttu-id="4c0b9-138">只读。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-138">Read-only.</span></span>|
|<span data-ttu-id="4c0b9-139">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="4c0b9-139">isValidationOnly</span></span>|<span data-ttu-id="4c0b9-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c0b9-140">Boolean</span></span>|<span data-ttu-id="4c0b9-141">如果请求不处理工作分配，则为 True。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-141">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="4c0b9-142">合理化</span><span class="sxs-lookup"><span data-stu-id="4c0b9-142">justification</span></span>|<span data-ttu-id="4c0b9-143">String</span><span class="sxs-lookup"><span data-stu-id="4c0b9-143">String</span></span>|<span data-ttu-id="4c0b9-144">请求者提供的理由。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-144">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="4c0b9-145">requestState</span><span class="sxs-lookup"><span data-stu-id="4c0b9-145">requestState</span></span>|<span data-ttu-id="4c0b9-146">String</span><span class="sxs-lookup"><span data-stu-id="4c0b9-146">String</span></span>|<span data-ttu-id="4c0b9-147">、、、、、或中的一个 `PendingApproval` `Canceled`  `Denied` `Delivering` `Delivered` `PartiallyDelivered` `Submitted` `Scheduled` 。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-147">One of `PendingApproval`, `Canceled`,  `Denied`, `Delivering`, `Delivered`, `PartiallyDelivered`, `Submitted` or `Scheduled`.</span></span> <span data-ttu-id="4c0b9-148">只读。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-148">Read-only.</span></span>|
|<span data-ttu-id="4c0b9-149">requestStatus</span><span class="sxs-lookup"><span data-stu-id="4c0b9-149">requestStatus</span></span>|<span data-ttu-id="4c0b9-150">String</span><span class="sxs-lookup"><span data-stu-id="4c0b9-150">String</span></span>|<span data-ttu-id="4c0b9-151">有关请求处理状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-151">More information on the request processing status.</span></span> <span data-ttu-id="4c0b9-152">只读。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-152">Read-only.</span></span>|
|<span data-ttu-id="4c0b9-153">requestType</span><span class="sxs-lookup"><span data-stu-id="4c0b9-153">requestType</span></span>|<span data-ttu-id="4c0b9-154">String</span><span class="sxs-lookup"><span data-stu-id="4c0b9-154">String</span></span>|<span data-ttu-id="4c0b9-155">、、或的其中一个 `UserAdd` `UserRemove` `AdminAdd` `AdminRemove` `SystemRemove` 。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-155">One of `UserAdd`, `UserRemove`, `AdminAdd`, `AdminRemove` or `SystemRemove`.</span></span> <span data-ttu-id="4c0b9-156">来自用户自身的请求将对或进行 requestType `UserAdd` `UserRemove` 。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-156">A request from the user themselves would have requestType of `UserAdd` or `UserRemove`.</span></span> <span data-ttu-id="4c0b9-157">只读。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-157">Read-only.</span></span>|
|<span data-ttu-id="4c0b9-158">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="4c0b9-158">accessPackageAssignment</span></span>|[<span data-ttu-id="4c0b9-159">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="4c0b9-159">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="4c0b9-160">对于或的 requestType `UserAdd` `AdminAdd` ，这是请求创建的访问包分配。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-160">For a requestType of `UserAdd` or `AdminAdd`, this is an access package assignment requested to be created.</span></span>  <span data-ttu-id="4c0b9-161">对于的 requestType `UserRemove` `AdminRemove` 或 `SystemRemove` ，它具有 `id` 要删除的现有工作分配的属性。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-161">For a requestType of `UserRemove`, `AdminRemove` or `SystemRemove`, this has the `id` property of an existing assignment to be removed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c0b9-162">关系</span><span class="sxs-lookup"><span data-stu-id="4c0b9-162">Relationships</span></span>

| <span data-ttu-id="4c0b9-163">关系</span><span class="sxs-lookup"><span data-stu-id="4c0b9-163">Relationship</span></span> | <span data-ttu-id="4c0b9-164">类型</span><span class="sxs-lookup"><span data-stu-id="4c0b9-164">Type</span></span>        | <span data-ttu-id="4c0b9-165">说明</span><span class="sxs-lookup"><span data-stu-id="4c0b9-165">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4c0b9-166">请求程序</span><span class="sxs-lookup"><span data-stu-id="4c0b9-166">requestor</span></span>|[<span data-ttu-id="4c0b9-167">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="4c0b9-167">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="4c0b9-168">分配了请求的主题或分配了直接分配的主题。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-168">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="4c0b9-169">只读。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-169">Read-only.</span></span> <span data-ttu-id="4c0b9-170">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-170">Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="4c0b9-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4c0b9-171">JSON representation</span></span>

<span data-ttu-id="4c0b9-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c0b9-172">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "2020-02-12T22:06:58.303Z",
  "completedDate": "2020-02-12T22:14:28.19Z",
  "id": "1244d439-5baa-4b9a-be5f-e8fdef5a998b",
  "requestType": "UserAdd",
  "requestState": "Delivered",
  "requestStatus": "FulfilledNotificationTriggered",
  "isValidationOnly": false,
  "justification": ""
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
