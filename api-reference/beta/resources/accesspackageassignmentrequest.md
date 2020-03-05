---
title: accessPackageAssignmentRequest 资源类型
description: 访问包分配请求由要获取访问包分配的用户创建。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7d7fcf663abf15478b0c2745e9c60e1021d1ee7b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508546"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="f4421-103">accessPackageAssignmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="f4421-103">accessPackageAssignmentRequest resource type</span></span>

<span data-ttu-id="f4421-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f4421-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4421-105">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配请求由要获取访问包分配的用户创建。</span><span class="sxs-lookup"><span data-stu-id="f4421-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="f4421-106">如果请求成功，并且具有必要的审批，则用户将收到访问包分配，并且是最终的访问包分配的主题。</span><span class="sxs-lookup"><span data-stu-id="f4421-106">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>  <span data-ttu-id="f4421-107">Azure AD 还会自动创建访问包分配请求，以用于跟踪访问删除。</span><span class="sxs-lookup"><span data-stu-id="f4421-107">Azure AD also creates access package assignment requests automatically for tracking access removal.</span></span>


## <a name="methods"></a><span data-ttu-id="f4421-108">方法</span><span class="sxs-lookup"><span data-stu-id="f4421-108">Methods</span></span>

| <span data-ttu-id="f4421-109">方法</span><span class="sxs-lookup"><span data-stu-id="f4421-109">Method</span></span>       | <span data-ttu-id="f4421-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f4421-110">Return Type</span></span> | <span data-ttu-id="f4421-111">说明</span><span class="sxs-lookup"><span data-stu-id="f4421-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f4421-112">列出 accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="f4421-112">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="f4421-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="f4421-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="f4421-114">检索 accesspackageassignmentrequest 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="f4421-114">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="f4421-115">创建 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f4421-115">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="f4421-116">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f4421-116">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="f4421-117">创建新的 accessPackageAssignmentRequest。</span><span class="sxs-lookup"><span data-stu-id="f4421-117">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="f4421-118">获取 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f4421-118">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="f4421-119">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f4421-119">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="f4421-120">读取 accessPackageAssignmentRequest 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f4421-120">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f4421-121">属性</span><span class="sxs-lookup"><span data-stu-id="f4421-121">Properties</span></span>

