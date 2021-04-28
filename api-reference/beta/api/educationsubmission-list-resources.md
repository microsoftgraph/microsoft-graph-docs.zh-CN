---
title: 列出资源
description: 列出与此提交关联的资源。 **submissionResource** 对象是学生正在处理的实际资源对象的包装。 如果资源是在分配过程中从分配复制的，包装器还包括指向分配上的资源的指针。 这些资源是工作分配的工作副本。 **submittedResources** 是已正式提交进行评分的资源。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 20d6cf5f500e23b3259be57e81ecdae754797d2f
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061628"
---
# <a name="list-resources"></a><span data-ttu-id="071ee-107">列出资源</span><span class="sxs-lookup"><span data-stu-id="071ee-107">List resources</span></span>

<span data-ttu-id="071ee-108">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="071ee-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="071ee-109">列出与此提交关联的资源。</span><span class="sxs-lookup"><span data-stu-id="071ee-109">List the resources associated with this submission.</span></span> <span data-ttu-id="071ee-110">**submissionResource** 对象是学生正在处理的实际资源对象的包装。</span><span class="sxs-lookup"><span data-stu-id="071ee-110">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="071ee-111">如果资源是在分配过程中从分配复制的，包装器还包括指向分配上的资源的指针。</span><span class="sxs-lookup"><span data-stu-id="071ee-111">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="071ee-112">这些资源是工作分配的工作副本。</span><span class="sxs-lookup"><span data-stu-id="071ee-112">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="071ee-113">**submittedResources** 是已正式提交进行评分的资源。</span><span class="sxs-lookup"><span data-stu-id="071ee-113">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="071ee-114">权限</span><span class="sxs-lookup"><span data-stu-id="071ee-114">Permissions</span></span>

<span data-ttu-id="071ee-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="071ee-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="071ee-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="071ee-117">Permission type</span></span>                        | <span data-ttu-id="071ee-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="071ee-118">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="071ee-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="071ee-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="071ee-120">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="071ee-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="071ee-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="071ee-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="071ee-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="071ee-122">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="071ee-123">Application\*</span><span class="sxs-lookup"><span data-stu-id="071ee-123">Application\*</span></span>                           | <span data-ttu-id="071ee-124">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="071ee-124">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

<span data-ttu-id="071ee-125">\*应用程序权限当前仅适用于个人预览版客户。</span><span class="sxs-lookup"><span data-stu-id="071ee-125">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="071ee-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="071ee-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="071ee-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="071ee-127">Optional query parameters</span></span>

<span data-ttu-id="071ee-128">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="071ee-128">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="071ee-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="071ee-129">Request headers</span></span>

| <span data-ttu-id="071ee-130">标头</span><span class="sxs-lookup"><span data-stu-id="071ee-130">Header</span></span>        | <span data-ttu-id="071ee-131">值</span><span class="sxs-lookup"><span data-stu-id="071ee-131">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="071ee-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="071ee-132">Authorization</span></span> | <span data-ttu-id="071ee-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="071ee-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="071ee-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="071ee-135">Request body</span></span>

<span data-ttu-id="071ee-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="071ee-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="071ee-137">响应</span><span class="sxs-lookup"><span data-stu-id="071ee-137">Response</span></span>

<span data-ttu-id="071ee-138">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [educationSubmissionResource](../resources/educationsubmissionresource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="071ee-138">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="071ee-139">示例</span><span class="sxs-lookup"><span data-stu-id="071ee-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="071ee-140">请求</span><span class="sxs-lookup"><span data-stu-id="071ee-140">Request</span></span>

<span data-ttu-id="071ee-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="071ee-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="071ee-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="071ee-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_resources_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/{id}/assignments/{id}/submissions/{id}/resources
```
# <a name="c"></a>[<span data-ttu-id="071ee-143">C#</span><span class="sxs-lookup"><span data-stu-id="071ee-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resources-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="071ee-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="071ee-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resources-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="071ee-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="071ee-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resources-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="071ee-146">Java</span><span class="sxs-lookup"><span data-stu-id="071ee-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-resources-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="071ee-147">响应</span><span class="sxs-lookup"><span data-stu-id="071ee-147">Response</span></span>

<span data-ttu-id="071ee-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="071ee-148">The following is an example of the response.</span></span> 

><span data-ttu-id="071ee-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="071ee-149">**Note:** The response object shown here might be shortened for readability.</span></span>

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
