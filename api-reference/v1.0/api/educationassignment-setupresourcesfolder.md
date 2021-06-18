---
title: educationAssignment： setUpResourcesFolder
description: 创建一SharePoint文件夹以上传给定 educationAssignment 的文件。
localization_priority: Normal
author: sharmas
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: bde62e08376c7fa2e4bcc151da6e6d5d0438aa84
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993167"
---
# <a name="educationassignment-setupresourcesfolder"></a><span data-ttu-id="0c687-103">educationAssignment： setUpResourcesFolder</span><span class="sxs-lookup"><span data-stu-id="0c687-103">educationAssignment: setUpResourcesFolder</span></span>

<span data-ttu-id="0c687-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c687-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0c687-105">创建一SharePoint文件夹，以上传给定[educationAssignment 的文件](../resources/educationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="0c687-105">Create a SharePoint folder to upload files for a given [educationAssignment](../resources/educationassignment.md).</span></span> 

<span data-ttu-id="0c687-106">教师确定要上载到作业文件夹中的资源。</span><span class="sxs-lookup"><span data-stu-id="0c687-106">The teacher determines the resources to upload in the assignment's folder.</span></span> 

## <a name="permissions"></a><span data-ttu-id="0c687-107">权限</span><span class="sxs-lookup"><span data-stu-id="0c687-107">Permissions</span></span>
<span data-ttu-id="0c687-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c687-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c687-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c687-110">Permission type</span></span>      | <span data-ttu-id="0c687-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0c687-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c687-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c687-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="0c687-113">EduAssignments.ReadBasic、EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="0c687-113">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="0c687-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c687-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0c687-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c687-115">Not supported.</span></span>  |
|<span data-ttu-id="0c687-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c687-116">Application</span></span> | <span data-ttu-id="0c687-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c687-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0c687-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c687-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/setUpResourcesFolder
```
## <a name="request-headers"></a><span data-ttu-id="0c687-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c687-119">Request headers</span></span>
| <span data-ttu-id="0c687-120">标头</span><span class="sxs-lookup"><span data-stu-id="0c687-120">Header</span></span>       | <span data-ttu-id="0c687-121">值</span><span class="sxs-lookup"><span data-stu-id="0c687-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0c687-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c687-122">Authorization</span></span>  | <span data-ttu-id="0c687-p102">持有者 `{token}`。必需。</span><span class="sxs-lookup"><span data-stu-id="0c687-p102">Bearer `{token}`. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0c687-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c687-125">Request body</span></span>
<span data-ttu-id="0c687-126">你需要提供一个空 json `{}` 作为此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0c687-126">You need to provide an empty json `{}` as request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0c687-127">响应</span><span class="sxs-lookup"><span data-stu-id="0c687-127">Response</span></span>
<span data-ttu-id="0c687-128">如果成功，此方法在请求正文中返回 200 Ok 响应代码和 [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) 对象。</span><span class="sxs-lookup"><span data-stu-id="0c687-128">If successful, this method returns a 200 Ok response code and [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) object in the request body.</span></span>

## <a name="example"></a><span data-ttu-id="0c687-129">示例</span><span class="sxs-lookup"><span data-stu-id="0c687-129">Example</span></span>
<span data-ttu-id="0c687-130">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="0c687-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="0c687-131">请求</span><span class="sxs-lookup"><span data-stu-id="0c687-131">Request</span></span>
<span data-ttu-id="0c687-132">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="0c687-132">The following is an example of a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0c687-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c687-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["ad8afb28-c138-4ad7-b7f5-a6986c2655a8"],
  "name": "educationassignment_setupresourcesfolder"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/education/classes/d38ffdea-da93-46ac-90ba-d568c6073075/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/setUpResourcesFolder
Content-type: application/json

{
}
```
# <a name="c"></a>[<span data-ttu-id="0c687-134">C#</span><span class="sxs-lookup"><span data-stu-id="0c687-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-setupresourcesfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0c687-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c687-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-setupresourcesfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0c687-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c687-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-setupresourcesfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0c687-137">Java</span><span class="sxs-lookup"><span data-stu-id="0c687-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationassignment-setupresourcesfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0c687-138">响应</span><span class="sxs-lookup"><span data-stu-id="0c687-138">Response</span></span>
<span data-ttu-id="0c687-139">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="0c687-139">The following is an example of a response.</span></span> 

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

