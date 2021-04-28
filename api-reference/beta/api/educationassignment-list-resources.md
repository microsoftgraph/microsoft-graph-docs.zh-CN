---
title: 列出 educationAssignmentResources
description: 获取与此工作分配关联的所有资源。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b788f254972832832336d5b7b69d8b6b8ec085cd
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061691"
---
# <a name="list-educationassignmentresources"></a><span data-ttu-id="4badb-103">列出 educationAssignmentResources</span><span class="sxs-lookup"><span data-stu-id="4badb-103">List educationAssignmentResources</span></span>

<span data-ttu-id="4badb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4badb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4badb-105">获取与此工作分配关联的所有资源。</span><span class="sxs-lookup"><span data-stu-id="4badb-105">Get all the resources associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="4badb-106">权限</span><span class="sxs-lookup"><span data-stu-id="4badb-106">Permissions</span></span>
<span data-ttu-id="4badb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4badb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4badb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4badb-109">Permission type</span></span>      | <span data-ttu-id="4badb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4badb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4badb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4badb-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="4badb-112">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4badb-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="4badb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4badb-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4badb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4badb-114">Not supported.</span></span>  |
|<span data-ttu-id="4badb-115">Application\*</span><span class="sxs-lookup"><span data-stu-id="4badb-115">Application\*</span></span> | <span data-ttu-id="4badb-116">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4badb-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

<span data-ttu-id="4badb-117">\*应用程序权限当前仅适用于个人预览版客户。</span><span class="sxs-lookup"><span data-stu-id="4badb-117">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="4badb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4badb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4badb-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4badb-119">Optional query parameters</span></span>
<span data-ttu-id="4badb-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4badb-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4badb-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4badb-121">Request headers</span></span>
| <span data-ttu-id="4badb-122">标头</span><span class="sxs-lookup"><span data-stu-id="4badb-122">Header</span></span>       | <span data-ttu-id="4badb-123">值</span><span class="sxs-lookup"><span data-stu-id="4badb-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4badb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4badb-124">Authorization</span></span>  | <span data-ttu-id="4badb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4badb-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4badb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4badb-127">Request body</span></span>
<span data-ttu-id="4badb-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4badb-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4badb-129">响应</span><span class="sxs-lookup"><span data-stu-id="4badb-129">Response</span></span>
<span data-ttu-id="4badb-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [educationAssignmentResource](../resources/educationassignmentresource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4badb-130">If successful, this method returns a `200 OK` response code and a collection of [educationAssignmentResource](../resources/educationassignmentresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4badb-131">示例</span><span class="sxs-lookup"><span data-stu-id="4badb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4badb-132">请求</span><span class="sxs-lookup"><span data-stu-id="4badb-132">Request</span></span>
<span data-ttu-id="4badb-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4badb-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4badb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4badb-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_resources_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/resources
```
# <a name="c"></a>[<span data-ttu-id="4badb-135">C#</span><span class="sxs-lookup"><span data-stu-id="4badb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resources-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4badb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4badb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resources-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4badb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4badb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resources-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4badb-138">Java</span><span class="sxs-lookup"><span data-stu-id="4badb-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-resources-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4badb-139">响应</span><span class="sxs-lookup"><span data-stu-id="4badb-139">Response</span></span>
<span data-ttu-id="4badb-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4badb-140">The following is an example of the response.</span></span> 

><span data-ttu-id="4badb-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4badb-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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