| <span data-ttu-id="f4421-122">属性</span><span class="sxs-lookup"><span data-stu-id="f4421-122">Property</span></span>     | <span data-ttu-id="f4421-123">类型</span><span class="sxs-lookup"><span data-stu-id="f4421-123">Type</span></span>        | <span data-ttu-id="f4421-124">说明</span><span class="sxs-lookup"><span data-stu-id="f4421-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f4421-125">completedDate</span><span class="sxs-lookup"><span data-stu-id="f4421-125">completedDate</span></span>|<span data-ttu-id="f4421-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4421-126">DateTimeOffset</span></span>|<span data-ttu-id="f4421-127">请求的处理结束日期（成功或失败）。</span><span class="sxs-lookup"><span data-stu-id="f4421-127">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="f4421-128">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="f4421-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f4421-129">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="f4421-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="f4421-130">只读。</span><span class="sxs-lookup"><span data-stu-id="f4421-130">Read-only.</span></span>|
|<span data-ttu-id="f4421-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4421-131">createdDateTime</span></span>|<span data-ttu-id="f4421-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4421-132">DateTimeOffset</span></span>|<span data-ttu-id="f4421-133">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="f4421-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f4421-134">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="f4421-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="f4421-135">只读。</span><span class="sxs-lookup"><span data-stu-id="f4421-135">Read-only.</span></span>|
|<span data-ttu-id="f4421-136">id</span><span class="sxs-lookup"><span data-stu-id="f4421-136">id</span></span>|<span data-ttu-id="f4421-137">String</span><span class="sxs-lookup"><span data-stu-id="f4421-137">String</span></span>| <span data-ttu-id="f4421-138">只读。</span><span class="sxs-lookup"><span data-stu-id="f4421-138">Read-only.</span></span>|
|<span data-ttu-id="f4421-139">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="f4421-139">isValidationOnly</span></span>|<span data-ttu-id="f4421-140">布尔</span><span class="sxs-lookup"><span data-stu-id="f4421-140">Boolean</span></span>|<span data-ttu-id="f4421-141">如果请求不处理工作分配，则为 True。</span><span class="sxs-lookup"><span data-stu-id="f4421-141">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="f4421-142">合理化</span><span class="sxs-lookup"><span data-stu-id="f4421-142">justification</span></span>|<span data-ttu-id="f4421-143">String</span><span class="sxs-lookup"><span data-stu-id="f4421-143">String</span></span>|<span data-ttu-id="f4421-144">请求者提供的理由。</span><span class="sxs-lookup"><span data-stu-id="f4421-144">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="f4421-145">requestState</span><span class="sxs-lookup"><span data-stu-id="f4421-145">requestState</span></span>|<span data-ttu-id="f4421-146">String</span><span class="sxs-lookup"><span data-stu-id="f4421-146">String</span></span>|<span data-ttu-id="f4421-147">、 `Denied` `Delivered` `Submitted` 、或`Scheduled`的其中`PartiallyDelivered`一个。</span><span class="sxs-lookup"><span data-stu-id="f4421-147">One of `Denied`, `Delivered`, `PartiallyDelivered`, `Submitted` or `Scheduled`.</span></span> <span data-ttu-id="f4421-148">只读。</span><span class="sxs-lookup"><span data-stu-id="f4421-148">Read-only.</span></span>|
|<span data-ttu-id="f4421-149">requestStatus</span><span class="sxs-lookup"><span data-stu-id="f4421-149">requestStatus</span></span>|<span data-ttu-id="f4421-150">String</span><span class="sxs-lookup"><span data-stu-id="f4421-150">String</span></span>|<span data-ttu-id="f4421-151">有关请求处理状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f4421-151">More information on the request processing status.</span></span> <span data-ttu-id="f4421-152">只读。</span><span class="sxs-lookup"><span data-stu-id="f4421-152">Read-only.</span></span>|
|<span data-ttu-id="f4421-153">requestType</span><span class="sxs-lookup"><span data-stu-id="f4421-153">requestType</span></span>|<span data-ttu-id="f4421-154">String</span><span class="sxs-lookup"><span data-stu-id="f4421-154">String</span></span>|<span data-ttu-id="f4421-155">、 `UserAdd` `UserRemove` `AdminRemove` 、或`SystemRemove`的其中`AdminAdd`一个。</span><span class="sxs-lookup"><span data-stu-id="f4421-155">One of `UserAdd`, `UserRemove`, `AdminAdd`, `AdminRemove` or `SystemRemove`.</span></span> <span data-ttu-id="f4421-156">只读。</span><span class="sxs-lookup"><span data-stu-id="f4421-156">Read-only.</span></span>|
|<span data-ttu-id="f4421-157">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="f4421-157">accessPackageAssignment</span></span>|[<span data-ttu-id="f4421-158">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="f4421-158">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="f4421-159">请求创建的访问包分配。</span><span class="sxs-lookup"><span data-stu-id="f4421-159">An access package assignment requested to be created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4421-160">关系</span><span class="sxs-lookup"><span data-stu-id="f4421-160">Relationships</span></span>

| <span data-ttu-id="f4421-161">关系</span><span class="sxs-lookup"><span data-stu-id="f4421-161">Relationship</span></span> | <span data-ttu-id="f4421-162">类型</span><span class="sxs-lookup"><span data-stu-id="f4421-162">Type</span></span>        | <span data-ttu-id="f4421-163">说明</span><span class="sxs-lookup"><span data-stu-id="f4421-163">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f4421-164">请求程序</span><span class="sxs-lookup"><span data-stu-id="f4421-164">requestor</span></span>|[<span data-ttu-id="f4421-165">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="f4421-165">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="f4421-166">分配了请求的主题或分配了直接分配的主题。</span><span class="sxs-lookup"><span data-stu-id="f4421-166">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="f4421-167">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="f4421-167">Read-only.</span></span> <span data-ttu-id="f4421-168">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f4421-168">Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f4421-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4421-169">JSON representation</span></span>

<span data-ttu-id="f4421-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4421-170">The following is a JSON representation of the resource.</span></span>

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
