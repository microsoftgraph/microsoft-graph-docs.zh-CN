# <a name="update-plannertaskdetails"></a><span data-ttu-id="0bbfd-101">更新 plannertaskdetails</span><span class="sxs-lookup"><span data-stu-id="0bbfd-101">Update plannertaskdetails</span></span>

<span data-ttu-id="0bbfd-102">更新 **plannertaskdetails** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-102">Update the properties of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0bbfd-103">权限</span><span class="sxs-lookup"><span data-stu-id="0bbfd-103">Permissions</span></span>
<span data-ttu-id="0bbfd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0bbfd-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="0bbfd-106">Permission type</span></span>      | <span data-ttu-id="0bbfd-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0bbfd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0bbfd-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0bbfd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0bbfd-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bbfd-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0bbfd-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0bbfd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bbfd-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-111">Not supported.</span></span>    |
|<span data-ttu-id="0bbfd-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="0bbfd-112">Application</span></span> | <span data-ttu-id="0bbfd-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bbfd-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0bbfd-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="0bbfd-115">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="0bbfd-115">Optional request headers</span></span>
| <span data-ttu-id="0bbfd-116">名称</span><span class="sxs-lookup"><span data-stu-id="0bbfd-116">Name</span></span>       | <span data-ttu-id="0bbfd-117">说明</span><span class="sxs-lookup"><span data-stu-id="0bbfd-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0bbfd-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bbfd-118">Authorization</span></span>  | <span data-ttu-id="0bbfd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0bbfd-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="0bbfd-121">If-Match</span></span>  | <span data-ttu-id="0bbfd-p103">要更新的 **plannerTaskDetails** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-p103">Last known ETag value for the **plannerTaskDetails** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bbfd-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="0bbfd-124">Request body</span></span>
<span data-ttu-id="0bbfd-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0bbfd-128">属性</span><span class="sxs-lookup"><span data-stu-id="0bbfd-128">Property</span></span>     | <span data-ttu-id="0bbfd-129">类型</span><span class="sxs-lookup"><span data-stu-id="0bbfd-129">Type</span></span>   |<span data-ttu-id="0bbfd-130">说明</span><span class="sxs-lookup"><span data-stu-id="0bbfd-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0bbfd-131">checklist</span><span class="sxs-lookup"><span data-stu-id="0bbfd-131">checklist</span></span>|[<span data-ttu-id="0bbfd-132">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="0bbfd-132">plannerChecklistItems</span></span>](../resources/plannerchecklistitems.md)|<span data-ttu-id="0bbfd-133">任务上的检查表项目集合。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-133">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="0bbfd-134">description</span><span class="sxs-lookup"><span data-stu-id="0bbfd-134">description</span></span>|<span data-ttu-id="0bbfd-135">String</span><span class="sxs-lookup"><span data-stu-id="0bbfd-135">String</span></span>|<span data-ttu-id="0bbfd-136">任务描述</span><span class="sxs-lookup"><span data-stu-id="0bbfd-136">Description of the task</span></span>|
|<span data-ttu-id="0bbfd-137">previewType</span><span class="sxs-lookup"><span data-stu-id="0bbfd-137">previewType</span></span>|<span data-ttu-id="0bbfd-138">string</span><span class="sxs-lookup"><span data-stu-id="0bbfd-138">string</span></span>|<span data-ttu-id="0bbfd-p105">这将设置显示在任务上的预览类型。可能的值是：`automatic`、`noPreview`、`checklist`、`description`、`reference`。当设为 `automatic` 时，由查看任务的应用选择显示的预览。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-p105">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="0bbfd-142">references</span><span class="sxs-lookup"><span data-stu-id="0bbfd-142">references</span></span>|[<span data-ttu-id="0bbfd-143">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="0bbfd-143">plannerExternalReferences</span></span>](../resources/plannerexternalreferences.md)|<span data-ttu-id="0bbfd-144">任务上的引用集合。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-144">The collection of references on the task.</span></span>|

## <a name="response"></a><span data-ttu-id="0bbfd-145">响应</span><span class="sxs-lookup"><span data-stu-id="0bbfd-145">Response</span></span>

<span data-ttu-id="0bbfd-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [plannerTaskDetails](../resources/plannertaskdetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-146">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="0bbfd-p106">此方法可以返回任何 [HTTP 状态代码](../../../concepts/errors.md)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner_overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-p106">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="0bbfd-150">示例</span><span class="sxs-lookup"><span data-stu-id="0bbfd-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0bbfd-151">请求</span><span class="sxs-lookup"><span data-stu-id="0bbfd-151">Request</span></span>
<span data-ttu-id="0bbfd-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannertaskdetails"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/details
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
      "ischecked": true
    },
    "d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff":{
      "@odata.type": "microsoft.graph.plannerChecklistItem",
      "isChecked": true,
    },
    "a93c93c5-10a6-4167-9551-8bafa09967a7": null
  }
}
```
##### <a name="response"></a><span data-ttu-id="0bbfd-153">响应</span><span class="sxs-lookup"><span data-stu-id="0bbfd-153">Response</span></span>
<span data-ttu-id="0bbfd-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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