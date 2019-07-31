---
title: 列出作业
description: 检索工作分配对象的列表。 允许教师查看该类的所有工作分配对象。 学生只能查看分配给他们的工作分配。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a7b201dcafa69fa17650b0d4154ad558d0a78c96
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955437"
---
# <a name="list-assignments"></a><span data-ttu-id="64ddc-105">列出作业</span><span class="sxs-lookup"><span data-stu-id="64ddc-105">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64ddc-106">检索工作分配对象的列表。</span><span class="sxs-lookup"><span data-stu-id="64ddc-106">Retrieve a list of assignment objects.</span></span> <span data-ttu-id="64ddc-107">允许教师查看该类的所有工作分配对象。</span><span class="sxs-lookup"><span data-stu-id="64ddc-107">A teacher is allowed to see all assignment objects for the class.</span></span> <span data-ttu-id="64ddc-108">学生只能查看分配给他们的工作分配。</span><span class="sxs-lookup"><span data-stu-id="64ddc-108">Students can only see assignments that are assigned to them.</span></span>

## <a name="permissions"></a><span data-ttu-id="64ddc-109">权限</span><span class="sxs-lookup"><span data-stu-id="64ddc-109">Permissions</span></span>

<span data-ttu-id="64ddc-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64ddc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="64ddc-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="64ddc-112">Permission type</span></span>                        | <span data-ttu-id="64ddc-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="64ddc-113">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="64ddc-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64ddc-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="64ddc-115">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="64ddc-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="64ddc-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64ddc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64ddc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="64ddc-117">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="64ddc-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="64ddc-118">Application</span></span>                            | <span data-ttu-id="64ddc-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="64ddc-119">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="64ddc-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64ddc-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64ddc-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="64ddc-121">Optional query parameters</span></span>
<span data-ttu-id="64ddc-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="64ddc-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64ddc-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="64ddc-123">Request headers</span></span>

| <span data-ttu-id="64ddc-124">标头</span><span class="sxs-lookup"><span data-stu-id="64ddc-124">Header</span></span>        | <span data-ttu-id="64ddc-125">值</span><span class="sxs-lookup"><span data-stu-id="64ddc-125">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="64ddc-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="64ddc-126">Authorization</span></span> | <span data-ttu-id="64ddc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="64ddc-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64ddc-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="64ddc-129">Request body</span></span>

<span data-ttu-id="64ddc-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="64ddc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64ddc-131">响应</span><span class="sxs-lookup"><span data-stu-id="64ddc-131">Response</span></span>

<span data-ttu-id="64ddc-132">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationAssignment](../resources/educationassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="64ddc-132">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64ddc-133">示例</span><span class="sxs-lookup"><span data-stu-id="64ddc-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="64ddc-134">请求</span><span class="sxs-lookup"><span data-stu-id="64ddc-134">Request</span></span>

<span data-ttu-id="64ddc-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="64ddc-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignments
```

##### <a name="response"></a><span data-ttu-id="64ddc-136">响应</span><span class="sxs-lookup"><span data-stu-id="64ddc-136">Response</span></span>

<span data-ttu-id="64ddc-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="64ddc-137">The following is an example of the response.</span></span> 

><span data-ttu-id="64ddc-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="64ddc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
