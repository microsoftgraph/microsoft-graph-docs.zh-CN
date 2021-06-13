---
title: 列出提交资源
description: 列出与提交关联的资源。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 174f9fa606ab9f4a4bdc85fb60dd1e4f75d7ae39
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911800"
---
# <a name="list-submission-resources"></a><span data-ttu-id="9ec83-103">列出提交资源</span><span class="sxs-lookup"><span data-stu-id="9ec83-103">List submission resources</span></span>

<span data-ttu-id="9ec83-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ec83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ec83-105">列出与提交关联的资源。</span><span class="sxs-lookup"><span data-stu-id="9ec83-105">List the resources associated with a submission.</span></span> 

<span data-ttu-id="9ec83-106">**submissionResource** 对象是学生正在处理的实际资源对象的包装。</span><span class="sxs-lookup"><span data-stu-id="9ec83-106">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="9ec83-107">如果资源是在分配过程中从分配复制的，包装器还包括指向分配上的资源的指针。</span><span class="sxs-lookup"><span data-stu-id="9ec83-107">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="9ec83-108">这些资源是工作分配的工作副本。</span><span class="sxs-lookup"><span data-stu-id="9ec83-108">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="9ec83-109">**submittedResources** 是已正式提交进行评分的资源。</span><span class="sxs-lookup"><span data-stu-id="9ec83-109">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ec83-110">权限</span><span class="sxs-lookup"><span data-stu-id="9ec83-110">Permissions</span></span>

<span data-ttu-id="9ec83-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ec83-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9ec83-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ec83-113">Permission type</span></span>                        | <span data-ttu-id="9ec83-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9ec83-114">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="9ec83-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ec83-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ec83-116">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ec83-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="9ec83-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ec83-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ec83-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ec83-118">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="9ec83-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ec83-119">Application</span></span>                            | <span data-ttu-id="9ec83-120">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ec83-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ec83-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ec83-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ec83-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9ec83-122">Optional query parameters</span></span>

<span data-ttu-id="9ec83-123">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9ec83-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ec83-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ec83-124">Request headers</span></span>

| <span data-ttu-id="9ec83-125">标头</span><span class="sxs-lookup"><span data-stu-id="9ec83-125">Header</span></span>        | <span data-ttu-id="9ec83-126">值</span><span class="sxs-lookup"><span data-stu-id="9ec83-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="9ec83-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ec83-127">Authorization</span></span> | <span data-ttu-id="9ec83-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9ec83-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ec83-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ec83-130">Request body</span></span>

<span data-ttu-id="9ec83-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9ec83-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ec83-132">响应</span><span class="sxs-lookup"><span data-stu-id="9ec83-132">Response</span></span>

<span data-ttu-id="9ec83-133">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [educationSubmissionResource](../resources/educationsubmissionresource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9ec83-133">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ec83-134">示例</span><span class="sxs-lookup"><span data-stu-id="9ec83-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9ec83-135">请求</span><span class="sxs-lookup"><span data-stu-id="9ec83-135">Request</span></span>

<span data-ttu-id="9ec83-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9ec83-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9ec83-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ec83-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_resources_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/{id}/assignments/{id}/submissions/{id}/resources
```
# <a name="c"></a>[<span data-ttu-id="9ec83-138">C#</span><span class="sxs-lookup"><span data-stu-id="9ec83-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resources-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ec83-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ec83-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resources-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ec83-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ec83-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resources-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ec83-141">Java</span><span class="sxs-lookup"><span data-stu-id="9ec83-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-resources-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9ec83-142">响应</span><span class="sxs-lookup"><span data-stu-id="9ec83-142">Response</span></span>

<span data-ttu-id="9ec83-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9ec83-143">The following is an example of the response.</span></span> 

><span data-ttu-id="9ec83-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9ec83-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1045

{
  "value": [
    {
      "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "id": "f2387c3b-ec39-4bf2-a399-d7242677f024",
      "resource": {
          "@odata.type": "#microsoft.graph.educationLinkResource",
          "displayName": "Microsoft Homepage",
          "createdDateTime": "2017-10-21T07:52:45.5675913Z",
          "createdBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "lastModifiedDateTime": "2017-10-21T07:52:45.5675913Z",
          "lastModifiedBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "link": "https://www.microsoft.com"
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
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
