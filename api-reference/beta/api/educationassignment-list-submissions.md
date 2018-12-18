---
title: 列表提交
description: 列出与此工作分配关联的所有提交。 教师可以获取所有提交时学生可以仅都获取与其关联的提交。
author: dipakboyed
ms.openlocfilehash: ac7bd47b4cbc4549f38239c4a68504bd20b3a2e8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308426"
---
# <a name="list-submissions"></a><span data-ttu-id="5a0a8-104">列表提交</span><span class="sxs-lookup"><span data-stu-id="5a0a8-104">List submissions</span></span>

> <span data-ttu-id="5a0a8-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5a0a8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a0a8-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5a0a8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a0a8-107">列出与此工作分配关联的所有提交。</span><span class="sxs-lookup"><span data-stu-id="5a0a8-107">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="5a0a8-108">教师可以获取所有提交时学生可以仅都获取与其关联的提交。</span><span class="sxs-lookup"><span data-stu-id="5a0a8-108">A teacher can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a0a8-109">权限</span><span class="sxs-lookup"><span data-stu-id="5a0a8-109">Permissions</span></span>
<span data-ttu-id="5a0a8-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a0a8-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a0a8-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a0a8-112">Permission type</span></span>      | <span data-ttu-id="5a0a8-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5a0a8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a0a8-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a0a8-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="5a0a8-115">EduAssignments.ReadBasic，EduAssignments.ReadWriteBasic，EduAssignments.Read EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a0a8-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="5a0a8-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a0a8-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5a0a8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a0a8-117">Not supported.</span></span>  |
|<span data-ttu-id="5a0a8-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a0a8-118">Application</span></span> | <span data-ttu-id="5a0a8-119">不受支持。</span><span class="sxs-lookup"><span data-stu-id="5a0a8-119">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5a0a8-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a0a8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5a0a8-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5a0a8-121">Optional query parameters</span></span>
<span data-ttu-id="5a0a8-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5a0a8-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a0a8-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a0a8-123">Request headers</span></span>
| <span data-ttu-id="5a0a8-124">标头</span><span class="sxs-lookup"><span data-stu-id="5a0a8-124">Header</span></span>       | <span data-ttu-id="5a0a8-125">值</span><span class="sxs-lookup"><span data-stu-id="5a0a8-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5a0a8-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a0a8-126">Authorization</span></span>  | <span data-ttu-id="5a0a8-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5a0a8-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5a0a8-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a0a8-129">Request body</span></span>
<span data-ttu-id="5a0a8-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5a0a8-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5a0a8-131">响应</span><span class="sxs-lookup"><span data-stu-id="5a0a8-131">Response</span></span>
<span data-ttu-id="5a0a8-132">如果成功，此方法返回`200 OK`响应代码和响应正文中的[educationSubmission](../resources/educationsubmission.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="5a0a8-132">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5a0a8-133">示例</span><span class="sxs-lookup"><span data-stu-id="5a0a8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a0a8-134">请求</span><span class="sxs-lookup"><span data-stu-id="5a0a8-134">Request</span></span>
<span data-ttu-id="5a0a8-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5a0a8-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
##### <a name="response"></a><span data-ttu-id="5a0a8-136">响应</span><span class="sxs-lookup"><span data-stu-id="5a0a8-136">Response</span></span>
<span data-ttu-id="5a0a8-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5a0a8-137">The following is an example of the response.</span></span> 

><span data-ttu-id="5a0a8-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5a0a8-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5a0a8-139">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5a0a8-139">All of the properties will be returned from an actual call.</span></span>

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