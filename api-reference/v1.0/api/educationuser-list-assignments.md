---
title: 列出用户的分配
description: 获取分配给用户的所有课程的工作分配列表。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4d64a865bf6554cfb9c1a7e2abea812e6ba0b8e4
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912283"
---
# <a name="list-assignments-of-a-user"></a><span data-ttu-id="d263a-103">列出用户的分配</span><span class="sxs-lookup"><span data-stu-id="d263a-103">List assignments of a user</span></span>

<span data-ttu-id="d263a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d263a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d263a-105">获取分配给用户的所有课程的工作分配列表。</span><span class="sxs-lookup"><span data-stu-id="d263a-105">Get a list of assignments assigned to a user for all classes.</span></span> 

<span data-ttu-id="d263a-106">此实用工具命名空间允许呼叫者在一次呼叫中查找学生的所有作业，而不必从每个班级请求作业。</span><span class="sxs-lookup"><span data-stu-id="d263a-106">This utility namespace allows a caller to find all a student's assignments in a single call rather than having to request assignments from each class.</span></span> <span data-ttu-id="d263a-107">工作分配列表包含从类命名空间内获取工作分配的详细信息所需的内容。</span><span class="sxs-lookup"><span data-stu-id="d263a-107">The assignment list contains what is needed to get the detailed information for the assignment from within the class namespace.</span></span> <span data-ttu-id="d263a-108">对分配执行的其他所有操作都应使用类命名空间。</span><span class="sxs-lookup"><span data-stu-id="d263a-108">All other operations on the assignment should use the class namespace.</span></span>

## <a name="permissions"></a><span data-ttu-id="d263a-109">权限</span><span class="sxs-lookup"><span data-stu-id="d263a-109">Permissions</span></span>

<span data-ttu-id="d263a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d263a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d263a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="d263a-112">Permission type</span></span>                        | <span data-ttu-id="d263a-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d263a-113">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d263a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d263a-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="d263a-115">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d263a-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="d263a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d263a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d263a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d263a-117">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="d263a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="d263a-118">Application</span></span>                            | <span data-ttu-id="d263a-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d263a-119">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="d263a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d263a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users/{id}/assignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d263a-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d263a-121">Optional query parameters</span></span>

<span data-ttu-id="d263a-122">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d263a-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d263a-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="d263a-123">Request headers</span></span>

| <span data-ttu-id="d263a-124">标头</span><span class="sxs-lookup"><span data-stu-id="d263a-124">Header</span></span>        | <span data-ttu-id="d263a-125">值</span><span class="sxs-lookup"><span data-stu-id="d263a-125">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="d263a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d263a-126">Authorization</span></span> | <span data-ttu-id="d263a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d263a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d263a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d263a-129">Request body</span></span>

<span data-ttu-id="d263a-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d263a-130">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d263a-131">响应</span><span class="sxs-lookup"><span data-stu-id="d263a-131">Response</span></span>

<span data-ttu-id="d263a-132">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [educationAssignment](../resources/educationassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d263a-132">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d263a-133">示例</span><span class="sxs-lookup"><span data-stu-id="d263a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d263a-134">请求</span><span class="sxs-lookup"><span data-stu-id="d263a-134">Request</span></span>
<span data-ttu-id="d263a-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d263a-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_me_assignments"
}-->

```http 
GET https://graph.microsoft.com/v1.0/education/me/assignments
```

### <a name="response"></a><span data-ttu-id="d263a-136">响应</span><span class="sxs-lookup"><span data-stu-id="d263a-136">Response</span></span>

<span data-ttu-id="d263a-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d263a-137">The following is an example of the response.</span></span> 

> <span data-ttu-id="d263a-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d263a-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "allowLateSubmissions": true,
      "allowStudentsToAddResourcesToSubmission": true,
      "assignDateTime": "2014-01-01T00:00:00Z",
      "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
      "assignedDateTime": "2014-01-01T00:00:00Z",
      "classId": "11010",
      "closeDateTime": "2014-01-11T00:00:00Z",
      "createdBy": {
        "user": {
            "displayName": "Shawn Hughes",
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
            "displayName": "Shawn Hughes",
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
