---
title: 更新 plannerTask
description: 更新 **plannertask** 对象的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 515bb5b7b8403aab01e12eaa40b0ade5d2a68268
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455611"
---
# <a name="update-plannertask"></a><span data-ttu-id="97e34-103">更新 plannerTask</span><span class="sxs-lookup"><span data-stu-id="97e34-103">Update plannertask</span></span>

<span data-ttu-id="97e34-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="97e34-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97e34-105">更新 **plannertask** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="97e34-105">Update the properties of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="97e34-106">权限</span><span class="sxs-lookup"><span data-stu-id="97e34-106">Permissions</span></span>
<span data-ttu-id="97e34-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97e34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97e34-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="97e34-109">Permission type</span></span>      | <span data-ttu-id="97e34-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="97e34-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97e34-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97e34-111">Delegated (work or school account)</span></span> | <span data-ttu-id="97e34-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97e34-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="97e34-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97e34-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97e34-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="97e34-114">Not supported.</span></span>    |
|<span data-ttu-id="97e34-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="97e34-115">Application</span></span> | <span data-ttu-id="97e34-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="97e34-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="97e34-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97e34-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="97e34-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="97e34-118">Optional request headers</span></span>
| <span data-ttu-id="97e34-119">名称</span><span class="sxs-lookup"><span data-stu-id="97e34-119">Name</span></span>       | <span data-ttu-id="97e34-120">说明</span><span class="sxs-lookup"><span data-stu-id="97e34-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="97e34-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="97e34-121">Authorization</span></span>  | <span data-ttu-id="97e34-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="97e34-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="97e34-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="97e34-124">If-Match</span></span>  | <span data-ttu-id="97e34-p103">要更新的 **plannerTask** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="97e34-p103">Last known ETag value for the **plannerTask** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="97e34-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="97e34-127">Request body</span></span>
<span data-ttu-id="97e34-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="97e34-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="97e34-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="97e34-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="97e34-130">为了获得最佳性能，请不要包含尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="97e34-130">For best performance,  don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="97e34-131">属性</span><span class="sxs-lookup"><span data-stu-id="97e34-131">Property</span></span>     | <span data-ttu-id="97e34-132">类型</span><span class="sxs-lookup"><span data-stu-id="97e34-132">Type</span></span>   |<span data-ttu-id="97e34-133">说明</span><span class="sxs-lookup"><span data-stu-id="97e34-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97e34-134">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="97e34-134">appliedCategories</span></span>|[<span data-ttu-id="97e34-135">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="97e34-135">plannerAppliedCategories</span></span>](../resources/plannerappliedcategories.md)|<span data-ttu-id="97e34-p105">此任务已应用的类别。有关可能的值，请参阅[已应用的类别](../resources/plannerappliedcategories.md)。</span><span class="sxs-lookup"><span data-stu-id="97e34-p105">The categories to which the task has been applied. See [applied Categories](../resources/plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="97e34-138">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="97e34-138">assigneePriority</span></span>|<span data-ttu-id="97e34-139">String</span><span class="sxs-lookup"><span data-stu-id="97e34-139">String</span></span>|<span data-ttu-id="97e34-p106">用于为列表视图中的此类型项目排序的提示。[此处](../resources/planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="97e34-p106">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="97e34-142">assignments</span><span class="sxs-lookup"><span data-stu-id="97e34-142">assignments</span></span>|[<span data-ttu-id="97e34-143">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="97e34-143">plannerAssignments</span></span>](../resources/plannerassignments.md)|<span data-ttu-id="97e34-144">分配到任务的用户集合。</span><span class="sxs-lookup"><span data-stu-id="97e34-144">The set of users the task is assigned to.</span></span>|
|<span data-ttu-id="97e34-145">bucketId</span><span class="sxs-lookup"><span data-stu-id="97e34-145">bucketId</span></span>|<span data-ttu-id="97e34-146">String</span><span class="sxs-lookup"><span data-stu-id="97e34-146">String</span></span>|<span data-ttu-id="97e34-147">任务所属的存储桶 id。</span><span class="sxs-lookup"><span data-stu-id="97e34-147">Bucket id to which the task belongs.</span></span> <span data-ttu-id="97e34-148">存储桶需要位于任务所在的计划中。</span><span class="sxs-lookup"><span data-stu-id="97e34-148">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="97e34-149">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="97e34-149">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="97e34-150">[格式验证](../resources/tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="97e34-150">[Format validation](../resources/tasks-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="97e34-151">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="97e34-151">conversationThreadId</span></span>|<span data-ttu-id="97e34-152">字符串</span><span class="sxs-lookup"><span data-stu-id="97e34-152">String</span></span>|<span data-ttu-id="97e34-p108">任务对话的线程 id。这是在组中创建的对话线程对象的 id。</span><span class="sxs-lookup"><span data-stu-id="97e34-p108">Thread id of the conversation on the task. This is the id of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="97e34-155">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="97e34-155">dueDateTime</span></span>|<span data-ttu-id="97e34-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97e34-156">DateTimeOffset</span></span>|<span data-ttu-id="97e34-p109">任务截止的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="97e34-p109">Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="97e34-160">orderHint</span><span class="sxs-lookup"><span data-stu-id="97e34-160">orderHint</span></span>|<span data-ttu-id="97e34-161">String</span><span class="sxs-lookup"><span data-stu-id="97e34-161">String</span></span>|<span data-ttu-id="97e34-p110">用于为列表视图中的此类型项目排序的提示。[此处](../resources/planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="97e34-p110">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="97e34-164">percentComplete</span><span class="sxs-lookup"><span data-stu-id="97e34-164">percentComplete</span></span>|<span data-ttu-id="97e34-165">Int32</span><span class="sxs-lookup"><span data-stu-id="97e34-165">Int32</span></span>|<span data-ttu-id="97e34-p111">任务完成的百分比。当设置为 `100` 时，任务被视为完成。</span><span class="sxs-lookup"><span data-stu-id="97e34-p111">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="97e34-168">priority</span><span class="sxs-lookup"><span data-stu-id="97e34-168">priority</span></span>|<span data-ttu-id="97e34-169">Int32</span><span class="sxs-lookup"><span data-stu-id="97e34-169">Int32</span></span>|<span data-ttu-id="97e34-170">任务的优先级。</span><span class="sxs-lookup"><span data-stu-id="97e34-170">Priority of the task.</span></span> <span data-ttu-id="97e34-171">值的有效范围介于和`0` （ `10`含）之间，并且值越低，优先级越`0`低（具有最高`10`优先级，优先级最低）。</span><span class="sxs-lookup"><span data-stu-id="97e34-171">Valid range of values is between `0` and `10` (inclusive), with increasing value being lower priority (`0` has the highest priority and `10` has the lowest priority).</span></span>  <span data-ttu-id="97e34-172">目前，规划者将`0`值`1`和 "紧急"， `2` `3` `4` `5`以及 "重要"、、 `6` `7` 、、和 "低" 的`8` `9` `10`值解释为 "中"。</span><span class="sxs-lookup"><span data-stu-id="97e34-172">Currently, Planner interprets values `0` and `1` as "urgent", `2` and `3` and `4` as "important", `5`, `6`, and `7` as "medium", and `8`, `9`, and `10` as "low".</span></span>  <span data-ttu-id="97e34-173">目前，规划器将设置`1` "紧急"、 `3` "重要" `5` 、"中" 和`9` "低" 的值。</span><span class="sxs-lookup"><span data-stu-id="97e34-173">Currently, Planner sets the value `1` for "urgent", `3` for "important", `5` for "medium", and `9` for "low".</span></span>|
|<span data-ttu-id="97e34-174">startDateTime</span><span class="sxs-lookup"><span data-stu-id="97e34-174">startDateTime</span></span>|<span data-ttu-id="97e34-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97e34-175">DateTimeOffset</span></span>|<span data-ttu-id="97e34-p113">任务开始的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="97e34-p113">Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="97e34-179">title</span><span class="sxs-lookup"><span data-stu-id="97e34-179">title</span></span>|<span data-ttu-id="97e34-180">String</span><span class="sxs-lookup"><span data-stu-id="97e34-180">String</span></span>|<span data-ttu-id="97e34-181">任务的标题。</span><span class="sxs-lookup"><span data-stu-id="97e34-181">Title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="97e34-182">响应</span><span class="sxs-lookup"><span data-stu-id="97e34-182">Response</span></span>

<span data-ttu-id="97e34-183">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[plannerTask](../resources/plannertask.md)对象。</span><span class="sxs-lookup"><span data-stu-id="97e34-183">If successful, this method returns a `200 OK` response code and an updated [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="97e34-p114">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="97e34-p114">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="97e34-187">示例</span><span class="sxs-lookup"><span data-stu-id="97e34-187">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97e34-188">请求</span><span class="sxs-lookup"><span data-stu-id="97e34-188">Request</span></span>
<span data-ttu-id="97e34-189">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="97e34-189">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="97e34-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="97e34-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannertask"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh
Content-type: application/json
Content-length: 247
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "orderHint": "N9917 U2883!"
    }
  },
  "appliedCategories": {
    "category3": true,
    "category4": false
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="97e34-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97e34-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannertask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="97e34-192">响应</span><span class="sxs-lookup"><span data-stu-id="97e34-192">Response</span></span>
<span data-ttu-id="97e34-193">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="97e34-193">Here is an example of the response.</span></span> 

><span data-ttu-id="97e34-p115">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="97e34-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1423

{
  "createdBy": {
    "user": {
      "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
    }
  },
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu",
  "title": "title-value",
  "orderHint": "9223370609546166567W",
  "assigneePriority": "90057581\"",
  "createdDateTime": "2015-03-24T18:36:49.2407981Z",
  "assignments": {
    "6463a5ce-2119-4198-9f2a-628761df4a62": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "assignedDateTime": "2015-03-25T18:38:21.956Z",
      "orderHint": "N9917"
    },
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
        }
      },
      "assignedDateTime": "2017-04-24T22:40:44.5665917",
      "orderHint": "RWk1"
    },
    "aaa27244-1db4-476a-a5cb-004607466324": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "assignedDateTime": "2015-03-25T18:38:21.956Z",
      "orderHint": "U2883"
    }
  },
  "appliedCategories": {
    "category3": true,
    "category5": true,
    "category6": true,
  },
  "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update plannertask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
