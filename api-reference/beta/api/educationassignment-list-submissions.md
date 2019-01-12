---
title: 列表提交
description: 列出与此工作分配关联的所有提交。 教师可以获取所有提交时学生可以仅都获取与其关联的提交。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2a4de863b69de420e89a9272e532fa889486fc22
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915184"
---
# <a name="list-submissions"></a><span data-ttu-id="f8c1a-104">列表提交</span><span class="sxs-lookup"><span data-stu-id="f8c1a-104">List submissions</span></span>

> <span data-ttu-id="f8c1a-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f8c1a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8c1a-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f8c1a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f8c1a-107">列出与此工作分配关联的所有提交。</span><span class="sxs-lookup"><span data-stu-id="f8c1a-107">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="f8c1a-108">教师可以获取所有提交时学生可以仅都获取与其关联的提交。</span><span class="sxs-lookup"><span data-stu-id="f8c1a-108">A teacher can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8c1a-109">权限</span><span class="sxs-lookup"><span data-stu-id="f8c1a-109">Permissions</span></span>
<span data-ttu-id="f8c1a-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8c1a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8c1a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8c1a-112">Permission type</span></span>      | <span data-ttu-id="f8c1a-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8c1a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8c1a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8c1a-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="f8c1a-115">EduAssignments.ReadBasic，EduAssignments.ReadWriteBasic，EduAssignments.Read EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8c1a-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f8c1a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8c1a-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f8c1a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8c1a-117">Not supported.</span></span>  |
|<span data-ttu-id="f8c1a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8c1a-118">Application</span></span> | <span data-ttu-id="f8c1a-119">不受支持。</span><span class="sxs-lookup"><span data-stu-id="f8c1a-119">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f8c1a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8c1a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f8c1a-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f8c1a-121">Optional query parameters</span></span>
<span data-ttu-id="f8c1a-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f8c1a-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8c1a-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8c1a-123">Request headers</span></span>
| <span data-ttu-id="f8c1a-124">标头</span><span class="sxs-lookup"><span data-stu-id="f8c1a-124">Header</span></span>       | <span data-ttu-id="f8c1a-125">值</span><span class="sxs-lookup"><span data-stu-id="f8c1a-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f8c1a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8c1a-126">Authorization</span></span>  | <span data-ttu-id="f8c1a-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8c1a-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f8c1a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8c1a-129">Request body</span></span>
<span data-ttu-id="f8c1a-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f8c1a-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f8c1a-131">响应</span><span class="sxs-lookup"><span data-stu-id="f8c1a-131">Response</span></span>
<span data-ttu-id="f8c1a-132">如果成功，此方法返回`200 OK`响应代码和响应正文中的[educationSubmission](../resources/educationsubmission.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="f8c1a-132">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f8c1a-133">示例</span><span class="sxs-lookup"><span data-stu-id="f8c1a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f8c1a-134">请求</span><span class="sxs-lookup"><span data-stu-id="f8c1a-134">Request</span></span>
<span data-ttu-id="f8c1a-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f8c1a-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
##### <a name="response"></a><span data-ttu-id="f8c1a-136">响应</span><span class="sxs-lookup"><span data-stu-id="f8c1a-136">Response</span></span>
<span data-ttu-id="f8c1a-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f8c1a-137">The following is an example of the response.</span></span> 

><span data-ttu-id="f8c1a-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f8c1a-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f8c1a-139">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f8c1a-139">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
  "value": [
    {
      "feedback": {
        "text": {
          "content": "Good work!",
          "contentType": "Text"
        },
        "feedbackDateTime": "2014-01-01T00:00:00Z",
        "feedbackBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
          "@odata.type": "microsoft.graph.identitySet"
        },
        "@odata.type": "microsoft.graph.educationFeedback"
        },
      "grade": {
         "gradedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
        "gradedDateTime": "2014-01-01T00:00:00Z"
      },
      "id": "33223",
      "recipient": {
        "userId": "13015",
        "@Odata.type":"microsoft.graph.educationSubmissionRecipient"
      },
      "releasedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
      "releasedDateTime": "2014-01-01T00:00:00Z",
      "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "status": "working",
      "submittedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
      "submittedDateTime": "2014-01-01T00:00:00Z"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List submissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
