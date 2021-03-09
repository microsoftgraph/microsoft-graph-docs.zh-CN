---
title: 列出资源
description: 列出与此提交关联的资源。 **submissionResource** 对象是围绕学生正在处理的实际资源对象的包装。 如果在分配过程中从分配中复制了该资源，包装器还包括指向工作分配上的资源的指针。 这些资源是工作分配的工作副本。 **submittedResources** 是已正式提交以评分的资源。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 9f22b67c47afdb96764b2fadb0b1ea1af2344ed0
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574291"
---
# <a name="list-resources"></a><span data-ttu-id="2d44c-107">列出资源</span><span class="sxs-lookup"><span data-stu-id="2d44c-107">List resources</span></span>

<span data-ttu-id="2d44c-108">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d44c-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d44c-109">列出与此提交关联的资源。</span><span class="sxs-lookup"><span data-stu-id="2d44c-109">List the resources associated with this submission.</span></span> <span data-ttu-id="2d44c-110">**submissionResource** 对象是围绕学生正在处理的实际资源对象的包装。</span><span class="sxs-lookup"><span data-stu-id="2d44c-110">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="2d44c-111">如果在分配过程中从分配中复制了该资源，包装器还包括指向工作分配上的资源的指针。</span><span class="sxs-lookup"><span data-stu-id="2d44c-111">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="2d44c-112">这些资源是工作分配的工作副本。</span><span class="sxs-lookup"><span data-stu-id="2d44c-112">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="2d44c-113">**submittedResources** 是已正式提交以评分的资源。</span><span class="sxs-lookup"><span data-stu-id="2d44c-113">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d44c-114">权限</span><span class="sxs-lookup"><span data-stu-id="2d44c-114">Permissions</span></span>

<span data-ttu-id="2d44c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d44c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2d44c-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d44c-117">Permission type</span></span>                        | <span data-ttu-id="2d44c-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2d44c-118">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="2d44c-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d44c-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d44c-120">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d44c-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="2d44c-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d44c-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d44c-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d44c-122">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="2d44c-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d44c-123">Application</span></span>                            | <span data-ttu-id="2d44c-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d44c-124">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="2d44c-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d44c-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2d44c-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2d44c-126">Optional query parameters</span></span>

<span data-ttu-id="2d44c-127">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2d44c-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d44c-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d44c-128">Request headers</span></span>

| <span data-ttu-id="2d44c-129">标头</span><span class="sxs-lookup"><span data-stu-id="2d44c-129">Header</span></span>        | <span data-ttu-id="2d44c-130">值</span><span class="sxs-lookup"><span data-stu-id="2d44c-130">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="2d44c-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d44c-131">Authorization</span></span> | <span data-ttu-id="2d44c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2d44c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d44c-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d44c-134">Request body</span></span>

<span data-ttu-id="2d44c-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2d44c-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d44c-136">响应</span><span class="sxs-lookup"><span data-stu-id="2d44c-136">Response</span></span>

<span data-ttu-id="2d44c-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [educationSubmissionResource](../resources/educationsubmissionresource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2d44c-137">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d44c-138">示例</span><span class="sxs-lookup"><span data-stu-id="2d44c-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2d44c-139">请求</span><span class="sxs-lookup"><span data-stu-id="2d44c-139">Request</span></span>

<span data-ttu-id="2d44c-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2d44c-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2d44c-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d44c-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_resources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/{id}/assignments/{id}/submissions/{id}/resources
```
# <a name="c"></a>[<span data-ttu-id="2d44c-142">C#</span><span class="sxs-lookup"><span data-stu-id="2d44c-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d44c-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d44c-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d44c-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d44c-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d44c-145">Java</span><span class="sxs-lookup"><span data-stu-id="2d44c-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-resources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2d44c-146">响应</span><span class="sxs-lookup"><span data-stu-id="2d44c-146">Response</span></span>

<span data-ttu-id="2d44c-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2d44c-147">The following is an example of the response.</span></span> 

><span data-ttu-id="2d44c-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2d44c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
