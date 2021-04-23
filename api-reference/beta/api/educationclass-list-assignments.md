---
title: 列出作业
description: 检索分配对象的列表。 允许教师或使用应用程序权限执行的应用程序查看课程的所有作业对象。 学生只能看到分配给他们的作业。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 474de134eceb456585a5c8df6d12347c4b9a802c
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961259"
---
# <a name="list-assignments"></a><span data-ttu-id="d221a-105">列出作业</span><span class="sxs-lookup"><span data-stu-id="d221a-105">List assignments</span></span>

<span data-ttu-id="d221a-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d221a-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d221a-107">检索分配对象的列表。</span><span class="sxs-lookup"><span data-stu-id="d221a-107">Retrieve a list of assignment objects.</span></span> <span data-ttu-id="d221a-108">允许教师或使用应用程序权限执行的应用程序查看课程的所有作业对象。</span><span class="sxs-lookup"><span data-stu-id="d221a-108">A teacher or an application executing with application permissions is allowed to see all assignment objects for the class.</span></span> <span data-ttu-id="d221a-109">学生只能看到分配给他们的作业。</span><span class="sxs-lookup"><span data-stu-id="d221a-109">Students can only see assignments that are assigned to them.</span></span>

## <a name="permissions"></a><span data-ttu-id="d221a-110">权限</span><span class="sxs-lookup"><span data-stu-id="d221a-110">Permissions</span></span>

<span data-ttu-id="d221a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d221a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d221a-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="d221a-113">Permission type</span></span>                        | <span data-ttu-id="d221a-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d221a-114">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d221a-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d221a-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="d221a-116">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d221a-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="d221a-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d221a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d221a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d221a-118">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="d221a-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="d221a-119">Application</span></span>                            | <span data-ttu-id="d221a-120">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d221a-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d221a-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d221a-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d221a-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d221a-122">Optional query parameters</span></span>
<span data-ttu-id="d221a-123">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d221a-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d221a-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="d221a-124">Request headers</span></span>

| <span data-ttu-id="d221a-125">标头</span><span class="sxs-lookup"><span data-stu-id="d221a-125">Header</span></span>        | <span data-ttu-id="d221a-126">值</span><span class="sxs-lookup"><span data-stu-id="d221a-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="d221a-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d221a-127">Authorization</span></span> | <span data-ttu-id="d221a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d221a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d221a-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="d221a-130">Request body</span></span>

<span data-ttu-id="d221a-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d221a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d221a-132">响应</span><span class="sxs-lookup"><span data-stu-id="d221a-132">Response</span></span>

<span data-ttu-id="d221a-133">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [educationAssignment](../resources/educationassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d221a-133">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d221a-134">示例</span><span class="sxs-lookup"><span data-stu-id="d221a-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d221a-135">请求</span><span class="sxs-lookup"><span data-stu-id="d221a-135">Request</span></span>

<span data-ttu-id="d221a-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d221a-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignments
```

##### <a name="response"></a><span data-ttu-id="d221a-137">响应</span><span class="sxs-lookup"><span data-stu-id="d221a-137">Response</span></span>

<span data-ttu-id="d221a-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d221a-138">The following is an example of the response.</span></span> 

><span data-ttu-id="d221a-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d221a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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