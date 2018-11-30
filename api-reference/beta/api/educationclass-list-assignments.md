---
title: 列表分配
description: 检索的 assignment 对象的列表。 教师允许查看类的所有工作分配对象。 学生只能查看分配给他们的工作分配。
ms.openlocfilehash: 664356620e83534c5cd686e0d1df796bd3743a3e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044255"
---
# <a name="list-assignments"></a><span data-ttu-id="d5eba-105">列表分配</span><span class="sxs-lookup"><span data-stu-id="d5eba-105">List assignments</span></span>

> <span data-ttu-id="d5eba-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d5eba-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5eba-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d5eba-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d5eba-108">检索的 assignment 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="d5eba-108">Retrieve a list of assignment objects.</span></span> <span data-ttu-id="d5eba-109">教师允许查看类的所有工作分配对象。</span><span class="sxs-lookup"><span data-stu-id="d5eba-109">A teacher is allowed to see all assignment objects for the class.</span></span> <span data-ttu-id="d5eba-110">学生只能查看分配给他们的工作分配。</span><span class="sxs-lookup"><span data-stu-id="d5eba-110">Students can only see assignments that are assigned to them.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5eba-111">权限</span><span class="sxs-lookup"><span data-stu-id="d5eba-111">Permissions</span></span>
<span data-ttu-id="d5eba-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5eba-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5eba-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5eba-114">Permission type</span></span>      | <span data-ttu-id="d5eba-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5eba-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5eba-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5eba-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d5eba-117">EduAssignments.ReadBasic，EduAssignments.ReadWriteBasic，EduAssignments.Read EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d5eba-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="d5eba-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5eba-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d5eba-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5eba-119">Not supported.</span></span>  |
|<span data-ttu-id="d5eba-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5eba-120">Application</span></span> | <span data-ttu-id="d5eba-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5eba-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d5eba-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5eba-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d5eba-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d5eba-123">Optional query parameters</span></span>
<span data-ttu-id="d5eba-124">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d5eba-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5eba-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5eba-125">Request headers</span></span>
| <span data-ttu-id="d5eba-126">标头</span><span class="sxs-lookup"><span data-stu-id="d5eba-126">Header</span></span>       | <span data-ttu-id="d5eba-127">值</span><span class="sxs-lookup"><span data-stu-id="d5eba-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d5eba-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5eba-128">Authorization</span></span>  | <span data-ttu-id="d5eba-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d5eba-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d5eba-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5eba-131">Request body</span></span>
<span data-ttu-id="d5eba-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d5eba-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d5eba-133">响应</span><span class="sxs-lookup"><span data-stu-id="d5eba-133">Response</span></span>
<span data-ttu-id="d5eba-134">如果成功，此方法返回`200 OK`响应代码和响应正文中的[educationAssignment](../resources/educationassignment.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="d5eba-134">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d5eba-135">示例</span><span class="sxs-lookup"><span data-stu-id="d5eba-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5eba-136">请求</span><span class="sxs-lookup"><span data-stu-id="d5eba-136">Request</span></span>
<span data-ttu-id="d5eba-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d5eba-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/<id>/assignments
```
##### <a name="response"></a><span data-ttu-id="d5eba-138">响应</span><span class="sxs-lookup"><span data-stu-id="d5eba-138">Response</span></span>
<span data-ttu-id="d5eba-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d5eba-139">The following is an example of the response.</span></span> 

><span data-ttu-id="d5eba-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d5eba-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 344

{
  "value": [
    {
      "id": "19002",
      "allowLateSubmissions": true,
      "allowStudentsToAddResourcesToSubmission": true,
      "assignDateTime": "2014-02-01T00:00:00Z",
      "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
      "assignedDateTime": "2014-02-01T00:00:00Z",
      "classId": "11018",
      "createdBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "createdDateTime": "2014-02-01T00:00:00Z",
      "displayName": "published",
      "dueDateTime": "2014-02-01T00:00:00Z",
      "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 100
      },
      "instructions": {
        "contentType": "Text",
        "content": "Read chapters 1 through 3"
      },
      "lastModifiedBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "lastModifiedDateTime": "2014-02-01T00:00:00Z",
      "status": "published"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->