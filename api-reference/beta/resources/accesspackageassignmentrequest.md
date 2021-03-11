---
title: accessPackageAssignmentRequest 资源类型
description: 访问包分配请求由想要获取访问包分配的用户创建。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 83218058d375a9f78a24b2af837c39fb5ee77a2c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720436"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="14f76-103">accessPackageAssignmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="14f76-103">accessPackageAssignmentRequest resource type</span></span>

<span data-ttu-id="14f76-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14f76-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14f76-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包分配请求由希望获取访问包分配的用户创建或代表用户创建。</span><span class="sxs-lookup"><span data-stu-id="14f76-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by or on behalf of a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="14f76-106">如果请求成功，并经过任何必要的审批，用户将收到访问包分配，并作为生成的访问包分配的主题。</span><span class="sxs-lookup"><span data-stu-id="14f76-106">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>  <span data-ttu-id="14f76-107">Azure AD 还自动创建访问包分配请求，以跟踪访问删除。</span><span class="sxs-lookup"><span data-stu-id="14f76-107">Azure AD also creates access package assignment requests automatically for tracking access removal.</span></span>

## <a name="methods"></a><span data-ttu-id="14f76-108">方法</span><span class="sxs-lookup"><span data-stu-id="14f76-108">Methods</span></span>

| <span data-ttu-id="14f76-109">方法</span><span class="sxs-lookup"><span data-stu-id="14f76-109">Method</span></span>       | <span data-ttu-id="14f76-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="14f76-110">Return Type</span></span> | <span data-ttu-id="14f76-111">说明</span><span class="sxs-lookup"><span data-stu-id="14f76-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="14f76-112">列出 accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="14f76-112">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="14f76-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14f76-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="14f76-114">检索 accesspackageassignmentrequest 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="14f76-114">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="14f76-115">创建 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="14f76-115">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="14f76-116">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="14f76-116">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="14f76-117">创建新的 accessPackageAssignmentRequest。</span><span class="sxs-lookup"><span data-stu-id="14f76-117">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="14f76-118">获取 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="14f76-118">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="14f76-119">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="14f76-119">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="14f76-120">读取 accessPackageAssignmentRequest 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="14f76-120">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="14f76-121">属性</span><span class="sxs-lookup"><span data-stu-id="14f76-121">Properties</span></span>

