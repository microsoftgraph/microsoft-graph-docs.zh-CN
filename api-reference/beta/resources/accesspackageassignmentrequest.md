---
title: accessPackageAssignmentRequest 资源类型
description: 访问包分配请求由要获取访问包分配的用户创建。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0fd9f5ea9cd15abac7eea693b2af5c595b145ac7
ms.sourcegitcommit: f51ba08d604d93f5f6af9ee8979cbf76baa285ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/19/2020
ms.locfileid: "42108439"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="91b49-103">accessPackageAssignmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="91b49-103">accessPackageAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91b49-104">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配请求由要获取访问包分配的用户创建。</span><span class="sxs-lookup"><span data-stu-id="91b49-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="91b49-105">如果请求成功，并且具有必要的审批，则用户将收到访问包分配，并且是最终的访问包分配的主题。</span><span class="sxs-lookup"><span data-stu-id="91b49-105">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>


## <a name="methods"></a><span data-ttu-id="91b49-106">方法</span><span class="sxs-lookup"><span data-stu-id="91b49-106">Methods</span></span>

| <span data-ttu-id="91b49-107">方法</span><span class="sxs-lookup"><span data-stu-id="91b49-107">Method</span></span>       | <span data-ttu-id="91b49-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="91b49-108">Return Type</span></span> | <span data-ttu-id="91b49-109">说明</span><span class="sxs-lookup"><span data-stu-id="91b49-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="91b49-110">列出 accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="91b49-110">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="91b49-111">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="91b49-111">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="91b49-112">检索 accesspackageassignmentrequest 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="91b49-112">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="91b49-113">创建 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="91b49-113">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="91b49-114">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="91b49-114">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="91b49-115">创建新的 accessPackageAssignmentRequest。</span><span class="sxs-lookup"><span data-stu-id="91b49-115">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="91b49-116">获取 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="91b49-116">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="91b49-117">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="91b49-117">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="91b49-118">读取 accessPackageAssignmentRequest 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="91b49-118">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="91b49-119">属性</span><span class="sxs-lookup"><span data-stu-id="91b49-119">Properties</span></span>

