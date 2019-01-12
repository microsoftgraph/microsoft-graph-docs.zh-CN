---
title: 更新 plannertaskdetails
description: 更新 **plannertaskdetails** 对象的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 04adf9c53907962f0298541f5d8c28402bc2b613
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960551"
---
# <a name="update-plannertaskdetails"></a><span data-ttu-id="f9c20-103">更新 plannertaskdetails</span><span class="sxs-lookup"><span data-stu-id="f9c20-103">Update plannertaskdetails</span></span>

> <span data-ttu-id="f9c20-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f9c20-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9c20-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f9c20-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f9c20-106">更新 **plannertaskdetails** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f9c20-106">Update the properties of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f9c20-107">权限</span><span class="sxs-lookup"><span data-stu-id="f9c20-107">Permissions</span></span>
<span data-ttu-id="f9c20-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9c20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9c20-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9c20-110">Permission type</span></span>      | <span data-ttu-id="f9c20-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f9c20-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9c20-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9c20-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f9c20-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9c20-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f9c20-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9c20-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9c20-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9c20-115">Not supported.</span></span>    |
|<span data-ttu-id="f9c20-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9c20-116">Application</span></span> | <span data-ttu-id="f9c20-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9c20-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9c20-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9c20-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="f9c20-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="f9c20-119">Optional request headers</span></span>
| <span data-ttu-id="f9c20-120">名称</span><span class="sxs-lookup"><span data-stu-id="f9c20-120">Name</span></span>       | <span data-ttu-id="f9c20-121">说明</span><span class="sxs-lookup"><span data-stu-id="f9c20-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f9c20-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9c20-122">Authorization</span></span>  | <span data-ttu-id="f9c20-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f9c20-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f9c20-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="f9c20-125">If-Match</span></span>  | <span data-ttu-id="f9c20-p104">要更新的 **plannerTaskDetails** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="f9c20-p104">Last known ETag value for the **plannerTaskDetails** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9c20-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9c20-128">Request body</span></span>
<span data-ttu-id="f9c20-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="f9c20-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f9c20-132">属性</span><span class="sxs-lookup"><span data-stu-id="f9c20-132">Property</span></span>     | <span data-ttu-id="f9c20-133">类型</span><span class="sxs-lookup"><span data-stu-id="f9c20-133">Type</span></span>   |<span data-ttu-id="f9c20-134">说明</span><span class="sxs-lookup"><span data-stu-id="f9c20-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9c20-135">checklist</span><span class="sxs-lookup"><span data-stu-id="f9c20-135">checklist</span></span>|[<span data-ttu-id="f9c20-136">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="f9c20-136">plannerChecklistItems</span></span>](../resources/plannerchecklistitems.md)|<span data-ttu-id="f9c20-137">任务上的检查表项目集合。</span><span class="sxs-lookup"><span data-stu-id="f9c20-137">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="f9c20-138">说明</span><span class="sxs-lookup"><span data-stu-id="f9c20-138">description</span></span>|<span data-ttu-id="f9c20-139">String</span><span class="sxs-lookup"><span data-stu-id="f9c20-139">String</span></span>|<span data-ttu-id="f9c20-140">任务描述</span><span class="sxs-lookup"><span data-stu-id="f9c20-140">Description of the task</span></span>|
|<span data-ttu-id="f9c20-141">previewType</span><span class="sxs-lookup"><span data-stu-id="f9c20-141">previewType</span></span>|<span data-ttu-id="f9c20-142">string</span><span class="sxs-lookup"><span data-stu-id="f9c20-142">string</span></span>|<span data-ttu-id="f9c20-p106">这将设置显示在任务上的预览类型。可能的值是：`automatic`、`noPreview`、`checklist`、`description`、`reference`。当设为 `automatic` 时，由查看任务的应用选择显示的预览。</span><span class="sxs-lookup"><span data-stu-id="f9c20-p106">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="f9c20-146">references</span><span class="sxs-lookup"><span data-stu-id="f9c20-146">references</span></span>|[<span data-ttu-id="f9c20-147">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="f9c20-147">plannerExternalReferences</span></span>](../resources/plannerexternalreferences.md)|<span data-ttu-id="f9c20-148">任务上的引用集合。</span><span class="sxs-lookup"><span data-stu-id="f9c20-148">The collection of references on the task.</span></span>|

## <a name="response"></a><span data-ttu-id="f9c20-149">响应</span><span class="sxs-lookup"><span data-stu-id="f9c20-149">Response</span></span>

<span data-ttu-id="f9c20-150">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [plannerTaskDetails](../resources/plannertaskdetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f9c20-150">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="f9c20-p107">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="f9c20-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="f9c20-154">示例</span><span class="sxs-lookup"><span data-stu-id="f9c20-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9c20-155">请求</span><span class="sxs-lookup"><span data-stu-id="f9c20-155">Request</span></span>
<span data-ttu-id="f9c20-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f9c20-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannertaskdetails"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/details
Content-type: application/json
Content-length: 857
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
##### <a name="response"></a><span data-ttu-id="f9c20-157">响应</span><span class="sxs-lookup"><span data-stu-id="f9c20-157">Response</span></span>
<span data-ttu-id="f9c20-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f9c20-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update plannertaskdetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
