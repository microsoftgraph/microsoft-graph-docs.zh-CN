---
title: educationAssignment： setUpResourcesFolder
description: 创建一SharePoint文件夹以上传给定 educationAssignment 的文件。
localization_priority: Normal
author: sharmas
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 32a69da6e1c03119c13114900c7e12563e504950
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629699"
---
# <a name="educationassignment-setupresourcesfolder"></a><span data-ttu-id="802f2-103">educationAssignment： setUpResourcesFolder</span><span class="sxs-lookup"><span data-stu-id="802f2-103">educationAssignment: setUpResourcesFolder</span></span>

<span data-ttu-id="802f2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="802f2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="802f2-105">创建一SharePoint文件夹，以上传给定[educationAssignment 的文件](../resources/educationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="802f2-105">Create a SharePoint folder to upload files for a given [educationAssignment](../resources/educationassignment.md).</span></span> 

<span data-ttu-id="802f2-106">教师确定要上载到作业文件夹中的资源。</span><span class="sxs-lookup"><span data-stu-id="802f2-106">The teacher determines the resources to upload in the assignment's folder.</span></span> 

## <a name="permissions"></a><span data-ttu-id="802f2-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="802f2-107">Permissions</span></span>
<span data-ttu-id="802f2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="802f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="802f2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="802f2-110">Permission type</span></span>      | <span data-ttu-id="802f2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="802f2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="802f2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="802f2-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="802f2-113">EduAssignments.ReadBasic、EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="802f2-113">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="802f2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="802f2-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="802f2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="802f2-115">Not supported.</span></span>  |
|<span data-ttu-id="802f2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="802f2-116">Application</span></span> | <span data-ttu-id="802f2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="802f2-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="802f2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="802f2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/setUpResourcesFolder

```
## <a name="request-headers"></a><span data-ttu-id="802f2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="802f2-119">Request headers</span></span>
| <span data-ttu-id="802f2-120">标头</span><span class="sxs-lookup"><span data-stu-id="802f2-120">Header</span></span>       | <span data-ttu-id="802f2-121">值</span><span class="sxs-lookup"><span data-stu-id="802f2-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="802f2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="802f2-122">Authorization</span></span>  | <span data-ttu-id="802f2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="802f2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="802f2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="802f2-125">Request body</span></span>
<span data-ttu-id="802f2-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="802f2-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="802f2-127">响应</span><span class="sxs-lookup"><span data-stu-id="802f2-127">Response</span></span>
<span data-ttu-id="802f2-128">如果成功，此方法在请求正文中返回 200 Ok 响应代码和 [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) 对象。</span><span class="sxs-lookup"><span data-stu-id="802f2-128">If successful, this method returns a 200 Ok response code and [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) object in the request body.</span></span>

## <a name="example"></a><span data-ttu-id="802f2-129">示例</span><span class="sxs-lookup"><span data-stu-id="802f2-129">Example</span></span>
<span data-ttu-id="802f2-130">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="802f2-130">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="802f2-131">请求</span><span class="sxs-lookup"><span data-stu-id="802f2-131">Request</span></span>
<span data-ttu-id="802f2-132">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="802f2-132">The following is an example of a request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationassignment_setupresourcesfolder"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/setUpResourcesFolder
```
---

### <a name="response"></a><span data-ttu-id="802f2-133">响应</span><span class="sxs-lookup"><span data-stu-id="802f2-133">Response</span></span>
<span data-ttu-id="802f2-134">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="802f2-134">The following is an example of a response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('955e0bd5-52c2-41ad-b7e8-5b33a18c5e78')/assignments/$entity",
    "classId": "955e0bd5-52c2-41ad-b7e8-5b33a18c5e78",
    "displayName": "Unit 3 Essay",
    "closeDateTime": "2021-04-06T00:00:00Z",
    "dueDateTime": "2021-04-05T00:00:00Z",
    "assignDateTime": "2021-04-01T00:00:00Z",
    "assignedDateTime": null,
    "allowLateSubmissions": true,
    "createdDateTime": "2021-03-04T00:02:31.9834674Z",
    "lastModifiedDateTime": "2021-03-04T00:02:32.0954032Z",
    "allowStudentsToAddResourcesToSubmission": true,
    "status": "draft",
    "notificationChannelUrl": null,
    "addedStudentAction": "assignIfOpen",
    "addToCalendarAction": "studentsAndTeamOwners",
    "id": "18d17255-3278-49fb-8da7-d095b7f610c4",
    "instructions": {
        "content": "Upload a 500 word essay about the theme of nature in a Shakespearean sonnet.",
        "contentType": "text"
    },
    "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 100
    },
    "assignTo": {
        "@odata.type": "#microsoft.graph.educationAssignmentIndividualRecipient",
        "recipients": [
            "42ff222c-571f-497c-a9d3-f77ea9ece327"
        ]
    },
    "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!H0Unq6KJREmMLHgbJXfKw4YTuh2luKRDvUVGQBLOmvaRxxvbedZKT4LKslSIjT9a/items/01SMYGQ3IUCDNLBJ4XCFE3AQMQHTLSLVYX",
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "42ff222c-571f-497c-a9d3-f77ea9ece327",
            "displayName": null
        }
    },
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "42ff222c-571f-497c-a9d3-f77ea9ece327",
            "displayName": null
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

