---
title: accessPackageAssignmentRequest 资源类型
description: 访问包分配请求由要获取访问包分配的用户创建。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c2440dfc7e798ea5b0a197f60b62acce4199b4ca
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331267"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="b0a3a-103">accessPackageAssignmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="b0a3a-103">accessPackageAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0a3a-104">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配请求由要获取访问包分配的用户创建。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="b0a3a-105">如果请求成功，并且具有必要的审批，则用户将收到访问包分配，并且是最终的访问包分配的主题。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-105">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>  <span data-ttu-id="b0a3a-106">Azure AD 还会自动创建访问包分配请求，以用于跟踪访问删除。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-106">Azure AD also creates access package assignment requests automatically for tracking access removal.</span></span>


## <a name="methods"></a><span data-ttu-id="b0a3a-107">Methods</span><span class="sxs-lookup"><span data-stu-id="b0a3a-107">Methods</span></span>

| <span data-ttu-id="b0a3a-108">方法</span><span class="sxs-lookup"><span data-stu-id="b0a3a-108">Method</span></span>       | <span data-ttu-id="b0a3a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b0a3a-109">Return Type</span></span> | <span data-ttu-id="b0a3a-110">说明</span><span class="sxs-lookup"><span data-stu-id="b0a3a-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b0a3a-111">列出 accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="b0a3a-111">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="b0a3a-112">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="b0a3a-112">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="b0a3a-113">检索 accesspackageassignmentrequest 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-113">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="b0a3a-114">创建 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="b0a3a-114">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="b0a3a-115">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="b0a3a-115">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="b0a3a-116">创建新的 accessPackageAssignmentRequest。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-116">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="b0a3a-117">获取 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="b0a3a-117">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="b0a3a-118">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="b0a3a-118">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="b0a3a-119">读取 accessPackageAssignmentRequest 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-119">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b0a3a-120">属性</span><span class="sxs-lookup"><span data-stu-id="b0a3a-120">Properties</span></span>

| <span data-ttu-id="b0a3a-121">属性</span><span class="sxs-lookup"><span data-stu-id="b0a3a-121">Property</span></span>     | <span data-ttu-id="b0a3a-122">类型</span><span class="sxs-lookup"><span data-stu-id="b0a3a-122">Type</span></span>        | <span data-ttu-id="b0a3a-123">说明</span><span class="sxs-lookup"><span data-stu-id="b0a3a-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b0a3a-124">completedDate</span><span class="sxs-lookup"><span data-stu-id="b0a3a-124">completedDate</span></span>|<span data-ttu-id="b0a3a-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0a3a-125">DateTimeOffset</span></span>|<span data-ttu-id="b0a3a-126">请求的处理结束日期（成功或失败）。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-126">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="b0a3a-127">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b0a3a-128">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="b0a3a-129">只读。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-129">Read-only.</span></span>|
|<span data-ttu-id="b0a3a-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0a3a-130">createdDateTime</span></span>|<span data-ttu-id="b0a3a-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0a3a-131">DateTimeOffset</span></span>|<span data-ttu-id="b0a3a-132">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-132">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b0a3a-133">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-133">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="b0a3a-134">只读。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-134">Read-only.</span></span>|
|<span data-ttu-id="b0a3a-135">id</span><span class="sxs-lookup"><span data-stu-id="b0a3a-135">id</span></span>|<span data-ttu-id="b0a3a-136">String</span><span class="sxs-lookup"><span data-stu-id="b0a3a-136">String</span></span>| <span data-ttu-id="b0a3a-137">只读。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-137">Read-only.</span></span>|
|<span data-ttu-id="b0a3a-138">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="b0a3a-138">isValidationOnly</span></span>|<span data-ttu-id="b0a3a-139">布尔值</span><span class="sxs-lookup"><span data-stu-id="b0a3a-139">Boolean</span></span>|<span data-ttu-id="b0a3a-140">如果请求不处理工作分配，则为 True。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-140">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="b0a3a-141">合理化</span><span class="sxs-lookup"><span data-stu-id="b0a3a-141">justification</span></span>|<span data-ttu-id="b0a3a-142">String</span><span class="sxs-lookup"><span data-stu-id="b0a3a-142">String</span></span>|<span data-ttu-id="b0a3a-143">请求者提供的理由。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-143">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="b0a3a-144">requestState</span><span class="sxs-lookup"><span data-stu-id="b0a3a-144">requestState</span></span>|<span data-ttu-id="b0a3a-145">String</span><span class="sxs-lookup"><span data-stu-id="b0a3a-145">String</span></span>|<span data-ttu-id="b0a3a-146">、 `Denied` `Delivered` `Submitted` 、或`Scheduled`的其中`PartiallyDelivered`一个。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-146">One of `Denied`, `Delivered`, `PartiallyDelivered`, `Submitted` or `Scheduled`.</span></span> <span data-ttu-id="b0a3a-147">只读。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-147">Read-only.</span></span>|
|<span data-ttu-id="b0a3a-148">requestStatus</span><span class="sxs-lookup"><span data-stu-id="b0a3a-148">requestStatus</span></span>|<span data-ttu-id="b0a3a-149">String</span><span class="sxs-lookup"><span data-stu-id="b0a3a-149">String</span></span>|<span data-ttu-id="b0a3a-150">有关请求处理状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-150">More information on the request processing status.</span></span> <span data-ttu-id="b0a3a-151">只读。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-151">Read-only.</span></span>|
|<span data-ttu-id="b0a3a-152">requestType</span><span class="sxs-lookup"><span data-stu-id="b0a3a-152">requestType</span></span>|<span data-ttu-id="b0a3a-153">String</span><span class="sxs-lookup"><span data-stu-id="b0a3a-153">String</span></span>|<span data-ttu-id="b0a3a-154">、 `UserAdd` `UserRemove` `AdminRemove` 、或`SystemRemove`的其中`AdminAdd`一个。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-154">One of `UserAdd`, `UserRemove`, `AdminAdd`, `AdminRemove` or `SystemRemove`.</span></span> <span data-ttu-id="b0a3a-155">只读。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-155">Read-only.</span></span>|
|<span data-ttu-id="b0a3a-156">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="b0a3a-156">accessPackageAssignment</span></span>|[<span data-ttu-id="b0a3a-157">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="b0a3a-157">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="b0a3a-158">请求创建的访问包分配。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-158">An access package assignment requested to be created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0a3a-159">关系</span><span class="sxs-lookup"><span data-stu-id="b0a3a-159">Relationships</span></span>

| <span data-ttu-id="b0a3a-160">关系</span><span class="sxs-lookup"><span data-stu-id="b0a3a-160">Relationship</span></span> | <span data-ttu-id="b0a3a-161">类型</span><span class="sxs-lookup"><span data-stu-id="b0a3a-161">Type</span></span>        | <span data-ttu-id="b0a3a-162">说明</span><span class="sxs-lookup"><span data-stu-id="b0a3a-162">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b0a3a-163">请求程序</span><span class="sxs-lookup"><span data-stu-id="b0a3a-163">requestor</span></span>|[<span data-ttu-id="b0a3a-164">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="b0a3a-164">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="b0a3a-165">分配了请求的主题或分配了直接分配的主题。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-165">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="b0a3a-166">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-166">Read-only.</span></span> <span data-ttu-id="b0a3a-167">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-167">Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b0a3a-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0a3a-168">JSON representation</span></span>

<span data-ttu-id="b0a3a-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0a3a-169">The following is a JSON representation of the resource.</span></span>

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
