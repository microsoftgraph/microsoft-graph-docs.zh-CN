---
title: 获取 educationAssignment
description: " 教师可以查看类中的所有工作分配。"
author: dipakboyed
ms.openlocfilehash: 384f99a48340e51c6d919b96471f31c9fbff27a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341907"
---
# <a name="get-educationassignment"></a><span data-ttu-id="1df1d-103">获取 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="1df1d-103">Get educationAssignment</span></span>

> <span data-ttu-id="1df1d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1df1d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1df1d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1df1d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1df1d-106">要获取的属性和工作分配的关系。</span><span class="sxs-lookup"><span data-stu-id="1df1d-106">Get the properties and relationships of an assignment.</span></span> <span data-ttu-id="1df1d-107">学生只能看到分配分配给它们。教师可以查看类中的所有工作分配。</span><span class="sxs-lookup"><span data-stu-id="1df1d-107">Students can only see assignments assigned to them; teachers can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="1df1d-108">权限</span><span class="sxs-lookup"><span data-stu-id="1df1d-108">Permissions</span></span>
<span data-ttu-id="1df1d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1df1d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1df1d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1df1d-111">Permission type</span></span>      | <span data-ttu-id="1df1d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1df1d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1df1d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1df1d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1df1d-114">EduAssignments.ReadBasic，EduAssignments.ReadWriteBasic，EduAssignments.Read EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1df1d-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="1df1d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1df1d-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1df1d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1df1d-116">Not supported.</span></span>  |
|<span data-ttu-id="1df1d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1df1d-117">Application</span></span> | <span data-ttu-id="1df1d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1df1d-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="1df1d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1df1d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1df1d-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1df1d-120">Optional query parameters</span></span>
<span data-ttu-id="1df1d-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1df1d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1df1d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1df1d-122">Request headers</span></span>
| <span data-ttu-id="1df1d-123">标头</span><span class="sxs-lookup"><span data-stu-id="1df1d-123">Header</span></span>       | <span data-ttu-id="1df1d-124">值</span><span class="sxs-lookup"><span data-stu-id="1df1d-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1df1d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1df1d-125">Authorization</span></span>  | <span data-ttu-id="1df1d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1df1d-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1df1d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1df1d-128">Request body</span></span>
<span data-ttu-id="1df1d-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1df1d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1df1d-130">响应</span><span class="sxs-lookup"><span data-stu-id="1df1d-130">Response</span></span>
<span data-ttu-id="1df1d-131">如果成功，此方法返回`200 OK`响应代码和响应正文中的[educationAssignment](../resources/educationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1df1d-131">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1df1d-132">示例</span><span class="sxs-lookup"><span data-stu-id="1df1d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1df1d-133">请求</span><span class="sxs-lookup"><span data-stu-id="1df1d-133">Request</span></span>
<span data-ttu-id="1df1d-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1df1d-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationassignment"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
##### <a name="response"></a><span data-ttu-id="1df1d-135">响应</span><span class="sxs-lookup"><span data-stu-id="1df1d-135">Response</span></span>
<span data-ttu-id="1df1d-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1df1d-136">The following is an example of the response.</span></span> 

><span data-ttu-id="1df1d-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1df1d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "id": "19002",
  "allowLateSubmissions": true,
  "allowStudentsToAddResourcesToSubmission": true,
  "assignDateTime": "String (timestamp)",
  "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
  "assignedDateTime": "2014-01-01T00:00:00Z",
  "classId": "11006",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "createdDateTime": "2014-01-01T00:00:00Z",
  "displayName": "Mid term exam",
  "dueDateTime": "2014-01-11T00:00:00Z",
  "grading": {
      "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType",
      "maxPoints": 100
  },
  "instructions": {
    "content": "Answer every question correctly",
    "contentType": "Text"
  },
  "lastModifiedBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "lastModifiedDateTime": "2014-01-01T00:00:00Z",
  "status": "assigned"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->