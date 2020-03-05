---
title: 列出作业
description: 返回为所有类分配给用户的工作分配的列表。 此实用程序命名空间允许呼叫者在单个呼叫中查找所有学生的分配，而无需从每个班级中请求分配。 工作分配列表包含从类命名空间中获取工作分配的详细信息所需的内容。 分配上的所有其他操作都应使用类命名空间。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 410514a30bb0f09d031fe26b2f0f02907dc943e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42423796"
---
# <a name="list-assignments"></a><span data-ttu-id="38e4c-106">列出作业</span><span class="sxs-lookup"><span data-stu-id="38e4c-106">List assignments</span></span>

<span data-ttu-id="38e4c-107">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="38e4c-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38e4c-108">返回为所有类分配给用户的工作分配的列表。</span><span class="sxs-lookup"><span data-stu-id="38e4c-108">Returns a list of assignments assigned to a user for all classes.</span></span> <span data-ttu-id="38e4c-109">此实用程序命名空间允许呼叫者在单个呼叫中查找所有学生的分配，而无需从每个班级中请求分配。</span><span class="sxs-lookup"><span data-stu-id="38e4c-109">This utility namespace allows a caller to find all a student's assignments in a single call rather than having to request assignments from each class.</span></span> <span data-ttu-id="38e4c-110">工作分配列表包含从类命名空间中获取工作分配的详细信息所需的内容。</span><span class="sxs-lookup"><span data-stu-id="38e4c-110">The assignment list contains what is needed to get the detailed information for the assignment from within the class namespace.</span></span> <span data-ttu-id="38e4c-111">分配上的所有其他操作都应使用类命名空间。</span><span class="sxs-lookup"><span data-stu-id="38e4c-111">All other operations on the assignment should use the class namespace.</span></span>

## <a name="permissions"></a><span data-ttu-id="38e4c-112">权限</span><span class="sxs-lookup"><span data-stu-id="38e4c-112">Permissions</span></span>

<span data-ttu-id="38e4c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38e4c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38e4c-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="38e4c-115">Permission type</span></span>                        | <span data-ttu-id="38e4c-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="38e4c-116">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="38e4c-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38e4c-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="38e4c-118">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="38e4c-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="38e4c-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38e4c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38e4c-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="38e4c-120">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="38e4c-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="38e4c-121">Application</span></span>                            | <span data-ttu-id="38e4c-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="38e4c-122">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="38e4c-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38e4c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/assignments/
GET /education/users/{id}/assignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="38e4c-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="38e4c-124">Optional query parameters</span></span>

<span data-ttu-id="38e4c-125">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="38e4c-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38e4c-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="38e4c-126">Request headers</span></span>

| <span data-ttu-id="38e4c-127">标头</span><span class="sxs-lookup"><span data-stu-id="38e4c-127">Header</span></span>        | <span data-ttu-id="38e4c-128">值</span><span class="sxs-lookup"><span data-stu-id="38e4c-128">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="38e4c-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="38e4c-129">Authorization</span></span> | <span data-ttu-id="38e4c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="38e4c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38e4c-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="38e4c-132">Request body</span></span>

<span data-ttu-id="38e4c-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="38e4c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38e4c-134">响应</span><span class="sxs-lookup"><span data-stu-id="38e4c-134">Response</span></span>

<span data-ttu-id="38e4c-135">如果成功，此方法在响应`200 OK`正文中返回响应代码和[educationAssignment](../resources/educationassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="38e4c-135">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38e4c-136">示例</span><span class="sxs-lookup"><span data-stu-id="38e4c-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="38e4c-137">请求</span><span class="sxs-lookup"><span data-stu-id="38e4c-137">Request</span></span>
<span data-ttu-id="38e4c-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="38e4c-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http 
GET https://graph.microsoft.com/beta/education/me/assignments
```

##### <a name="response"></a><span data-ttu-id="38e4c-139">响应</span><span class="sxs-lookup"><span data-stu-id="38e4c-139">Response</span></span>

<span data-ttu-id="38e4c-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="38e4c-140">The following is an example of the response.</span></span> 

> <span data-ttu-id="38e4c-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="38e4c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>


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
      "assignDateTime": "2014-01-01T00:00:00Z",
      "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
      "assignedDateTime": "2014-01-01T00:00:00Z",
      "classId": "11010",
      "closeDateTime": "2014-01-11T00:00:00Z",
      "createdBy": {
        "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          }
      },
      "createdDateTime": "2014-01-01T00:00:00Z",
      "displayName": "Assignment 1",
      "dueDateTime": "2014-01-01T00:00:00Z",
      "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 100
      },
      "instructions": {
        "content": "Answer every question correctly",
        "contentType": "Text"
      },
      "lastModifiedBy": {
        "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          }
      },
      "lastModifiedDateTime": "2014-01-01T00:00:00Z",
      "status": "assigned"
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
