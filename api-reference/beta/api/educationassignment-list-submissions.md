---
title: 列出提交
description: 列出与此分配关联的所有提交。 教师或具有应用程序权限的应用程序可以获取所有提交，而学生只能获取与其关联的提交。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c27472d82521c1972b468ebef7925e194efbae7f
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961287"
---
# <a name="list-submissions"></a><span data-ttu-id="596e2-104">列出提交</span><span class="sxs-lookup"><span data-stu-id="596e2-104">List submissions</span></span>

<span data-ttu-id="596e2-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="596e2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="596e2-106">列出与此分配关联的所有提交。</span><span class="sxs-lookup"><span data-stu-id="596e2-106">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="596e2-107">教师或具有应用程序权限的应用程序可以获取所有提交，而学生只能获取与其关联的提交。</span><span class="sxs-lookup"><span data-stu-id="596e2-107">A teacher or an application with application permissions can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="596e2-108">权限</span><span class="sxs-lookup"><span data-stu-id="596e2-108">Permissions</span></span>
<span data-ttu-id="596e2-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="596e2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="596e2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="596e2-111">Permission type</span></span>      | <span data-ttu-id="596e2-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="596e2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="596e2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="596e2-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="596e2-114">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="596e2-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="596e2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="596e2-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="596e2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="596e2-116">Not supported.</span></span>  |
|<span data-ttu-id="596e2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="596e2-117">Application</span></span> | <span data-ttu-id="596e2-118">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="596e2-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="596e2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="596e2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="596e2-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="596e2-120">Optional query parameters</span></span>
<span data-ttu-id="596e2-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="596e2-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="596e2-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="596e2-122">Request headers</span></span>
| <span data-ttu-id="596e2-123">标头</span><span class="sxs-lookup"><span data-stu-id="596e2-123">Header</span></span>       | <span data-ttu-id="596e2-124">值</span><span class="sxs-lookup"><span data-stu-id="596e2-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="596e2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="596e2-125">Authorization</span></span>  | <span data-ttu-id="596e2-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="596e2-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="596e2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="596e2-128">Request body</span></span>
<span data-ttu-id="596e2-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="596e2-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="596e2-130">响应</span><span class="sxs-lookup"><span data-stu-id="596e2-130">Response</span></span>
<span data-ttu-id="596e2-131">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码 [和 educationSubmission](../resources/educationsubmission.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="596e2-131">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="596e2-132">示例</span><span class="sxs-lookup"><span data-stu-id="596e2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="596e2-133">请求</span><span class="sxs-lookup"><span data-stu-id="596e2-133">Request</span></span>
<span data-ttu-id="596e2-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="596e2-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="596e2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="596e2-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_submissions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
# <a name="c"></a>[<span data-ttu-id="596e2-136">C#</span><span class="sxs-lookup"><span data-stu-id="596e2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-submissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="596e2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="596e2-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-submissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="596e2-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="596e2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-submissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="596e2-139">Java</span><span class="sxs-lookup"><span data-stu-id="596e2-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-submissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="596e2-140">响应</span><span class="sxs-lookup"><span data-stu-id="596e2-140">Response</span></span>
<span data-ttu-id="596e2-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="596e2-141">The following is an example of the response.</span></span> 

><span data-ttu-id="596e2-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="596e2-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="596e2-143">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="596e2-143">All of the properties will be returned from an actual call.</span></span>

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
