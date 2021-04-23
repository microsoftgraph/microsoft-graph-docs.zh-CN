---
title: 列出 educationAssignmentResources
description: 获取与此工作分配关联的所有资源。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d770d17644462db110be021a541a0dfc28eacf9b
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961308"
---
# <a name="list-educationassignmentresources"></a><span data-ttu-id="88964-103">列出 educationAssignmentResources</span><span class="sxs-lookup"><span data-stu-id="88964-103">List educationAssignmentResources</span></span>

<span data-ttu-id="88964-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88964-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88964-105">获取与此工作分配关联的所有资源。</span><span class="sxs-lookup"><span data-stu-id="88964-105">Get all the resources associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="88964-106">权限</span><span class="sxs-lookup"><span data-stu-id="88964-106">Permissions</span></span>
<span data-ttu-id="88964-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88964-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88964-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="88964-109">Permission type</span></span>      | <span data-ttu-id="88964-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88964-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88964-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88964-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="88964-112">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88964-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="88964-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88964-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="88964-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="88964-114">Not supported.</span></span>  |
|<span data-ttu-id="88964-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="88964-115">Application</span></span> | <span data-ttu-id="88964-116">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88964-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="88964-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88964-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="88964-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="88964-118">Optional query parameters</span></span>
<span data-ttu-id="88964-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="88964-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88964-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="88964-120">Request headers</span></span>
| <span data-ttu-id="88964-121">标头</span><span class="sxs-lookup"><span data-stu-id="88964-121">Header</span></span>       | <span data-ttu-id="88964-122">值</span><span class="sxs-lookup"><span data-stu-id="88964-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="88964-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="88964-123">Authorization</span></span>  | <span data-ttu-id="88964-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="88964-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="88964-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="88964-126">Request body</span></span>
<span data-ttu-id="88964-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="88964-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="88964-128">响应</span><span class="sxs-lookup"><span data-stu-id="88964-128">Response</span></span>
<span data-ttu-id="88964-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [educationAssignmentResource](../resources/educationassignmentresource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="88964-129">If successful, this method returns a `200 OK` response code and a collection of [educationAssignmentResource](../resources/educationassignmentresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="88964-130">示例</span><span class="sxs-lookup"><span data-stu-id="88964-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88964-131">请求</span><span class="sxs-lookup"><span data-stu-id="88964-131">Request</span></span>
<span data-ttu-id="88964-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="88964-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="88964-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="88964-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_resources_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/resources
```
# <a name="c"></a>[<span data-ttu-id="88964-134">C#</span><span class="sxs-lookup"><span data-stu-id="88964-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resources-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88964-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88964-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resources-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88964-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88964-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resources-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88964-137">Java</span><span class="sxs-lookup"><span data-stu-id="88964-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-resources-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="88964-138">响应</span><span class="sxs-lookup"><span data-stu-id="88964-138">Response</span></span>
<span data-ttu-id="88964-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="88964-139">The following is an example of the response.</span></span> 

><span data-ttu-id="88964-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="88964-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1011

{
  "value": [
    {
      "distributeForStudentWork": false,
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
      },
      "id": "850f51b7-1df9-4ec0-bd62-64a0214b9cbf"
    },
    {
      "distributeForStudentWork": true,
      "resource": {
          "@odata.type": "#microsoft.graph.educationWordResource",
          "displayName": "Report.docx",
          "createdDateTime": "2017-10-21T07:52:53.9863696Z",
          "createdBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "lastModifiedDateTime": "2017-10-21T07:52:53.9863696Z",
          "lastModifiedBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6"
      },
      "id": "f2387c3b-ec39-4bf2-a399-d7242677f024"
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
