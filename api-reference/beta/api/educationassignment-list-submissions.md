---
title: 列表提交
description: 列出与此工作分配相关联的所有提交。 教师可以获取所有提交, 而学生只能获取与之关联的提交。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8e01bb3960b3a8d29b48f3365fc8f2f61f4bb627
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324617"
---
# <a name="list-submissions"></a><span data-ttu-id="f1dc9-104">列表提交</span><span class="sxs-lookup"><span data-stu-id="f1dc9-104">List submissions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1dc9-105">列出与此工作分配相关联的所有提交。</span><span class="sxs-lookup"><span data-stu-id="f1dc9-105">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="f1dc9-106">教师可以获取所有提交, 而学生只能获取与之关联的提交。</span><span class="sxs-lookup"><span data-stu-id="f1dc9-106">A teacher can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1dc9-107">权限</span><span class="sxs-lookup"><span data-stu-id="f1dc9-107">Permissions</span></span>
<span data-ttu-id="f1dc9-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1dc9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1dc9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1dc9-110">Permission type</span></span>      | <span data-ttu-id="f1dc9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f1dc9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1dc9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1dc9-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="f1dc9-113">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="f1dc9-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f1dc9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1dc9-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f1dc9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1dc9-115">Not supported.</span></span>  |
|<span data-ttu-id="f1dc9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1dc9-116">Application</span></span> | <span data-ttu-id="f1dc9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1dc9-117">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f1dc9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1dc9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f1dc9-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f1dc9-119">Optional query parameters</span></span>
<span data-ttu-id="f1dc9-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f1dc9-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1dc9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1dc9-121">Request headers</span></span>
| <span data-ttu-id="f1dc9-122">标头</span><span class="sxs-lookup"><span data-stu-id="f1dc9-122">Header</span></span>       | <span data-ttu-id="f1dc9-123">值</span><span class="sxs-lookup"><span data-stu-id="f1dc9-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f1dc9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1dc9-124">Authorization</span></span>  | <span data-ttu-id="f1dc9-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f1dc9-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f1dc9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1dc9-127">Request body</span></span>
<span data-ttu-id="f1dc9-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f1dc9-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f1dc9-129">响应</span><span class="sxs-lookup"><span data-stu-id="f1dc9-129">Response</span></span>
<span data-ttu-id="f1dc9-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationSubmission](../resources/educationsubmission.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="f1dc9-130">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f1dc9-131">示例</span><span class="sxs-lookup"><span data-stu-id="f1dc9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1dc9-132">请求</span><span class="sxs-lookup"><span data-stu-id="f1dc9-132">Request</span></span>
<span data-ttu-id="f1dc9-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f1dc9-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
##### <a name="response"></a><span data-ttu-id="f1dc9-134">响应</span><span class="sxs-lookup"><span data-stu-id="f1dc9-134">Response</span></span>
<span data-ttu-id="f1dc9-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f1dc9-135">The following is an example of the response.</span></span> 

><span data-ttu-id="f1dc9-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f1dc9-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f1dc9-137">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f1dc9-137">All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List submissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
