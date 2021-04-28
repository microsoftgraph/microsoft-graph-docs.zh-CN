---
title: 列出提交
description: 列出与此分配关联的所有提交。 教师或具有应用程序权限的应用程序可以获取所有提交，而学生只能获取与其关联的提交。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7cbe965cde21b358eaa21adbdd994bb88070fbfc
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061670"
---
# <a name="list-submissions"></a><span data-ttu-id="fb872-104">列出提交</span><span class="sxs-lookup"><span data-stu-id="fb872-104">List submissions</span></span>

<span data-ttu-id="fb872-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb872-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb872-106">列出与此分配关联的所有提交。</span><span class="sxs-lookup"><span data-stu-id="fb872-106">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="fb872-107">教师或具有应用程序权限的应用程序可以获取所有提交，而学生只能获取与其关联的提交。</span><span class="sxs-lookup"><span data-stu-id="fb872-107">A teacher or an application with application permissions can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb872-108">权限</span><span class="sxs-lookup"><span data-stu-id="fb872-108">Permissions</span></span>
<span data-ttu-id="fb872-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb872-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb872-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb872-111">Permission type</span></span>      | <span data-ttu-id="fb872-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb872-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb872-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb872-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="fb872-114">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb872-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="fb872-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb872-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fb872-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb872-116">Not supported.</span></span>  |
|<span data-ttu-id="fb872-117">Application\*</span><span class="sxs-lookup"><span data-stu-id="fb872-117">Application\*</span></span> | <span data-ttu-id="fb872-118">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb872-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

<span data-ttu-id="fb872-119">\*应用程序权限当前仅适用于个人预览版客户。</span><span class="sxs-lookup"><span data-stu-id="fb872-119">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="fb872-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb872-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fb872-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fb872-121">Optional query parameters</span></span>
<span data-ttu-id="fb872-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fb872-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb872-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb872-123">Request headers</span></span>
| <span data-ttu-id="fb872-124">标头</span><span class="sxs-lookup"><span data-stu-id="fb872-124">Header</span></span>       | <span data-ttu-id="fb872-125">值</span><span class="sxs-lookup"><span data-stu-id="fb872-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fb872-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb872-126">Authorization</span></span>  | <span data-ttu-id="fb872-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fb872-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fb872-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb872-129">Request body</span></span>
<span data-ttu-id="fb872-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fb872-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fb872-131">响应</span><span class="sxs-lookup"><span data-stu-id="fb872-131">Response</span></span>
<span data-ttu-id="fb872-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码 [和 educationSubmission](../resources/educationsubmission.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fb872-132">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fb872-133">示例</span><span class="sxs-lookup"><span data-stu-id="fb872-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb872-134">请求</span><span class="sxs-lookup"><span data-stu-id="fb872-134">Request</span></span>
<span data-ttu-id="fb872-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fb872-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fb872-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb872-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_submissions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
# <a name="c"></a>[<span data-ttu-id="fb872-137">C#</span><span class="sxs-lookup"><span data-stu-id="fb872-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-submissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb872-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb872-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-submissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb872-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb872-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-submissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb872-140">Java</span><span class="sxs-lookup"><span data-stu-id="fb872-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-submissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fb872-141">响应</span><span class="sxs-lookup"><span data-stu-id="fb872-141">Response</span></span>
<span data-ttu-id="fb872-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fb872-142">The following is an example of the response.</span></span> 

><span data-ttu-id="fb872-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fb872-143">**Note:** The response object shown here might be shortened for readability.</span></span>

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
