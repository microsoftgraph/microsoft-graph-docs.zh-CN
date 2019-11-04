---
title: accessPackageAssignmentRequest 资源类型
description: 访问包分配请求由要获取访问包分配的用户创建。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a6be3fa431a2216ef8b31b673a5f73ef6067fff9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939199"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="1b3a8-103">accessPackageAssignmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b3a8-103">accessPackageAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b3a8-104">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配请求由要获取访问包分配的用户创建。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="1b3a8-105">如果请求成功，并且具有必要的审批，则用户将收到访问包分配，并且是最终的访问包分配的主题。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-105">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>


## <a name="methods"></a><span data-ttu-id="1b3a8-106">方法</span><span class="sxs-lookup"><span data-stu-id="1b3a8-106">Methods</span></span>

| <span data-ttu-id="1b3a8-107">方法</span><span class="sxs-lookup"><span data-stu-id="1b3a8-107">Method</span></span>       | <span data-ttu-id="1b3a8-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="1b3a8-108">Return Type</span></span> | <span data-ttu-id="1b3a8-109">说明</span><span class="sxs-lookup"><span data-stu-id="1b3a8-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1b3a8-110">列出 accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="1b3a8-110">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="1b3a8-111">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="1b3a8-111">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="1b3a8-112">检索 accesspackageassignmentrequest 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-112">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="1b3a8-113">创建 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="1b3a8-113">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="1b3a8-114">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="1b3a8-114">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="1b3a8-115">创建新的 accessPackageAssignmentRequest。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-115">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="1b3a8-116">获取 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="1b3a8-116">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="1b3a8-117">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="1b3a8-117">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="1b3a8-118">读取 accessPackageAssignmentRequest 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-118">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1b3a8-119">属性</span><span class="sxs-lookup"><span data-stu-id="1b3a8-119">Properties</span></span>

| <span data-ttu-id="1b3a8-120">属性</span><span class="sxs-lookup"><span data-stu-id="1b3a8-120">Property</span></span>     | <span data-ttu-id="1b3a8-121">类型</span><span class="sxs-lookup"><span data-stu-id="1b3a8-121">Type</span></span>        | <span data-ttu-id="1b3a8-122">描述</span><span class="sxs-lookup"><span data-stu-id="1b3a8-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1b3a8-123">completedDate</span><span class="sxs-lookup"><span data-stu-id="1b3a8-123">completedDate</span></span>|<span data-ttu-id="1b3a8-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b3a8-124">DateTimeOffset</span></span>|<span data-ttu-id="1b3a8-125">请求的处理结束日期（成功或失败）。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-125">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="1b3a8-126">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1b3a8-127">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="1b3a8-128">只读。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-128">Read-only.</span></span>|
|<span data-ttu-id="1b3a8-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b3a8-129">createdDateTime</span></span>|<span data-ttu-id="1b3a8-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b3a8-130">DateTimeOffset</span></span>|<span data-ttu-id="1b3a8-131">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1b3a8-132">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="1b3a8-133">只读。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-133">Read-only.</span></span>|
|<span data-ttu-id="1b3a8-134">id</span><span class="sxs-lookup"><span data-stu-id="1b3a8-134">id</span></span>|<span data-ttu-id="1b3a8-135">字符串</span><span class="sxs-lookup"><span data-stu-id="1b3a8-135">String</span></span>| <span data-ttu-id="1b3a8-136">只读。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-136">Read-only.</span></span>|
|<span data-ttu-id="1b3a8-137">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="1b3a8-137">isValidationOnly</span></span>|<span data-ttu-id="1b3a8-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b3a8-138">Boolean</span></span>|<span data-ttu-id="1b3a8-139">如果请求不处理工作分配，则为 True。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-139">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="1b3a8-140">合理化</span><span class="sxs-lookup"><span data-stu-id="1b3a8-140">justification</span></span>|<span data-ttu-id="1b3a8-141">字符串</span><span class="sxs-lookup"><span data-stu-id="1b3a8-141">String</span></span>|<span data-ttu-id="1b3a8-142">请求者提供的理由。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-142">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="1b3a8-143">requestState</span><span class="sxs-lookup"><span data-stu-id="1b3a8-143">requestState</span></span>|<span data-ttu-id="1b3a8-144">字符串</span><span class="sxs-lookup"><span data-stu-id="1b3a8-144">String</span></span>|<span data-ttu-id="1b3a8-145">、 `Denied` `Delivered`、中`PartiallyDelivered`的一个。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-145">One of `Denied`, `Delivered`, `PartiallyDelivered`.</span></span> <span data-ttu-id="1b3a8-146">只读。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-146">Read-only.</span></span>|
|<span data-ttu-id="1b3a8-147">requestStatus</span><span class="sxs-lookup"><span data-stu-id="1b3a8-147">requestStatus</span></span>|<span data-ttu-id="1b3a8-148">字符串</span><span class="sxs-lookup"><span data-stu-id="1b3a8-148">String</span></span>|<span data-ttu-id="1b3a8-149">有关请求处理状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-149">More information on the request processing status.</span></span> <span data-ttu-id="1b3a8-150">只读。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-150">Read-only.</span></span>|
|<span data-ttu-id="1b3a8-151">requestType</span><span class="sxs-lookup"><span data-stu-id="1b3a8-151">requestType</span></span>|<span data-ttu-id="1b3a8-152">字符串</span><span class="sxs-lookup"><span data-stu-id="1b3a8-152">String</span></span>|<span data-ttu-id="1b3a8-153">一个`UserAdd`或`UserRemove`。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-153">One of `UserAdd` or `UserRemove`.</span></span> <span data-ttu-id="1b3a8-154">只读。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-154">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="1b3a8-155">关系</span><span class="sxs-lookup"><span data-stu-id="1b3a8-155">Relationships</span></span>

| <span data-ttu-id="1b3a8-156">关系</span><span class="sxs-lookup"><span data-stu-id="1b3a8-156">Relationship</span></span> | <span data-ttu-id="1b3a8-157">类型</span><span class="sxs-lookup"><span data-stu-id="1b3a8-157">Type</span></span>        | <span data-ttu-id="1b3a8-158">描述</span><span class="sxs-lookup"><span data-stu-id="1b3a8-158">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1b3a8-159">请求程序</span><span class="sxs-lookup"><span data-stu-id="1b3a8-159">requestor</span></span>|[<span data-ttu-id="1b3a8-160">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="1b3a8-160">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="1b3a8-161">分配了请求的主题或分配了直接分配的主题。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-161">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="1b3a8-162">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-162">Read-only.</span></span> <span data-ttu-id="1b3a8-163">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-163">Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1b3a8-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b3a8-164">JSON representation</span></span>

<span data-ttu-id="1b3a8-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b3a8-165">The following is a JSON representation of the resource.</span></span>

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
