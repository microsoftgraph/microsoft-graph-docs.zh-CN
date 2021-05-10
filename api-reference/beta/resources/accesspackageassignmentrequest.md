---
title: accessPackageAssignmentRequest 资源类型
description: 访问包分配请求由想要获取访问包分配的用户创建。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7825b19e80274c8bcd54a5d8d03aa1dd40cf49c9
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298496"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="01a63-103">accessPackageAssignmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="01a63-103">accessPackageAssignmentRequest resource type</span></span>

<span data-ttu-id="01a63-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01a63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01a63-105">在 [Azure AD 授权管理](entitlementmanagement-root.md)中，访问包分配请求由希望获取访问包分配的用户创建或代表用户创建。</span><span class="sxs-lookup"><span data-stu-id="01a63-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), an access package assignment request is created by or on behalf of a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="01a63-106">如果请求成功，并且经过任何必要的审批，用户将收到访问包分配，并且是生成的访问包分配的主题。</span><span class="sxs-lookup"><span data-stu-id="01a63-106">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>  <span data-ttu-id="01a63-107">Azure AD 还自动创建访问包分配请求，以跟踪访问删除。</span><span class="sxs-lookup"><span data-stu-id="01a63-107">Azure AD also creates access package assignment requests automatically for tracking access removal.</span></span>

## <a name="methods"></a><span data-ttu-id="01a63-108">方法</span><span class="sxs-lookup"><span data-stu-id="01a63-108">Methods</span></span>

