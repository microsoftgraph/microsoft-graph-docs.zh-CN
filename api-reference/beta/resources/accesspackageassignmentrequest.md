---
title: accessPackageAssignmentRequest 资源类型
description: 访问包分配请求由想要获取访问包分配的用户创建。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9ecaa9b77a92dc6393b3c7231976937e36502c8d
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719753"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="e0552-103">accessPackageAssignmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0552-103">accessPackageAssignmentRequest resource type</span></span>

<span data-ttu-id="e0552-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0552-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0552-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包分配请求由想要获取访问包分配的用户创建或代表用户创建。</span><span class="sxs-lookup"><span data-stu-id="e0552-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by or on behalf of a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="e0552-106">如果请求成功，经过任何必要的审批，用户将收到访问包分配，并作为生成的访问包分配的主题。</span><span class="sxs-lookup"><span data-stu-id="e0552-106">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>  <span data-ttu-id="e0552-107">Azure AD 还自动创建访问包分配请求，以跟踪访问权限删除。</span><span class="sxs-lookup"><span data-stu-id="e0552-107">Azure AD also creates access package assignment requests automatically for tracking access removal.</span></span>

## <a name="methods"></a><span data-ttu-id="e0552-108">方法</span><span class="sxs-lookup"><span data-stu-id="e0552-108">Methods</span></span>

| <span data-ttu-id="e0552-109">方法</span><span class="sxs-lookup"><span data-stu-id="e0552-109">Method</span></span>       | <span data-ttu-id="e0552-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e0552-110">Return Type</span></span> | <span data-ttu-id="e0552-111">说明</span><span class="sxs-lookup"><span data-stu-id="e0552-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e0552-112">列出 accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="e0552-112">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="e0552-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0552-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="e0552-114">检索 accesspackageassignmentrequest 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="e0552-114">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="e0552-115">创建 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="e0552-115">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="e0552-116">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="e0552-116">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="e0552-117">创建新的 accessPackageAssignmentRequest。</span><span class="sxs-lookup"><span data-stu-id="e0552-117">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="e0552-118">获取 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="e0552-118">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="e0552-119">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="e0552-119">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="e0552-120">读取 accessPackageAssignmentRequest 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e0552-120">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e0552-121">属性</span><span class="sxs-lookup"><span data-stu-id="e0552-121">Properties</span></span>

