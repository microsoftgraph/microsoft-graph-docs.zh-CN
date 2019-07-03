---
title: 列出 educationSchools
description: 检索所有 school 对象的列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 87b521dd870eaf715d67afc72128e0bc5f006db1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441574"
---
# <a name="list-educationschools"></a><span data-ttu-id="fc0e9-103">列出 educationSchools</span><span class="sxs-lookup"><span data-stu-id="fc0e9-103">List educationSchools</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc0e9-104">检索所有 school 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="fc0e9-104">Retrieve a list of all school objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc0e9-105">权限</span><span class="sxs-lookup"><span data-stu-id="fc0e9-105">Permissions</span></span>
<span data-ttu-id="fc0e9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc0e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc0e9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc0e9-108">Permission type</span></span>      | <span data-ttu-id="fc0e9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc0e9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc0e9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc0e9-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="fc0e9-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="fc0e9-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="fc0e9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc0e9-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fc0e9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc0e9-113">Not supported.</span></span>  |
|<span data-ttu-id="fc0e9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc0e9-114">Application</span></span> | <span data-ttu-id="fc0e9-115">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc0e9-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fc0e9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc0e9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="fc0e9-117">\`\`\`http GET /education/schools</span><span class="sxs-lookup"><span data-stu-id="fc0e9-117">\`\`\`http GET /education/schools</span></span>
```
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.

## Request headers
| Header       | Value |
|:---------------|:--------|
| Authorization  | Bearer {token}. Required.  |

## Request body
Do not supply a request body for this method.
## Response
If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.
## Example
##### Request
The following is an example of the request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fc0e9-118">C#</span><span class="sxs-lookup"><span data-stu-id="fc0e9-118">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc0e9-119">Javascript</span><span class="sxs-lookup"><span data-stu-id="fc0e9-119">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fc0e9-120">目标-C</span><span class="sxs-lookup"><span data-stu-id="fc0e9-120">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fc0e9-121">响应</span><span class="sxs-lookup"><span data-stu-id="fc0e9-121">Response</span></span>
<span data-ttu-id="fc0e9-122">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fc0e9-122">The following is an example of the response.</span></span> 

><span data-ttu-id="fc0e9-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fc0e9-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
    {
      "id": "10001",
      "displayName": "Contoso High School",
      "description": "Public 9-12 high school",
      "status": "active",
      "externalSource": "sis",
      "principalEmail": "amyr@contoso.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10001",
      "address": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalId": "10001",
      "fax": "+1 (253) 555-0101",
      "phone": "+1 (253) 555-0102",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