| <span data-ttu-id="01a63-109">方法</span><span class="sxs-lookup"><span data-stu-id="01a63-109">Method</span></span>       | <span data-ttu-id="01a63-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="01a63-110">Return Type</span></span> | <span data-ttu-id="01a63-111">说明</span><span class="sxs-lookup"><span data-stu-id="01a63-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="01a63-112">列出 accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="01a63-112">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="01a63-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="01a63-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="01a63-114">检索 **accesspackageassignmentrequest 对象** 的列表。</span><span class="sxs-lookup"><span data-stu-id="01a63-114">Retrieve a list of **accesspackageassignmentrequest** objects.</span></span> |
| [<span data-ttu-id="01a63-115">创建 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="01a63-115">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="01a63-116">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="01a63-116">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="01a63-117">创建新的 **accessPackageAssignmentRequest**。</span><span class="sxs-lookup"><span data-stu-id="01a63-117">Create a new **accessPackageAssignmentRequest**.</span></span> |
| [<span data-ttu-id="01a63-118">获取 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="01a63-118">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="01a63-119">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="01a63-119">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="01a63-120">读取 **accessPackageAssignmentRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="01a63-120">Read properties and relationships of an **accessPackageAssignmentRequest** object.</span></span> |
|[<span data-ttu-id="01a63-121">filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="01a63-121">filterByCurrentUser</span></span>](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|<span data-ttu-id="01a63-122">[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="01a63-122">[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection</span></span>|<span data-ttu-id="01a63-123">检索已登录 **用户筛选的 accessPackageAssignmentRequest** 对象列表。</span><span class="sxs-lookup"><span data-stu-id="01a63-123">Retrieve the list of **accessPackageAssignmentRequest** objects filtered on the signed-in user.</span></span>|
|[<span data-ttu-id="01a63-124">取消</span><span class="sxs-lookup"><span data-stu-id="01a63-124">cancel</span></span>](../api/accesspackageassignmentrequest-cancel.md)|<span data-ttu-id="01a63-125">[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="01a63-125">[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection</span></span>|<span data-ttu-id="01a63-126">取消 **处于可取消状态中的 accessPackageAssignmentRequest** 对象。</span><span class="sxs-lookup"><span data-stu-id="01a63-126">Cancel an **accessPackageAssignmentRequest** object that is in a cancellable state.</span></span>|

## <a name="properties"></a><span data-ttu-id="01a63-127">属性</span><span class="sxs-lookup"><span data-stu-id="01a63-127">Properties</span></span>

| <span data-ttu-id="01a63-128">属性</span><span class="sxs-lookup"><span data-stu-id="01a63-128">Property</span></span>     | <span data-ttu-id="01a63-129">类型</span><span class="sxs-lookup"><span data-stu-id="01a63-129">Type</span></span>        | <span data-ttu-id="01a63-130">说明</span><span class="sxs-lookup"><span data-stu-id="01a63-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="01a63-131">completedDate</span><span class="sxs-lookup"><span data-stu-id="01a63-131">completedDate</span></span>|<span data-ttu-id="01a63-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01a63-132">DateTimeOffset</span></span>|<span data-ttu-id="01a63-133">请求处理终止的日期（成功或失败）。</span><span class="sxs-lookup"><span data-stu-id="01a63-133">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="01a63-134">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="01a63-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="01a63-135">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="01a63-135">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="01a63-136">只读。</span><span class="sxs-lookup"><span data-stu-id="01a63-136">Read-only.</span></span>|
|<span data-ttu-id="01a63-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="01a63-137">createdDateTime</span></span>|<span data-ttu-id="01a63-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01a63-138">DateTimeOffset</span></span>|<span data-ttu-id="01a63-139">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="01a63-139">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="01a63-140">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="01a63-140">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="01a63-141">只读。</span><span class="sxs-lookup"><span data-stu-id="01a63-141">Read-only.</span></span>|
|<span data-ttu-id="01a63-142">id</span><span class="sxs-lookup"><span data-stu-id="01a63-142">id</span></span>|<span data-ttu-id="01a63-143">String</span><span class="sxs-lookup"><span data-stu-id="01a63-143">String</span></span>| <span data-ttu-id="01a63-144">只读。</span><span class="sxs-lookup"><span data-stu-id="01a63-144">Read-only.</span></span>|
|<span data-ttu-id="01a63-145">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="01a63-145">isValidationOnly</span></span>|<span data-ttu-id="01a63-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="01a63-146">Boolean</span></span>|<span data-ttu-id="01a63-147">如此 如果不处理工作分配的请求。</span><span class="sxs-lookup"><span data-stu-id="01a63-147">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="01a63-148">justification</span><span class="sxs-lookup"><span data-stu-id="01a63-148">justification</span></span>|<span data-ttu-id="01a63-149">String</span><span class="sxs-lookup"><span data-stu-id="01a63-149">String</span></span>|<span data-ttu-id="01a63-150">请求者提供的理由。</span><span class="sxs-lookup"><span data-stu-id="01a63-150">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="01a63-151">requestState</span><span class="sxs-lookup"><span data-stu-id="01a63-151">requestState</span></span>|<span data-ttu-id="01a63-152">String</span><span class="sxs-lookup"><span data-stu-id="01a63-152">String</span></span>|<span data-ttu-id="01a63-153">、 `PendingApproval` `Canceled` 、  `Denied` 、 、 、 `Delivering` 或 `Delivered` `PartiallyDelivered` `Submitted` `Scheduled` 之一。</span><span class="sxs-lookup"><span data-stu-id="01a63-153">One of `PendingApproval`, `Canceled`,  `Denied`, `Delivering`, `Delivered`, `PartiallyDelivered`, `Submitted` or `Scheduled`.</span></span> <span data-ttu-id="01a63-154">只读。</span><span class="sxs-lookup"><span data-stu-id="01a63-154">Read-only.</span></span>|
|<span data-ttu-id="01a63-155">requestStatus</span><span class="sxs-lookup"><span data-stu-id="01a63-155">requestStatus</span></span>|<span data-ttu-id="01a63-156">String</span><span class="sxs-lookup"><span data-stu-id="01a63-156">String</span></span>|<span data-ttu-id="01a63-157">有关请求处理状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="01a63-157">More information on the request processing status.</span></span> <span data-ttu-id="01a63-158">只读。</span><span class="sxs-lookup"><span data-stu-id="01a63-158">Read-only.</span></span>|
|<span data-ttu-id="01a63-159">requestType</span><span class="sxs-lookup"><span data-stu-id="01a63-159">requestType</span></span>|<span data-ttu-id="01a63-160">String</span><span class="sxs-lookup"><span data-stu-id="01a63-160">String</span></span>|<span data-ttu-id="01a63-161">、 `UserAdd` `UserRemove` 、 `AdminAdd` 或 `AdminRemove` `SystemRemove` 之一。</span><span class="sxs-lookup"><span data-stu-id="01a63-161">One of `UserAdd`, `UserRemove`, `AdminAdd`, `AdminRemove` or `SystemRemove`.</span></span> <span data-ttu-id="01a63-162">来自用户本身的请求的 requestType 为 `UserAdd` 或 `UserRemove` 。</span><span class="sxs-lookup"><span data-stu-id="01a63-162">A request from the user themselves would have requestType of `UserAdd` or `UserRemove`.</span></span> <span data-ttu-id="01a63-163">只读。</span><span class="sxs-lookup"><span data-stu-id="01a63-163">Read-only.</span></span>|
|<span data-ttu-id="01a63-164">schedule</span><span class="sxs-lookup"><span data-stu-id="01a63-164">schedule</span></span>|[<span data-ttu-id="01a63-165">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="01a63-165">requestSchedule</span></span>](requestschedule.md)| <span data-ttu-id="01a63-166">要分配给请求者的日期范围。</span><span class="sxs-lookup"><span data-stu-id="01a63-166">The range of dates that access is to be assigned to the requestor.</span></span> <span data-ttu-id="01a63-167">只读。</span><span class="sxs-lookup"><span data-stu-id="01a63-167">Read-only.</span></span>|
|<span data-ttu-id="01a63-168">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="01a63-168">accessPackageAssignment</span></span>|[<span data-ttu-id="01a63-169">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="01a63-169">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="01a63-170">对于 或 `UserAdd` 的 `AdminAdd` requestType，这是请求创建的访问包分配。</span><span class="sxs-lookup"><span data-stu-id="01a63-170">For a requestType of `UserAdd` or `AdminAdd`, this is an access package assignment requested to be created.</span></span>  <span data-ttu-id="01a63-171">对于 、 `UserRemove` 或 的 requestType，此属性具有要删除的现有 `AdminRemove` `SystemRemove` `id` 工作分配的 属性。</span><span class="sxs-lookup"><span data-stu-id="01a63-171">For a requestType of `UserRemove`, `AdminRemove` or `SystemRemove`, this has the `id` property of an existing assignment to be removed.</span></span>|
|<span data-ttu-id="01a63-172">answers</span><span class="sxs-lookup"><span data-stu-id="01a63-172">answers</span></span>|<span data-ttu-id="01a63-173">[accessPackageAnswer](accesspackageanswer.md) 集合</span><span class="sxs-lookup"><span data-stu-id="01a63-173">[accessPackageAnswer](accesspackageanswer.md) collection</span></span>|<span data-ttu-id="01a63-174">请求者提供的 [accessPackageQuestions](accesspackagequestion.md) 在请求时询问他们的答案。</span><span class="sxs-lookup"><span data-stu-id="01a63-174">Answers provided by the requestor to [accessPackageQuestions](accesspackagequestion.md) asked of them at the time of request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01a63-175">关系</span><span class="sxs-lookup"><span data-stu-id="01a63-175">Relationships</span></span>

| <span data-ttu-id="01a63-176">关系</span><span class="sxs-lookup"><span data-stu-id="01a63-176">Relationship</span></span> | <span data-ttu-id="01a63-177">类型</span><span class="sxs-lookup"><span data-stu-id="01a63-177">Type</span></span>        | <span data-ttu-id="01a63-178">说明</span><span class="sxs-lookup"><span data-stu-id="01a63-178">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="01a63-179">accessPackage</span><span class="sxs-lookup"><span data-stu-id="01a63-179">accessPackage</span></span>|[<span data-ttu-id="01a63-180">accessPackage</span><span class="sxs-lookup"><span data-stu-id="01a63-180">accessPackage</span></span>](../resources/accesspackage.md)|<span data-ttu-id="01a63-181">与 accessPackageAssignmentRequest 关联的访问包。</span><span class="sxs-lookup"><span data-stu-id="01a63-181">The access package associated with the accessPackageAssignmentRequest.</span></span> <span data-ttu-id="01a63-182">访问包定义资源角色的集合，以及一个或多个用户如何访问这些资源的策略。</span><span class="sxs-lookup"><span data-stu-id="01a63-182">An access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span> <span data-ttu-id="01a63-183">只读。</span><span class="sxs-lookup"><span data-stu-id="01a63-183">Read-only.</span></span> <span data-ttu-id="01a63-184">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="01a63-184">Nullable.</span></span>|
|<span data-ttu-id="01a63-185">requestor</span><span class="sxs-lookup"><span data-stu-id="01a63-185">requestor</span></span>|[<span data-ttu-id="01a63-186">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="01a63-186">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="01a63-187">请求或分配直接分配（如果直接分配）的主题。</span><span class="sxs-lookup"><span data-stu-id="01a63-187">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="01a63-188">只读。</span><span class="sxs-lookup"><span data-stu-id="01a63-188">Read-only.</span></span> <span data-ttu-id="01a63-189">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="01a63-189">Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="01a63-190">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="01a63-190">JSON representation</span></span>

<span data-ttu-id="01a63-191">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01a63-191">The following is a JSON representation of the resource.</span></span>

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

