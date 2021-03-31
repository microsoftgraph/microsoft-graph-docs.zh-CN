---
title: 更新 plannertaskdetails
description: 更新 **plannertaskdetails** 对象的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 02c558b1a28ad4348f28c3f7738bf6e2b21ddd3e
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473332"
---
# <a name="update-plannertaskdetails"></a><span data-ttu-id="5e34d-103">更新 plannertaskdetails</span><span class="sxs-lookup"><span data-stu-id="5e34d-103">Update plannertaskdetails</span></span>

<span data-ttu-id="5e34d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e34d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e34d-105">更新 **plannertaskdetails** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5e34d-105">Update the properties of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5e34d-106">权限</span><span class="sxs-lookup"><span data-stu-id="5e34d-106">Permissions</span></span>
<span data-ttu-id="5e34d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e34d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e34d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e34d-109">Permission type</span></span>      | <span data-ttu-id="5e34d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5e34d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e34d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e34d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5e34d-112">Tasks.ReadWrite、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e34d-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5e34d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e34d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e34d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e34d-114">Not supported.</span></span>    |
|<span data-ttu-id="5e34d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e34d-115">Application</span></span> | <span data-ttu-id="5e34d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e34d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e34d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e34d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="5e34d-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="5e34d-118">Optional request headers</span></span>
| <span data-ttu-id="5e34d-119">名称</span><span class="sxs-lookup"><span data-stu-id="5e34d-119">Name</span></span>       | <span data-ttu-id="5e34d-120">说明</span><span class="sxs-lookup"><span data-stu-id="5e34d-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5e34d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e34d-121">Authorization</span></span>  | <span data-ttu-id="5e34d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5e34d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5e34d-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="5e34d-124">If-Match</span></span>  | <span data-ttu-id="5e34d-p103">要更新的 **plannerTaskDetails** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="5e34d-p103">Last known ETag value for the **plannerTaskDetails** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e34d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e34d-127">Request body</span></span>
<span data-ttu-id="5e34d-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="5e34d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5e34d-131">属性</span><span class="sxs-lookup"><span data-stu-id="5e34d-131">Property</span></span>     | <span data-ttu-id="5e34d-132">类型</span><span class="sxs-lookup"><span data-stu-id="5e34d-132">Type</span></span>   |<span data-ttu-id="5e34d-133">说明</span><span class="sxs-lookup"><span data-stu-id="5e34d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e34d-134">checklist</span><span class="sxs-lookup"><span data-stu-id="5e34d-134">checklist</span></span>|[<span data-ttu-id="5e34d-135">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="5e34d-135">plannerChecklistItems</span></span>](../resources/plannerchecklistitems.md)|<span data-ttu-id="5e34d-136">任务上的检查表项目集合。</span><span class="sxs-lookup"><span data-stu-id="5e34d-136">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="5e34d-137">说明</span><span class="sxs-lookup"><span data-stu-id="5e34d-137">description</span></span>|<span data-ttu-id="5e34d-138">String</span><span class="sxs-lookup"><span data-stu-id="5e34d-138">String</span></span>|<span data-ttu-id="5e34d-139">任务描述</span><span class="sxs-lookup"><span data-stu-id="5e34d-139">Description of the task</span></span>|
|<span data-ttu-id="5e34d-140">previewType</span><span class="sxs-lookup"><span data-stu-id="5e34d-140">previewType</span></span>|<span data-ttu-id="5e34d-141">string</span><span class="sxs-lookup"><span data-stu-id="5e34d-141">string</span></span>|<span data-ttu-id="5e34d-p105">这将设置显示在任务上的预览类型。可能的值是：`automatic`、`noPreview`、`checklist`、`description`、`reference`。当设为 `automatic` 时，由查看任务的应用选择显示的预览。</span><span class="sxs-lookup"><span data-stu-id="5e34d-p105">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="5e34d-145">references</span><span class="sxs-lookup"><span data-stu-id="5e34d-145">references</span></span>|[<span data-ttu-id="5e34d-146">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="5e34d-146">plannerExternalReferences</span></span>](../resources/plannerexternalreferences.md)|<span data-ttu-id="5e34d-147">任务上的引用集合。</span><span class="sxs-lookup"><span data-stu-id="5e34d-147">The collection of references on the task.</span></span>|