| <span data-ttu-id="91b49-120">属性</span><span class="sxs-lookup"><span data-stu-id="91b49-120">Property</span></span>     | <span data-ttu-id="91b49-121">类型</span><span class="sxs-lookup"><span data-stu-id="91b49-121">Type</span></span>        | <span data-ttu-id="91b49-122">说明</span><span class="sxs-lookup"><span data-stu-id="91b49-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="91b49-123">completedDate</span><span class="sxs-lookup"><span data-stu-id="91b49-123">completedDate</span></span>|<span data-ttu-id="91b49-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91b49-124">DateTimeOffset</span></span>|<span data-ttu-id="91b49-125">请求的处理结束日期（成功或失败）。</span><span class="sxs-lookup"><span data-stu-id="91b49-125">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="91b49-126">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="91b49-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="91b49-127">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="91b49-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="91b49-128">只读。</span><span class="sxs-lookup"><span data-stu-id="91b49-128">Read-only.</span></span>|
|<span data-ttu-id="91b49-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="91b49-129">createdDateTime</span></span>|<span data-ttu-id="91b49-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91b49-130">DateTimeOffset</span></span>|<span data-ttu-id="91b49-131">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="91b49-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="91b49-132">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="91b49-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="91b49-133">只读。</span><span class="sxs-lookup"><span data-stu-id="91b49-133">Read-only.</span></span>|
|<span data-ttu-id="91b49-134">id</span><span class="sxs-lookup"><span data-stu-id="91b49-134">id</span></span>|<span data-ttu-id="91b49-135">String</span><span class="sxs-lookup"><span data-stu-id="91b49-135">String</span></span>| <span data-ttu-id="91b49-136">只读。</span><span class="sxs-lookup"><span data-stu-id="91b49-136">Read-only.</span></span>|
|<span data-ttu-id="91b49-137">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="91b49-137">isValidationOnly</span></span>|<span data-ttu-id="91b49-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="91b49-138">Boolean</span></span>|<span data-ttu-id="91b49-139">如果请求不处理工作分配，则为 True。</span><span class="sxs-lookup"><span data-stu-id="91b49-139">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="91b49-140">合理化</span><span class="sxs-lookup"><span data-stu-id="91b49-140">justification</span></span>|<span data-ttu-id="91b49-141">String</span><span class="sxs-lookup"><span data-stu-id="91b49-141">String</span></span>|<span data-ttu-id="91b49-142">请求者提供的理由。</span><span class="sxs-lookup"><span data-stu-id="91b49-142">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="91b49-143">requestState</span><span class="sxs-lookup"><span data-stu-id="91b49-143">requestState</span></span>|<span data-ttu-id="91b49-144">String</span><span class="sxs-lookup"><span data-stu-id="91b49-144">String</span></span>|<span data-ttu-id="91b49-145">、 `Denied` `Delivered`、 `PartiallyDelivered`或`Submitted`中的一个。</span><span class="sxs-lookup"><span data-stu-id="91b49-145">One of `Denied`, `Delivered`, `PartiallyDelivered` or `Submitted`.</span></span> <span data-ttu-id="91b49-146">只读。</span><span class="sxs-lookup"><span data-stu-id="91b49-146">Read-only.</span></span>|
|<span data-ttu-id="91b49-147">requestStatus</span><span class="sxs-lookup"><span data-stu-id="91b49-147">requestStatus</span></span>|<span data-ttu-id="91b49-148">String</span><span class="sxs-lookup"><span data-stu-id="91b49-148">String</span></span>|<span data-ttu-id="91b49-149">有关请求处理状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="91b49-149">More information on the request processing status.</span></span> <span data-ttu-id="91b49-150">只读。</span><span class="sxs-lookup"><span data-stu-id="91b49-150">Read-only.</span></span>|
|<span data-ttu-id="91b49-151">requestType</span><span class="sxs-lookup"><span data-stu-id="91b49-151">requestType</span></span>|<span data-ttu-id="91b49-152">String</span><span class="sxs-lookup"><span data-stu-id="91b49-152">String</span></span>|<span data-ttu-id="91b49-153">、 `UserAdd` `UserRemove`、 `AdminAdd`或`AdminRemove`中的一个。</span><span class="sxs-lookup"><span data-stu-id="91b49-153">One of `UserAdd`, `UserRemove`, `AdminAdd` or `AdminRemove`.</span></span> <span data-ttu-id="91b49-154">只读。</span><span class="sxs-lookup"><span data-stu-id="91b49-154">Read-only.</span></span>|
|<span data-ttu-id="91b49-155">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="91b49-155">accessPackageAssignment</span></span>|[<span data-ttu-id="91b49-156">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="91b49-156">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="91b49-157">请求创建的访问包分配。</span><span class="sxs-lookup"><span data-stu-id="91b49-157">An access package assignment requested to be created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91b49-158">关系</span><span class="sxs-lookup"><span data-stu-id="91b49-158">Relationships</span></span>

| <span data-ttu-id="91b49-159">关系</span><span class="sxs-lookup"><span data-stu-id="91b49-159">Relationship</span></span> | <span data-ttu-id="91b49-160">类型</span><span class="sxs-lookup"><span data-stu-id="91b49-160">Type</span></span>        | <span data-ttu-id="91b49-161">说明</span><span class="sxs-lookup"><span data-stu-id="91b49-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="91b49-162">请求程序</span><span class="sxs-lookup"><span data-stu-id="91b49-162">requestor</span></span>|[<span data-ttu-id="91b49-163">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="91b49-163">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="91b49-164">分配了请求的主题或分配了直接分配的主题。</span><span class="sxs-lookup"><span data-stu-id="91b49-164">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="91b49-165">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="91b49-165">Read-only.</span></span> <span data-ttu-id="91b49-166">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="91b49-166">Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="91b49-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91b49-167">JSON representation</span></span>

<span data-ttu-id="91b49-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91b49-168">The following is a JSON representation of the resource.</span></span>

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