| <span data-ttu-id="e0552-122">属性</span><span class="sxs-lookup"><span data-stu-id="e0552-122">Property</span></span>     | <span data-ttu-id="e0552-123">类型</span><span class="sxs-lookup"><span data-stu-id="e0552-123">Type</span></span>        | <span data-ttu-id="e0552-124">说明</span><span class="sxs-lookup"><span data-stu-id="e0552-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e0552-125">completedDate</span><span class="sxs-lookup"><span data-stu-id="e0552-125">completedDate</span></span>|<span data-ttu-id="e0552-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0552-126">DateTimeOffset</span></span>|<span data-ttu-id="e0552-127">请求处理结束的日期（成功或失败）。</span><span class="sxs-lookup"><span data-stu-id="e0552-127">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="e0552-128">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="e0552-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e0552-129">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="e0552-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="e0552-130">只读。</span><span class="sxs-lookup"><span data-stu-id="e0552-130">Read-only.</span></span>|
|<span data-ttu-id="e0552-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0552-131">createdDateTime</span></span>|<span data-ttu-id="e0552-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0552-132">DateTimeOffset</span></span>|<span data-ttu-id="e0552-133">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="e0552-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e0552-134">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="e0552-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="e0552-135">只读。</span><span class="sxs-lookup"><span data-stu-id="e0552-135">Read-only.</span></span>|
|<span data-ttu-id="e0552-136">id</span><span class="sxs-lookup"><span data-stu-id="e0552-136">id</span></span>|<span data-ttu-id="e0552-137">String</span><span class="sxs-lookup"><span data-stu-id="e0552-137">String</span></span>| <span data-ttu-id="e0552-138">只读。</span><span class="sxs-lookup"><span data-stu-id="e0552-138">Read-only.</span></span>|
|<span data-ttu-id="e0552-139">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="e0552-139">isValidationOnly</span></span>|<span data-ttu-id="e0552-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0552-140">Boolean</span></span>|<span data-ttu-id="e0552-141">如此 如果不处理工作分配的请求。</span><span class="sxs-lookup"><span data-stu-id="e0552-141">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="e0552-142">justification</span><span class="sxs-lookup"><span data-stu-id="e0552-142">justification</span></span>|<span data-ttu-id="e0552-143">String</span><span class="sxs-lookup"><span data-stu-id="e0552-143">String</span></span>|<span data-ttu-id="e0552-144">请求者提供的理由。</span><span class="sxs-lookup"><span data-stu-id="e0552-144">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="e0552-145">requestState</span><span class="sxs-lookup"><span data-stu-id="e0552-145">requestState</span></span>|<span data-ttu-id="e0552-146">String</span><span class="sxs-lookup"><span data-stu-id="e0552-146">String</span></span>|<span data-ttu-id="e0552-147">、 `PendingApproval` `Canceled`  `Denied` `Delivering` 或 `Delivered` `PartiallyDelivered` `Submitted` `Scheduled` 。</span><span class="sxs-lookup"><span data-stu-id="e0552-147">One of `PendingApproval`, `Canceled`,  `Denied`, `Delivering`, `Delivered`, `PartiallyDelivered`, `Submitted` or `Scheduled`.</span></span> <span data-ttu-id="e0552-148">只读。</span><span class="sxs-lookup"><span data-stu-id="e0552-148">Read-only.</span></span>|
|<span data-ttu-id="e0552-149">requestStatus</span><span class="sxs-lookup"><span data-stu-id="e0552-149">requestStatus</span></span>|<span data-ttu-id="e0552-150">String</span><span class="sxs-lookup"><span data-stu-id="e0552-150">String</span></span>|<span data-ttu-id="e0552-151">有关请求处理状态的信息。</span><span class="sxs-lookup"><span data-stu-id="e0552-151">More information on the request processing status.</span></span> <span data-ttu-id="e0552-152">只读。</span><span class="sxs-lookup"><span data-stu-id="e0552-152">Read-only.</span></span>|
|<span data-ttu-id="e0552-153">requestType</span><span class="sxs-lookup"><span data-stu-id="e0552-153">requestType</span></span>|<span data-ttu-id="e0552-154">String</span><span class="sxs-lookup"><span data-stu-id="e0552-154">String</span></span>|<span data-ttu-id="e0552-155">之一 `UserAdd` `UserRemove` ， ， 或 `AdminAdd` `AdminRemove` `SystemRemove` 。</span><span class="sxs-lookup"><span data-stu-id="e0552-155">One of `UserAdd`, `UserRemove`, `AdminAdd`, `AdminRemove` or `SystemRemove`.</span></span> <span data-ttu-id="e0552-156">来自用户本身的请求将具有的 requestType `UserAdd` 或 `UserRemove` 。</span><span class="sxs-lookup"><span data-stu-id="e0552-156">A request from the user themselves would have requestType of `UserAdd` or `UserRemove`.</span></span> <span data-ttu-id="e0552-157">只读。</span><span class="sxs-lookup"><span data-stu-id="e0552-157">Read-only.</span></span>|
|<span data-ttu-id="e0552-158">schedule</span><span class="sxs-lookup"><span data-stu-id="e0552-158">schedule</span></span>|[<span data-ttu-id="e0552-159">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="e0552-159">requestSchedule</span></span>](requestschedule.md)| <span data-ttu-id="e0552-160">要分配给请求者的日期范围。</span><span class="sxs-lookup"><span data-stu-id="e0552-160">The range of dates that access is to be assigned to the requestor.</span></span> <span data-ttu-id="e0552-161">只读。</span><span class="sxs-lookup"><span data-stu-id="e0552-161">Read-only.</span></span>|
|<span data-ttu-id="e0552-162">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="e0552-162">accessPackageAssignment</span></span>|[<span data-ttu-id="e0552-163">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="e0552-163">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="e0552-164">对于 or 的 `UserAdd` `AdminAdd` requestType，这是请求创建的访问包分配。</span><span class="sxs-lookup"><span data-stu-id="e0552-164">For a requestType of `UserAdd` or `AdminAdd`, this is an access package assignment requested to be created.</span></span>  <span data-ttu-id="e0552-165">对于或 的 `UserRemove` `AdminRemove` `SystemRemove` requestType，此属性具有要删除 `id` 的现有工作分配的属性。</span><span class="sxs-lookup"><span data-stu-id="e0552-165">For a requestType of `UserRemove`, `AdminRemove` or `SystemRemove`, this has the `id` property of an existing assignment to be removed.</span></span>|
|<span data-ttu-id="e0552-166">answers</span><span class="sxs-lookup"><span data-stu-id="e0552-166">answers</span></span>|<span data-ttu-id="e0552-167">[accessPackageAnswer](accesspackageanswer.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0552-167">[accessPackageAnswer](accesspackageanswer.md) collection</span></span>|<span data-ttu-id="e0552-168">请求者提供的对 [accessPackageQuestions](accesspackagequestion.md) 的回答在请求时询问他们。</span><span class="sxs-lookup"><span data-stu-id="e0552-168">Answers provided by the requestor to [accessPackageQuestions](accesspackagequestion.md) asked of them at the time of request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0552-169">关系</span><span class="sxs-lookup"><span data-stu-id="e0552-169">Relationships</span></span>

| <span data-ttu-id="e0552-170">关系</span><span class="sxs-lookup"><span data-stu-id="e0552-170">Relationship</span></span> | <span data-ttu-id="e0552-171">类型</span><span class="sxs-lookup"><span data-stu-id="e0552-171">Type</span></span>        | <span data-ttu-id="e0552-172">说明</span><span class="sxs-lookup"><span data-stu-id="e0552-172">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e0552-173">requestor</span><span class="sxs-lookup"><span data-stu-id="e0552-173">requestor</span></span>|[<span data-ttu-id="e0552-174">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="e0552-174">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="e0552-175">请求或分配了直接分配（如果直接分配）的主题。</span><span class="sxs-lookup"><span data-stu-id="e0552-175">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="e0552-176">只读。</span><span class="sxs-lookup"><span data-stu-id="e0552-176">Read-only.</span></span> <span data-ttu-id="e0552-177">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e0552-177">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e0552-178">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0552-178">JSON representation</span></span>

<span data-ttu-id="e0552-179">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0552-179">The following is a JSON representation of the resource.</span></span>

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
    "createdDateTime": "string",
    "completedDate": "string",
    "id": "string",
    "requestType": "string",
    "requestState": "string",
    "requestStatus": "string",
    "isValidationOnly": false,
    "justification": "string",
    "answers": [{
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "string",
        "answeredQuestion": {
            "id": "string",
            "text": {
                "defaultText": "string",
                "localizedTexts": [{
                    "text": "string",
                    "languageCode": "string"
                }]
            },
            "isRequired": true,
            "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
            "isSingleLineQuestion": true
        }
    }]
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

