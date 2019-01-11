---
title: 更新 plannerTask
description: 更新 **plannertask** 对象的属性。
localization_priority: Normal
ms.openlocfilehash: b753e62e463ecd3a19e16ddaca5d2fd03c90a44b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838757"
---
# <a name="update-plannertask"></a><span data-ttu-id="72620-103">更新 plannerTask</span><span class="sxs-lookup"><span data-stu-id="72620-103">Update plannertask</span></span>

> <span data-ttu-id="72620-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="72620-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72620-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="72620-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="72620-106">更新 **plannertask** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="72620-106">Update the properties of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="72620-107">权限</span><span class="sxs-lookup"><span data-stu-id="72620-107">Permissions</span></span>
<span data-ttu-id="72620-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72620-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72620-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="72620-110">Permission type</span></span>      | <span data-ttu-id="72620-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="72620-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72620-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72620-112">Delegated (work or school account)</span></span> | <span data-ttu-id="72620-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72620-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="72620-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72620-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72620-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="72620-115">Not supported.</span></span>    |
|<span data-ttu-id="72620-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="72620-116">Application</span></span> | <span data-ttu-id="72620-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="72620-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72620-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72620-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="72620-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="72620-119">Optional request headers</span></span>
| <span data-ttu-id="72620-120">名称</span><span class="sxs-lookup"><span data-stu-id="72620-120">Name</span></span>       | <span data-ttu-id="72620-121">说明</span><span class="sxs-lookup"><span data-stu-id="72620-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="72620-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="72620-122">Authorization</span></span>  | <span data-ttu-id="72620-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="72620-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="72620-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="72620-125">If-Match</span></span>  | <span data-ttu-id="72620-p104">要更新的 **plannerTask** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="72620-p104">Last known ETag value for the **plannerTask** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="72620-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="72620-128">Request body</span></span>
<span data-ttu-id="72620-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="72620-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="72620-132">属性</span><span class="sxs-lookup"><span data-stu-id="72620-132">Property</span></span>     | <span data-ttu-id="72620-133">类型</span><span class="sxs-lookup"><span data-stu-id="72620-133">Type</span></span>   |<span data-ttu-id="72620-134">说明</span><span class="sxs-lookup"><span data-stu-id="72620-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72620-135">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="72620-135">appliedCategories</span></span>|[<span data-ttu-id="72620-136">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="72620-136">plannerAppliedCategories</span></span>](../resources/plannerappliedcategories.md)|<span data-ttu-id="72620-p106">此任务已应用的类别。有关可能的值，请参阅[已应用的类别](../resources/plannerappliedcategories.md)。</span><span class="sxs-lookup"><span data-stu-id="72620-p106">The categories to which the task has been applied. See [applied Categories](../resources/plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="72620-139">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="72620-139">assigneePriority</span></span>|<span data-ttu-id="72620-140">String</span><span class="sxs-lookup"><span data-stu-id="72620-140">String</span></span>|<span data-ttu-id="72620-p107">提示用于为列表视图中的此类项目排序。[此处](../resources/planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="72620-p107">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="72620-143">assignments</span><span class="sxs-lookup"><span data-stu-id="72620-143">assignments</span></span>|[<span data-ttu-id="72620-144">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="72620-144">plannerAssignments</span></span>](../resources/plannerassignments.md)|<span data-ttu-id="72620-145">分配到任务的用户集合。</span><span class="sxs-lookup"><span data-stu-id="72620-145">The set of users the task is assigned to.</span></span>|
|<span data-ttu-id="72620-146">bucketId</span><span class="sxs-lookup"><span data-stu-id="72620-146">bucketId</span></span>|<span data-ttu-id="72620-147">字符串</span><span class="sxs-lookup"><span data-stu-id="72620-147">String</span></span>|<span data-ttu-id="72620-148">任务所属的地址散列表元 id。</span><span class="sxs-lookup"><span data-stu-id="72620-148">Bucket id to which the task belongs.</span></span> <span data-ttu-id="72620-149">地址散列表元需要在计划中的任务。</span><span class="sxs-lookup"><span data-stu-id="72620-149">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="72620-150">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="72620-150">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="72620-151">服务上执行[格式验证](../resources/tasks-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="72620-151">[Format validation](../resources/tasks-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="72620-152">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="72620-152">conversationThreadId</span></span>|<span data-ttu-id="72620-153">String</span><span class="sxs-lookup"><span data-stu-id="72620-153">String</span></span>|<span data-ttu-id="72620-p109">任务对话的线程 id。这是在组中创建的对话线程对象的 id。</span><span class="sxs-lookup"><span data-stu-id="72620-p109">Thread id of the conversation on the task. This is the id of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="72620-156">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="72620-156">dueDateTime</span></span>|<span data-ttu-id="72620-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72620-157">DateTimeOffset</span></span>|<span data-ttu-id="72620-p110">任务截止的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="72620-p110">Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="72620-161">orderHint</span><span class="sxs-lookup"><span data-stu-id="72620-161">orderHint</span></span>|<span data-ttu-id="72620-162">String</span><span class="sxs-lookup"><span data-stu-id="72620-162">String</span></span>|<span data-ttu-id="72620-p111">提示用于为列表视图中的此类项目排序。[此处](../resources/planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="72620-p111">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="72620-165">percentComplete</span><span class="sxs-lookup"><span data-stu-id="72620-165">percentComplete</span></span>|<span data-ttu-id="72620-166">Int32</span><span class="sxs-lookup"><span data-stu-id="72620-166">Int32</span></span>|<span data-ttu-id="72620-p112">任务完成的百分比。当设置为 `100` 时，任务被视为完成。</span><span class="sxs-lookup"><span data-stu-id="72620-p112">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="72620-169">planId</span><span class="sxs-lookup"><span data-stu-id="72620-169">planId</span></span>|<span data-ttu-id="72620-170">String</span><span class="sxs-lookup"><span data-stu-id="72620-170">String</span></span>|<span data-ttu-id="72620-171">此任务所属的计划 id。</span><span class="sxs-lookup"><span data-stu-id="72620-171">Plan id to which the task belongs.</span></span>|
|<span data-ttu-id="72620-172">startDateTime</span><span class="sxs-lookup"><span data-stu-id="72620-172">startDateTime</span></span>|<span data-ttu-id="72620-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72620-173">DateTimeOffset</span></span>|<span data-ttu-id="72620-p113">任务开始的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="72620-p113">Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="72620-177">title</span><span class="sxs-lookup"><span data-stu-id="72620-177">title</span></span>|<span data-ttu-id="72620-178">String</span><span class="sxs-lookup"><span data-stu-id="72620-178">String</span></span>|<span data-ttu-id="72620-179">任务的标题。</span><span class="sxs-lookup"><span data-stu-id="72620-179">Title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="72620-180">响应</span><span class="sxs-lookup"><span data-stu-id="72620-180">Response</span></span>

<span data-ttu-id="72620-181">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [plannerTask](../resources/plannertask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="72620-181">If successful, this method returns a `200 OK` response code and updated [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="72620-p114">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="72620-p114">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="72620-185">示例</span><span class="sxs-lookup"><span data-stu-id="72620-185">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72620-186">请求</span><span class="sxs-lookup"><span data-stu-id="72620-186">Request</span></span>
<span data-ttu-id="72620-187">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="72620-187">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="72620-188">响应</span><span class="sxs-lookup"><span data-stu-id="72620-188">Response</span></span>
<span data-ttu-id="72620-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="72620-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update plannertask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