## <a name="response"></a><span data-ttu-id="5e34d-148">响应</span><span class="sxs-lookup"><span data-stu-id="5e34d-148">Response</span></span>

<span data-ttu-id="5e34d-149">如果成功，此方法将返回 `204 No Content` 响应和空内容。</span><span class="sxs-lookup"><span data-stu-id="5e34d-149">If successful, this method returns `204 No Content` response and empty content.</span></span> <span data-ttu-id="5e34d-150">如果请求指定具有首选项的标头，则此方法在响应正文中返回 响应代码和更新的 `Prefer` `return=representation` `200 OK` [plannerTaskDetails](../resources/plannertaskdetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5e34d-150">If the request specifies `Prefer` header with `return=representation` preference, then this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="5e34d-p107">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="5e34d-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="5e34d-154">示例</span><span class="sxs-lookup"><span data-stu-id="5e34d-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e34d-155">请求</span><span class="sxs-lookup"><span data-stu-id="5e34d-155">Request</span></span>
<span data-ttu-id="5e34d-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5e34d-156">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5e34d-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e34d-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannertaskdetails"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/details
Content-type: application/json
Content-length: 857
Prefer: return=representation
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "previewType": "noPreview",
  "references": {
    "http%3A//developer%2Emicrosoft%2Ecom":{
      "@odata.type": "microsoft.graph.plannerExternalReference",
      "alias": "Documentation",
      "previewPriority": " !",
      "type": "Other"
    },
    "https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer":{
      "@odata.type": "microsoft.graph.plannerExternalReference",
      "previewPriority": "  !!",
    },
    "http%3A//www%2Ebing%2Ecom": null
  },
  "checklist": {
    "95e27074-6c4a-447a-aa24-9d718a0b86fa":{
      "@odata.type": "microsoft.graph.plannerChecklistItem",
      "title": "Update task details",
      "isChecked": true
    },
    "d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff":{
      "@odata.type": "microsoft.graph.plannerChecklistItem",
      "isChecked": true,
    },
    "a93c93c5-10a6-4167-9551-8bafa09967a7": null
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="5e34d-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e34d-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannertaskdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="5e34d-159">C#</span><span class="sxs-lookup"><span data-stu-id="5e34d-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannertaskdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5e34d-160">响应</span><span class="sxs-lookup"><span data-stu-id="5e34d-160">Response</span></span>
<span data-ttu-id="5e34d-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5e34d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTaskDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1793

{
  "description": "Task details properties:\nchecklist:Sub items\nreferences:Related links",
  "previewType": "automatic",
  "references": {
    "https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer": {
      "@odata.type": "#microsoft.graph.plannerExternalReference",
      "alias": "Graph Explorer",
      "type": "Other",
      "previewPriority": "8599273",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    },
    "http%3A//developer%2Emicrosoft%2Ecom": {
      "@odata.type": "#microsoft.graph.plannerExternalReference",
      "alias": "Documentation",
      "type": "Other",
      "previewPriority": "90727736",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    }
  },
  "checklist": {
    "d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff": {
      "@odata.type": "#microsoft.graph.plannerChecklistItem",
      "isChecked": true,
      "title": "Try reading task details",
      "orderHint": "a93c93c5^",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    },
    "95e27074-6c4a-447a-aa24-9d718a0b86f": {
      "@odata.type": "#microsoft.graph.plannerChecklistItem",
      "isChecked": true,
      "title": "Update task details",
      "orderHint": "8587094707721254251P]",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    }
  },
  "id": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update plannertaskdetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


