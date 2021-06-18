---
title: 列出课程分配
description: 检索分配对象的列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a0c85c4aaac82583acda75158ec73c31d2d91837
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993074"
---
# <a name="list-class-assignments"></a><span data-ttu-id="0e695-103">列出课程分配</span><span class="sxs-lookup"><span data-stu-id="0e695-103">List class assignments</span></span>

<span data-ttu-id="0e695-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e695-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0e695-105">检索分配对象的列表。</span><span class="sxs-lookup"><span data-stu-id="0e695-105">Retrieve a list of assignment objects.</span></span> 

<span data-ttu-id="0e695-106">教师或使用应用程序权限执行的应用程序可以看到课程的所有作业对象。</span><span class="sxs-lookup"><span data-stu-id="0e695-106">A teacher or an application executing with application permissions can see all assignment objects for the class.</span></span> <span data-ttu-id="0e695-107">学生只能看到分配给他们的作业。</span><span class="sxs-lookup"><span data-stu-id="0e695-107">Students can only see assignments that are assigned to them.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e695-108">权限</span><span class="sxs-lookup"><span data-stu-id="0e695-108">Permissions</span></span>

<span data-ttu-id="0e695-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e695-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0e695-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e695-111">Permission type</span></span>                        | <span data-ttu-id="0e695-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e695-112">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="0e695-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e695-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="0e695-114">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e695-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="0e695-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e695-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e695-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e695-116">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="0e695-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e695-117">Application</span></span>                            | <span data-ttu-id="0e695-118">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e695-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e695-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e695-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0e695-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0e695-120">Optional query parameters</span></span>
<span data-ttu-id="0e695-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0e695-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e695-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e695-122">Request headers</span></span>

| <span data-ttu-id="0e695-123">标头</span><span class="sxs-lookup"><span data-stu-id="0e695-123">Header</span></span>        | <span data-ttu-id="0e695-124">值</span><span class="sxs-lookup"><span data-stu-id="0e695-124">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="0e695-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e695-125">Authorization</span></span> | <span data-ttu-id="0e695-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e695-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e695-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e695-128">Request body</span></span>

<span data-ttu-id="0e695-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0e695-129">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e695-130">响应</span><span class="sxs-lookup"><span data-stu-id="0e695-130">Response</span></span>

<span data-ttu-id="0e695-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [educationAssignment](../resources/educationassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0e695-131">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e695-132">示例</span><span class="sxs-lookup"><span data-stu-id="0e695-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e695-133">请求</span><span class="sxs-lookup"><span data-stu-id="0e695-133">Request</span></span>

<span data-ttu-id="0e695-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0e695-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0e695-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e695-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments
```
# <a name="c"></a>[<span data-ttu-id="0e695-136">C#</span><span class="sxs-lookup"><span data-stu-id="0e695-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-assignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e695-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e695-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-assignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e695-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e695-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-assignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e695-139">Java</span><span class="sxs-lookup"><span data-stu-id="0e695-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-assignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0e695-140">响应</span><span class="sxs-lookup"><span data-stu-id="0e695-140">Response</span></span>

<span data-ttu-id="0e695-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0e695-141">The following is an example of the response.</span></span> 

><span data-ttu-id="0e695-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0e695-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
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
      "addedStudentAction": "none",
      "allowLateSubmissions": true,
      "allowStudentsToAddResourcesToSubmission": true,
      "assignDateTime": "2014-02-01T00:00:00Z",
      "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
      "assignedDateTime": "2014-02-01T00:00:00Z",
      "classId": "11018",
      "closeDateTime": "2014-02-11T00:00:00Z",
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
      "notificationChannelUrl": null,
      "status": "published"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
