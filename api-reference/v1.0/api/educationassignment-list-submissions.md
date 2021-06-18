---
title: 列出提交
description: 列出与工作分配关联的所有提交。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 86647daa0d19555f53c8f0969cdd831ebd9e7e39
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992755"
---
# <a name="list-submissions"></a><span data-ttu-id="107a9-103">列出提交</span><span class="sxs-lookup"><span data-stu-id="107a9-103">List submissions</span></span>

<span data-ttu-id="107a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="107a9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="107a9-105">列出与工作分配关联的所有提交。</span><span class="sxs-lookup"><span data-stu-id="107a9-105">List all the submissions associated with an assignment.</span></span> 

<span data-ttu-id="107a9-106">教师或具有应用程序权限的应用程序可以获取所有提交，而学生只能获取与其关联的提交。</span><span class="sxs-lookup"><span data-stu-id="107a9-106">A teacher or an application with application permissions can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="107a9-107">权限</span><span class="sxs-lookup"><span data-stu-id="107a9-107">Permissions</span></span>
<span data-ttu-id="107a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="107a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="107a9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="107a9-110">Permission type</span></span>      | <span data-ttu-id="107a9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="107a9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="107a9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="107a9-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="107a9-113">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="107a9-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="107a9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="107a9-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="107a9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="107a9-115">Not supported.</span></span>  |
|<span data-ttu-id="107a9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="107a9-116">Application</span></span> | <span data-ttu-id="107a9-117">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="107a9-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="107a9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="107a9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="107a9-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="107a9-119">Optional query parameters</span></span>
<span data-ttu-id="107a9-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="107a9-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="107a9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="107a9-121">Request headers</span></span>
| <span data-ttu-id="107a9-122">标头</span><span class="sxs-lookup"><span data-stu-id="107a9-122">Header</span></span>       | <span data-ttu-id="107a9-123">值</span><span class="sxs-lookup"><span data-stu-id="107a9-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="107a9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="107a9-124">Authorization</span></span>  | <span data-ttu-id="107a9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="107a9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="107a9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="107a9-127">Request body</span></span>
<span data-ttu-id="107a9-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="107a9-128">Don't supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="107a9-129">响应</span><span class="sxs-lookup"><span data-stu-id="107a9-129">Response</span></span>
<span data-ttu-id="107a9-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码 [和 educationSubmission](../resources/educationsubmission.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="107a9-130">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="107a9-131">示例</span><span class="sxs-lookup"><span data-stu-id="107a9-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="107a9-132">请求</span><span class="sxs-lookup"><span data-stu-id="107a9-132">Request</span></span>
<span data-ttu-id="107a9-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="107a9-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="107a9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="107a9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["ad8afb28-c138-4ad7-b7f5-a6986c2655a8"],
  "name": "get_submissions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions
```
# <a name="c"></a>[<span data-ttu-id="107a9-135">C#</span><span class="sxs-lookup"><span data-stu-id="107a9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-submissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="107a9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="107a9-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-submissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="107a9-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="107a9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-submissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="107a9-138">Java</span><span class="sxs-lookup"><span data-stu-id="107a9-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-submissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="107a9-139">响应</span><span class="sxs-lookup"><span data-stu-id="107a9-139">Response</span></span>
<span data-ttu-id="107a9-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="107a9-140">The following is an example of the response.</span></span> 

><span data-ttu-id="107a9-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="107a9-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
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
      "id": "33223",
      "recipient": {
        "userId": "13015",
        "@Odata.type":"microsoft.graph.educationSubmissionRecipient"
      },
      "releasedBy": {
          "user": {
            "displayName": "Shawn Hughes",
            "id": "14012"
          },
        },
      "releasedDateTime": "2014-01-01T00:00:00Z",
      "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "status": "working",
      "submittedBy": {
          "user": {
            "displayName": "Shawn Hughes",
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
