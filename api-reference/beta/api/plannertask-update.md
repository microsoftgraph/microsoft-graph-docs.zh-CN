---
title: 更新 plannerTask
description: 更新 **plannertask** 对象的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: ae2551165405161e071d23cf704851ac18fbf73e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538845"
---
# <a name="update-plannertask"></a><span data-ttu-id="4f774-103">更新 plannerTask</span><span class="sxs-lookup"><span data-stu-id="4f774-103">Update plannertask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f774-104">更新 **plannertask** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4f774-104">Update the properties of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4f774-105">权限</span><span class="sxs-lookup"><span data-stu-id="4f774-105">Permissions</span></span>
<span data-ttu-id="4f774-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f774-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f774-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f774-108">Permission type</span></span>      | <span data-ttu-id="4f774-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4f774-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f774-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f774-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4f774-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f774-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4f774-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f774-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f774-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f774-113">Not supported.</span></span>    |
|<span data-ttu-id="4f774-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4f774-114">Application</span></span> | <span data-ttu-id="4f774-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f774-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f774-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f774-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="4f774-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="4f774-117">Optional request headers</span></span>
| <span data-ttu-id="4f774-118">名称</span><span class="sxs-lookup"><span data-stu-id="4f774-118">Name</span></span>       | <span data-ttu-id="4f774-119">说明</span><span class="sxs-lookup"><span data-stu-id="4f774-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4f774-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f774-120">Authorization</span></span>  | <span data-ttu-id="4f774-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4f774-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4f774-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="4f774-123">If-Match</span></span>  | <span data-ttu-id="4f774-p103">要更新的 **plannerTask** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="4f774-p103">Last known ETag value for the **plannerTask** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f774-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f774-126">Request body</span></span>
<span data-ttu-id="4f774-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="4f774-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4f774-130">属性</span><span class="sxs-lookup"><span data-stu-id="4f774-130">Property</span></span>     | <span data-ttu-id="4f774-131">类型</span><span class="sxs-lookup"><span data-stu-id="4f774-131">Type</span></span>   |<span data-ttu-id="4f774-132">说明</span><span class="sxs-lookup"><span data-stu-id="4f774-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f774-133">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="4f774-133">appliedCategories</span></span>|[<span data-ttu-id="4f774-134">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="4f774-134">plannerAppliedCategories</span></span>](../resources/plannerappliedcategories.md)|<span data-ttu-id="4f774-p105">此任务已应用的类别。有关可能的值，请参阅[已应用的类别](../resources/plannerappliedcategories.md)。</span><span class="sxs-lookup"><span data-stu-id="4f774-p105">The categories to which the task has been applied. See [applied Categories](../resources/plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="4f774-137">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="4f774-137">assigneePriority</span></span>|<span data-ttu-id="4f774-138">String</span><span class="sxs-lookup"><span data-stu-id="4f774-138">String</span></span>|<span data-ttu-id="4f774-p106">用于为列表视图中的此类型项目排序的提示。[此处](../resources/planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="4f774-p106">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="4f774-141">assignments</span><span class="sxs-lookup"><span data-stu-id="4f774-141">assignments</span></span>|[<span data-ttu-id="4f774-142">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="4f774-142">plannerAssignments</span></span>](../resources/plannerassignments.md)|<span data-ttu-id="4f774-143">分配到任务的用户集合。</span><span class="sxs-lookup"><span data-stu-id="4f774-143">The set of users the task is assigned to.</span></span>|
|<span data-ttu-id="4f774-144">bucketId</span><span class="sxs-lookup"><span data-stu-id="4f774-144">bucketId</span></span>|<span data-ttu-id="4f774-145">String</span><span class="sxs-lookup"><span data-stu-id="4f774-145">String</span></span>|<span data-ttu-id="4f774-146">任务所属的存储桶 id。</span><span class="sxs-lookup"><span data-stu-id="4f774-146">Bucket id to which the task belongs.</span></span> <span data-ttu-id="4f774-147">存储桶需要位于任务所在的计划中。</span><span class="sxs-lookup"><span data-stu-id="4f774-147">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="4f774-148">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="4f774-148">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="4f774-149">[格式验证](../resources/tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="4f774-149">[Format validation](../resources/tasks-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="4f774-150">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="4f774-150">conversationThreadId</span></span>|<span data-ttu-id="4f774-151">字符串</span><span class="sxs-lookup"><span data-stu-id="4f774-151">String</span></span>|<span data-ttu-id="4f774-p108">任务对话的线程 id。这是在组中创建的对话线程对象的 id。</span><span class="sxs-lookup"><span data-stu-id="4f774-p108">Thread id of the conversation on the task. This is the id of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="4f774-154">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="4f774-154">dueDateTime</span></span>|<span data-ttu-id="4f774-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f774-155">DateTimeOffset</span></span>|<span data-ttu-id="4f774-p109">任务截止的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4f774-p109">Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4f774-159">orderHint</span><span class="sxs-lookup"><span data-stu-id="4f774-159">orderHint</span></span>|<span data-ttu-id="4f774-160">String</span><span class="sxs-lookup"><span data-stu-id="4f774-160">String</span></span>|<span data-ttu-id="4f774-p110">用于为列表视图中的此类型项目排序的提示。[此处](../resources/planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="4f774-p110">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="4f774-163">percentComplete</span><span class="sxs-lookup"><span data-stu-id="4f774-163">percentComplete</span></span>|<span data-ttu-id="4f774-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4f774-164">Int32</span></span>|<span data-ttu-id="4f774-p111">任务完成的百分比。当设置为 `100` 时，任务被视为完成。</span><span class="sxs-lookup"><span data-stu-id="4f774-p111">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="4f774-167">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4f774-167">startDateTime</span></span>|<span data-ttu-id="4f774-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f774-168">DateTimeOffset</span></span>|<span data-ttu-id="4f774-p112">任务开始的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4f774-p112">Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4f774-172">title</span><span class="sxs-lookup"><span data-stu-id="4f774-172">title</span></span>|<span data-ttu-id="4f774-173">String</span><span class="sxs-lookup"><span data-stu-id="4f774-173">String</span></span>|<span data-ttu-id="4f774-174">任务的标题。</span><span class="sxs-lookup"><span data-stu-id="4f774-174">Title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="4f774-175">响应</span><span class="sxs-lookup"><span data-stu-id="4f774-175">Response</span></span>

<span data-ttu-id="4f774-176">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [plannerTask](../resources/plannertask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4f774-176">If successful, this method returns a `200 OK` response code and updated [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="4f774-p113">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="4f774-p113">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="4f774-180">示例</span><span class="sxs-lookup"><span data-stu-id="4f774-180">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4f774-181">请求</span><span class="sxs-lookup"><span data-stu-id="4f774-181">Request</span></span>
<span data-ttu-id="4f774-182">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4f774-182">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="4f774-183">响应</span><span class="sxs-lookup"><span data-stu-id="4f774-183">Response</span></span>
<span data-ttu-id="4f774-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4f774-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/plannertask-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
