---
title: 获取 educationAssignment
description: " 教师可以在课堂中查看所有作业。"
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 17cc7921c451fae534cd2bbe278ed89ce5e523af
ms.sourcegitcommit: 86d427ac670ebc3fdcf8e06541218bb74d39279d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2020
ms.locfileid: "49675861"
---
# <a name="get-educationassignment"></a><span data-ttu-id="38fab-103">获取 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="38fab-103">Get educationAssignment</span></span>

<span data-ttu-id="38fab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38fab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38fab-105">获取工作分配的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="38fab-105">Get the properties and relationships of an assignment.</span></span> <span data-ttu-id="38fab-106">学生只能看到分配给他们的作业;教师可以在课堂中查看所有作业。</span><span class="sxs-lookup"><span data-stu-id="38fab-106">Students can only see assignments assigned to them; teachers can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="38fab-107">权限</span><span class="sxs-lookup"><span data-stu-id="38fab-107">Permissions</span></span>
<span data-ttu-id="38fab-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38fab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="38fab-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="38fab-110">Permission type</span></span>      | <span data-ttu-id="38fab-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="38fab-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38fab-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38fab-112">Delegated (work or school account)</span></span> | <span data-ttu-id="38fab-113">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38fab-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="38fab-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38fab-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="38fab-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="38fab-115">Not supported.</span></span>  |
|<span data-ttu-id="38fab-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="38fab-116">Application</span></span> | <span data-ttu-id="38fab-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="38fab-117">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="38fab-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38fab-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="38fab-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="38fab-119">Optional query parameters</span></span>
<span data-ttu-id="38fab-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="38fab-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38fab-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="38fab-121">Request headers</span></span>
| <span data-ttu-id="38fab-122">标头</span><span class="sxs-lookup"><span data-stu-id="38fab-122">Header</span></span>       | <span data-ttu-id="38fab-123">值</span><span class="sxs-lookup"><span data-stu-id="38fab-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="38fab-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="38fab-124">Authorization</span></span>  | <span data-ttu-id="38fab-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="38fab-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="38fab-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="38fab-127">Request body</span></span>
<span data-ttu-id="38fab-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="38fab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38fab-129">响应</span><span class="sxs-lookup"><span data-stu-id="38fab-129">Response</span></span>
<span data-ttu-id="38fab-130">如果成功，此方法在响应 `200 OK` 正文中返回响应代码和 [educationAssignment](../resources/educationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="38fab-130">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="38fab-131">示例</span><span class="sxs-lookup"><span data-stu-id="38fab-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38fab-132">请求</span><span class="sxs-lookup"><span data-stu-id="38fab-132">Request</span></span>
<span data-ttu-id="38fab-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="38fab-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationassignment"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
##### <a name="response"></a><span data-ttu-id="38fab-134">响应</span><span class="sxs-lookup"><span data-stu-id="38fab-134">Response</span></span>
<span data-ttu-id="38fab-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="38fab-135">The following is an example of the response.</span></span> 

><span data-ttu-id="38fab-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="38fab-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "addedStudentAction": "none",
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
  "closeDateTime": "2014-01-11T00:00:00Z",
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
  "notificationChannelUrl": null,
  "status": "assigned"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->