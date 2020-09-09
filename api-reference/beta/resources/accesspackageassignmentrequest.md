---
title: accessPackageAssignmentRequest 资源类型
description: 访问包分配请求由要获取访问包分配的用户创建。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3a3309df4106d30de2190b1c321adb3ea0b1a670
ms.sourcegitcommit: 01f73b4dce6f885da18d62fe800b387c286c7a8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/09/2020
ms.locfileid: "47413308"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="8cb43-103">accessPackageAssignmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="8cb43-103">accessPackageAssignmentRequest resource type</span></span>

<span data-ttu-id="8cb43-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cb43-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cb43-105">在 [AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配请求是由要获取访问包分配的用户创建或代表的。</span><span class="sxs-lookup"><span data-stu-id="8cb43-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by or on behalf of a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="8cb43-106">如果请求成功，并且具有必要的审批，则用户将收到访问包分配，并且是最终的访问包分配的主题。</span><span class="sxs-lookup"><span data-stu-id="8cb43-106">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>  <span data-ttu-id="8cb43-107">Azure AD 还会自动创建访问包分配请求，以用于跟踪访问删除。</span><span class="sxs-lookup"><span data-stu-id="8cb43-107">Azure AD also creates access package assignment requests automatically for tracking access removal.</span></span>

## <a name="methods"></a><span data-ttu-id="8cb43-108">方法</span><span class="sxs-lookup"><span data-stu-id="8cb43-108">Methods</span></span>

| <span data-ttu-id="8cb43-109">方法</span><span class="sxs-lookup"><span data-stu-id="8cb43-109">Method</span></span>       | <span data-ttu-id="8cb43-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="8cb43-110">Return Type</span></span> | <span data-ttu-id="8cb43-111">说明</span><span class="sxs-lookup"><span data-stu-id="8cb43-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8cb43-112">列出 accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="8cb43-112">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="8cb43-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8cb43-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="8cb43-114">检索 accesspackageassignmentrequest 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="8cb43-114">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="8cb43-115">创建 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="8cb43-115">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="8cb43-116">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="8cb43-116">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="8cb43-117">创建新的 accessPackageAssignmentRequest。</span><span class="sxs-lookup"><span data-stu-id="8cb43-117">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="8cb43-118">获取 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="8cb43-118">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="8cb43-119">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="8cb43-119">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="8cb43-120">读取 accessPackageAssignmentRequest 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8cb43-120">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8cb43-121">属性</span><span class="sxs-lookup"><span data-stu-id="8cb43-121">Properties</span></span>

| <span data-ttu-id="8cb43-122">属性</span><span class="sxs-lookup"><span data-stu-id="8cb43-122">Property</span></span>     | <span data-ttu-id="8cb43-123">类型</span><span class="sxs-lookup"><span data-stu-id="8cb43-123">Type</span></span>        | <span data-ttu-id="8cb43-124">说明</span><span class="sxs-lookup"><span data-stu-id="8cb43-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8cb43-125">completedDate</span><span class="sxs-lookup"><span data-stu-id="8cb43-125">completedDate</span></span>|<span data-ttu-id="8cb43-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cb43-126">DateTimeOffset</span></span>|<span data-ttu-id="8cb43-127">请求的处理结束日期（成功或失败）。</span><span class="sxs-lookup"><span data-stu-id="8cb43-127">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="8cb43-128">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="8cb43-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8cb43-129">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="8cb43-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="8cb43-130">只读。</span><span class="sxs-lookup"><span data-stu-id="8cb43-130">Read-only.</span></span>|
|<span data-ttu-id="8cb43-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8cb43-131">createdDateTime</span></span>|<span data-ttu-id="8cb43-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cb43-132">DateTimeOffset</span></span>|<span data-ttu-id="8cb43-133">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="8cb43-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8cb43-134">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="8cb43-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="8cb43-135">只读。</span><span class="sxs-lookup"><span data-stu-id="8cb43-135">Read-only.</span></span>|
|<span data-ttu-id="8cb43-136">id</span><span class="sxs-lookup"><span data-stu-id="8cb43-136">id</span></span>|<span data-ttu-id="8cb43-137">String</span><span class="sxs-lookup"><span data-stu-id="8cb43-137">String</span></span>| <span data-ttu-id="8cb43-138">只读。</span><span class="sxs-lookup"><span data-stu-id="8cb43-138">Read-only.</span></span>|
|<span data-ttu-id="8cb43-139">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="8cb43-139">isValidationOnly</span></span>|<span data-ttu-id="8cb43-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cb43-140">Boolean</span></span>|<span data-ttu-id="8cb43-141">如果请求不处理工作分配，则为 True。</span><span class="sxs-lookup"><span data-stu-id="8cb43-141">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="8cb43-142">合理化</span><span class="sxs-lookup"><span data-stu-id="8cb43-142">justification</span></span>|<span data-ttu-id="8cb43-143">String</span><span class="sxs-lookup"><span data-stu-id="8cb43-143">String</span></span>|<span data-ttu-id="8cb43-144">请求者提供的理由。</span><span class="sxs-lookup"><span data-stu-id="8cb43-144">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="8cb43-145">requestState</span><span class="sxs-lookup"><span data-stu-id="8cb43-145">requestState</span></span>|<span data-ttu-id="8cb43-146">String</span><span class="sxs-lookup"><span data-stu-id="8cb43-146">String</span></span>|<span data-ttu-id="8cb43-147">、、、、、或中的一个 `PendingApproval` `Canceled`  `Denied` `Delivering` `Delivered` `PartiallyDelivered` `Submitted` `Scheduled` 。</span><span class="sxs-lookup"><span data-stu-id="8cb43-147">One of `PendingApproval`, `Canceled`,  `Denied`, `Delivering`, `Delivered`, `PartiallyDelivered`, `Submitted` or `Scheduled`.</span></span> <span data-ttu-id="8cb43-148">只读。</span><span class="sxs-lookup"><span data-stu-id="8cb43-148">Read-only.</span></span>|
|<span data-ttu-id="8cb43-149">requestStatus</span><span class="sxs-lookup"><span data-stu-id="8cb43-149">requestStatus</span></span>|<span data-ttu-id="8cb43-150">String</span><span class="sxs-lookup"><span data-stu-id="8cb43-150">String</span></span>|<span data-ttu-id="8cb43-151">有关请求处理状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8cb43-151">More information on the request processing status.</span></span> <span data-ttu-id="8cb43-152">只读。</span><span class="sxs-lookup"><span data-stu-id="8cb43-152">Read-only.</span></span>|
|<span data-ttu-id="8cb43-153">requestType</span><span class="sxs-lookup"><span data-stu-id="8cb43-153">requestType</span></span>|<span data-ttu-id="8cb43-154">String</span><span class="sxs-lookup"><span data-stu-id="8cb43-154">String</span></span>|<span data-ttu-id="8cb43-155">、、或的其中一个 `UserAdd` `UserRemove` `AdminAdd` `AdminRemove` `SystemRemove` 。</span><span class="sxs-lookup"><span data-stu-id="8cb43-155">One of `UserAdd`, `UserRemove`, `AdminAdd`, `AdminRemove` or `SystemRemove`.</span></span> <span data-ttu-id="8cb43-156">来自用户自身的请求将对或进行 requestType `UserAdd` `UserRemove` 。</span><span class="sxs-lookup"><span data-stu-id="8cb43-156">A request from the user themselves would have requestType of `UserAdd` or `UserRemove`.</span></span> <span data-ttu-id="8cb43-157">只读。</span><span class="sxs-lookup"><span data-stu-id="8cb43-157">Read-only.</span></span>|
|<span data-ttu-id="8cb43-158">schedule</span><span class="sxs-lookup"><span data-stu-id="8cb43-158">schedule</span></span>|[<span data-ttu-id="8cb43-159">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="8cb43-159">requestSchedule</span></span>](requestschedule.md)| <span data-ttu-id="8cb43-160">要将访问权限分配给请求者的日期范围。</span><span class="sxs-lookup"><span data-stu-id="8cb43-160">The range of dates that access is to be assigned to the requestor.</span></span> <span data-ttu-id="8cb43-161">只读。</span><span class="sxs-lookup"><span data-stu-id="8cb43-161">Read-only.</span></span>|
|<span data-ttu-id="8cb43-162">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="8cb43-162">accessPackageAssignment</span></span>|[<span data-ttu-id="8cb43-163">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="8cb43-163">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="8cb43-164">对于或的 requestType `UserAdd` `AdminAdd` ，这是请求创建的访问包分配。</span><span class="sxs-lookup"><span data-stu-id="8cb43-164">For a requestType of `UserAdd` or `AdminAdd`, this is an access package assignment requested to be created.</span></span>  <span data-ttu-id="8cb43-165">对于的 requestType `UserRemove` `AdminRemove` 或 `SystemRemove` ，它具有 `id` 要删除的现有工作分配的属性。</span><span class="sxs-lookup"><span data-stu-id="8cb43-165">For a requestType of `UserRemove`, `AdminRemove` or `SystemRemove`, this has the `id` property of an existing assignment to be removed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cb43-166">关系</span><span class="sxs-lookup"><span data-stu-id="8cb43-166">Relationships</span></span>

| <span data-ttu-id="8cb43-167">关系</span><span class="sxs-lookup"><span data-stu-id="8cb43-167">Relationship</span></span> | <span data-ttu-id="8cb43-168">类型</span><span class="sxs-lookup"><span data-stu-id="8cb43-168">Type</span></span>        | <span data-ttu-id="8cb43-169">说明</span><span class="sxs-lookup"><span data-stu-id="8cb43-169">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8cb43-170">请求程序</span><span class="sxs-lookup"><span data-stu-id="8cb43-170">requestor</span></span>|[<span data-ttu-id="8cb43-171">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="8cb43-171">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="8cb43-172">分配了请求的主题或分配了直接分配的主题。</span><span class="sxs-lookup"><span data-stu-id="8cb43-172">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="8cb43-173">只读。</span><span class="sxs-lookup"><span data-stu-id="8cb43-173">Read-only.</span></span> <span data-ttu-id="8cb43-174">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8cb43-174">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8cb43-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8cb43-175">JSON representation</span></span>

<span data-ttu-id="8cb43-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8cb43-176">The following is a JSON representation of the resource.</span></span>

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
