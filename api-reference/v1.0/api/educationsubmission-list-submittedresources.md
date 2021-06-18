---
title: 列出 submittedResources
description: 列出已正式提交进行评分的资源。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2fc647442d302bfd38705725374e8933dc9e0702
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993440"
---
# <a name="list-submittedresources"></a><span data-ttu-id="3093c-103">列出 submittedResources</span><span class="sxs-lookup"><span data-stu-id="3093c-103">List submittedResources</span></span>

<span data-ttu-id="3093c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3093c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3093c-105">列出已正式提交进行评分的资源。</span><span class="sxs-lookup"><span data-stu-id="3093c-105">List the resources that have officially been submitted for grading.</span></span> 

<span data-ttu-id="3093c-106">拥有提交的学生如果不重新提交作业，则无法更改提交的列表。</span><span class="sxs-lookup"><span data-stu-id="3093c-106">The student who owns the submission cannot change the submitted list without resubmitting the assignment.</span></span> <span data-ttu-id="3093c-107">这是实际资源的包装器，如果此资源是从工作分配复制的，则可以包含一个返回实际工作分配资源的指针。</span><span class="sxs-lookup"><span data-stu-id="3093c-107">This is a wrapper around the real resource and can contain a pointer back to the actual assignment resource if this resource was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="3093c-108">权限</span><span class="sxs-lookup"><span data-stu-id="3093c-108">Permissions</span></span>
<span data-ttu-id="3093c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3093c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3093c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3093c-111">Permission type</span></span>      | <span data-ttu-id="3093c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3093c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3093c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3093c-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="3093c-114">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3093c-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="3093c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3093c-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3093c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3093c-116">Not supported.</span></span>  |
|<span data-ttu-id="3093c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3093c-117">Application</span></span> | <span data-ttu-id="3093c-118">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3093c-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3093c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3093c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3093c-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3093c-120">Optional query parameters</span></span>
<span data-ttu-id="3093c-121">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3093c-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3093c-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="3093c-122">Request headers</span></span>
| <span data-ttu-id="3093c-123">标头</span><span class="sxs-lookup"><span data-stu-id="3093c-123">Header</span></span>       | <span data-ttu-id="3093c-124">值</span><span class="sxs-lookup"><span data-stu-id="3093c-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3093c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3093c-125">Authorization</span></span>  | <span data-ttu-id="3093c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3093c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3093c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="3093c-128">Request body</span></span>
<span data-ttu-id="3093c-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3093c-129">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3093c-130">响应</span><span class="sxs-lookup"><span data-stu-id="3093c-130">Response</span></span>
<span data-ttu-id="3093c-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [educationSubmissionResource](../resources/educationsubmissionresource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3093c-131">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3093c-132">示例</span><span class="sxs-lookup"><span data-stu-id="3093c-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="3093c-133">请求</span><span class="sxs-lookup"><span data-stu-id="3093c-133">Request</span></span>
<span data-ttu-id="3093c-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3093c-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3093c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3093c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_submittedresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/submittedResources
```
# <a name="c"></a>[<span data-ttu-id="3093c-136">C#</span><span class="sxs-lookup"><span data-stu-id="3093c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-submittedresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3093c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3093c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-submittedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3093c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3093c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-submittedresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3093c-139">Java</span><span class="sxs-lookup"><span data-stu-id="3093c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-submittedresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="3093c-140">响应</span><span class="sxs-lookup"><span data-stu-id="3093c-140">Response</span></span>
<span data-ttu-id="3093c-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3093c-141">The following is an example of the response.</span></span> 

><span data-ttu-id="3093c-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3093c-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1045

{
  "value": [
    {
        "assignmentResourceUrl": null,
        "id": "0f7dd681-f1b6-4f78-b8fb-a579fc4a36ae",
        "resource": {
            "@odata.type": "#microsoft.graph.educationLinkResource",
            "displayName": "ABC",
            "createdDateTime": "2021-03-11T20:47:53.0823323Z",
            "lastModifiedDateTime": "2021-03-11T20:47:53.0823323Z",
            "link": "https://www.bing.com/",
            "createdBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f8bbb2a4-2cdd-4d49-ac81-d4113fc72dc1",
                    "displayName": null
                }
            },
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f8bbb2a4-2cdd-4d49-ac81-d4113fc72dc1",
                    "displayName": null
                }
            }
        }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List submittedResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