| <span data-ttu-id="14f76-122">属性</span><span class="sxs-lookup"><span data-stu-id="14f76-122">Property</span></span>     | <span data-ttu-id="14f76-123">类型</span><span class="sxs-lookup"><span data-stu-id="14f76-123">Type</span></span>        | <span data-ttu-id="14f76-124">说明</span><span class="sxs-lookup"><span data-stu-id="14f76-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="14f76-125">completedDate</span><span class="sxs-lookup"><span data-stu-id="14f76-125">completedDate</span></span>|<span data-ttu-id="14f76-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14f76-126">DateTimeOffset</span></span>|<span data-ttu-id="14f76-127">请求处理结束的日期（成功或失败）。</span><span class="sxs-lookup"><span data-stu-id="14f76-127">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="14f76-128">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="14f76-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="14f76-129">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="14f76-129">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="14f76-130">只读。</span><span class="sxs-lookup"><span data-stu-id="14f76-130">Read-only.</span></span>|
|<span data-ttu-id="14f76-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14f76-131">createdDateTime</span></span>|<span data-ttu-id="14f76-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14f76-132">DateTimeOffset</span></span>|<span data-ttu-id="14f76-133">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="14f76-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="14f76-134">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="14f76-134">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="14f76-135">只读。</span><span class="sxs-lookup"><span data-stu-id="14f76-135">Read-only.</span></span>|
|<span data-ttu-id="14f76-136">id</span><span class="sxs-lookup"><span data-stu-id="14f76-136">id</span></span>|<span data-ttu-id="14f76-137">String</span><span class="sxs-lookup"><span data-stu-id="14f76-137">String</span></span>| <span data-ttu-id="14f76-138">只读。</span><span class="sxs-lookup"><span data-stu-id="14f76-138">Read-only.</span></span>|
|<span data-ttu-id="14f76-139">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="14f76-139">isValidationOnly</span></span>|<span data-ttu-id="14f76-140">布尔</span><span class="sxs-lookup"><span data-stu-id="14f76-140">Boolean</span></span>|<span data-ttu-id="14f76-141">如此 如果不处理工作分配的请求。</span><span class="sxs-lookup"><span data-stu-id="14f76-141">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="14f76-142">justification</span><span class="sxs-lookup"><span data-stu-id="14f76-142">justification</span></span>|<span data-ttu-id="14f76-143">String</span><span class="sxs-lookup"><span data-stu-id="14f76-143">String</span></span>|<span data-ttu-id="14f76-144">请求者提供的理由。</span><span class="sxs-lookup"><span data-stu-id="14f76-144">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="14f76-145">requestState</span><span class="sxs-lookup"><span data-stu-id="14f76-145">requestState</span></span>|<span data-ttu-id="14f76-146">String</span><span class="sxs-lookup"><span data-stu-id="14f76-146">String</span></span>|<span data-ttu-id="14f76-147">`PendingApproval` `Canceled` `Denied` `Delivering` 、、、、或 `Delivered` `PartiallyDelivered` `Submitted` `Scheduled` 。</span><span class="sxs-lookup"><span data-stu-id="14f76-147">One of `PendingApproval`, `Canceled`,  `Denied`, `Delivering`, `Delivered`, `PartiallyDelivered`, `Submitted` or `Scheduled`.</span></span> <span data-ttu-id="14f76-148">只读。</span><span class="sxs-lookup"><span data-stu-id="14f76-148">Read-only.</span></span>|
|<span data-ttu-id="14f76-149">requestStatus</span><span class="sxs-lookup"><span data-stu-id="14f76-149">requestStatus</span></span>|<span data-ttu-id="14f76-150">String</span><span class="sxs-lookup"><span data-stu-id="14f76-150">String</span></span>|<span data-ttu-id="14f76-151">有关请求处理状态的信息。</span><span class="sxs-lookup"><span data-stu-id="14f76-151">More information on the request processing status.</span></span> <span data-ttu-id="14f76-152">只读。</span><span class="sxs-lookup"><span data-stu-id="14f76-152">Read-only.</span></span>|
|<span data-ttu-id="14f76-153">requestType</span><span class="sxs-lookup"><span data-stu-id="14f76-153">requestType</span></span>|<span data-ttu-id="14f76-154">String</span><span class="sxs-lookup"><span data-stu-id="14f76-154">String</span></span>|<span data-ttu-id="14f76-155">之一 `UserAdd` `UserRemove` ， ， 或 `AdminAdd` `AdminRemove` `SystemRemove` 。</span><span class="sxs-lookup"><span data-stu-id="14f76-155">One of `UserAdd`, `UserRemove`, `AdminAdd`, `AdminRemove` or `SystemRemove`.</span></span> <span data-ttu-id="14f76-156">来自用户本身的请求将具有 or 的 `UserAdd` `UserRemove` requestType。</span><span class="sxs-lookup"><span data-stu-id="14f76-156">A request from the user themselves would have requestType of `UserAdd` or `UserRemove`.</span></span> <span data-ttu-id="14f76-157">只读。</span><span class="sxs-lookup"><span data-stu-id="14f76-157">Read-only.</span></span>|
|<span data-ttu-id="14f76-158">schedule</span><span class="sxs-lookup"><span data-stu-id="14f76-158">schedule</span></span>|[<span data-ttu-id="14f76-159">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="14f76-159">requestSchedule</span></span>](requestschedule.md)| <span data-ttu-id="14f76-160">要分配给请求者的访问日期范围。</span><span class="sxs-lookup"><span data-stu-id="14f76-160">The range of dates that access is to be assigned to the requestor.</span></span> <span data-ttu-id="14f76-161">只读。</span><span class="sxs-lookup"><span data-stu-id="14f76-161">Read-only.</span></span>|
|<span data-ttu-id="14f76-162">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="14f76-162">accessPackageAssignment</span></span>|[<span data-ttu-id="14f76-163">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="14f76-163">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="14f76-164">对于 or 的 `UserAdd` `AdminAdd` requestType，这是请求创建的访问包分配。</span><span class="sxs-lookup"><span data-stu-id="14f76-164">For a requestType of `UserAdd` or `AdminAdd`, this is an access package assignment requested to be created.</span></span>  <span data-ttu-id="14f76-165">对于 or 的 requestType，此属性具有要删除的现有 `UserRemove` `AdminRemove` `SystemRemove` `id` 工作分配的属性。</span><span class="sxs-lookup"><span data-stu-id="14f76-165">For a requestType of `UserRemove`, `AdminRemove` or `SystemRemove`, this has the `id` property of an existing assignment to be removed.</span></span>|
|<span data-ttu-id="14f76-166">答案</span><span class="sxs-lookup"><span data-stu-id="14f76-166">answers</span></span>|<span data-ttu-id="14f76-167">[accessPackageAnswer](accesspackageanswer.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14f76-167">[accessPackageAnswer](accesspackageanswer.md) collection</span></span>|<span data-ttu-id="14f76-168">请求者提供的访问 [PackageQuestions](accesspackagequestion.md) 的解答在请求时询问他们。</span><span class="sxs-lookup"><span data-stu-id="14f76-168">Answers provided by the requestor to [accessPackageQuestions](accesspackagequestion.md) asked of them at the time of request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14f76-169">关系</span><span class="sxs-lookup"><span data-stu-id="14f76-169">Relationships</span></span>

| <span data-ttu-id="14f76-170">关系</span><span class="sxs-lookup"><span data-stu-id="14f76-170">Relationship</span></span> | <span data-ttu-id="14f76-171">类型</span><span class="sxs-lookup"><span data-stu-id="14f76-171">Type</span></span>        | <span data-ttu-id="14f76-172">说明</span><span class="sxs-lookup"><span data-stu-id="14f76-172">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="14f76-173">requestor</span><span class="sxs-lookup"><span data-stu-id="14f76-173">requestor</span></span>|[<span data-ttu-id="14f76-174">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="14f76-174">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="14f76-175">请求或分配了直接分配的主题（如果为直接分配）。</span><span class="sxs-lookup"><span data-stu-id="14f76-175">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="14f76-176">只读。</span><span class="sxs-lookup"><span data-stu-id="14f76-176">Read-only.</span></span> <span data-ttu-id="14f76-177">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="14f76-177">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14f76-178">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14f76-178">JSON representation</span></span>

<span data-ttu-id="14f76-179">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14f76-179">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
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

