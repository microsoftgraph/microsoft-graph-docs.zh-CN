---
title: 列出 educationSchools
description: 检索所有 school 对象的列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 947754b6b043665d38c2ad209325bed5fbd2ea00
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720415"
---
# <a name="list-educationschools"></a><span data-ttu-id="3985c-103">列出 educationSchools</span><span class="sxs-lookup"><span data-stu-id="3985c-103">List educationSchools</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3985c-104">检索所有 school 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="3985c-104">Retrieve a list of all school objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="3985c-105">权限</span><span class="sxs-lookup"><span data-stu-id="3985c-105">Permissions</span></span>
<span data-ttu-id="3985c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3985c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3985c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3985c-108">Permission type</span></span>      | <span data-ttu-id="3985c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3985c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3985c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3985c-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="3985c-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="3985c-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="3985c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3985c-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3985c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3985c-113">Not supported.</span></span>  |
|<span data-ttu-id="3985c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3985c-114">Application</span></span> | <span data-ttu-id="3985c-115">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3985c-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3985c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3985c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http GET /education/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3985c-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3985c-117">Optional query parameters</span></span>
<span data-ttu-id="3985c-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3985c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3985c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3985c-119">Request headers</span></span>
| <span data-ttu-id="3985c-120">标头</span><span class="sxs-lookup"><span data-stu-id="3985c-120">Header</span></span>       | <span data-ttu-id="3985c-121">值</span><span class="sxs-lookup"><span data-stu-id="3985c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3985c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3985c-122">Authorization</span></span>  | <span data-ttu-id="3985c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3985c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3985c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3985c-125">Request body</span></span>
<span data-ttu-id="3985c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3985c-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3985c-127">响应</span><span class="sxs-lookup"><span data-stu-id="3985c-127">Response</span></span>
<span data-ttu-id="3985c-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationSchool](../resources/educationschool.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="3985c-128">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3985c-129">示例</span><span class="sxs-lookup"><span data-stu-id="3985c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3985c-130">请求</span><span class="sxs-lookup"><span data-stu-id="3985c-130">Request</span></span>
<span data-ttu-id="3985c-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3985c-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3985c-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="3985c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3985c-133">C#</span><span class="sxs-lookup"><span data-stu-id="3985c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3985c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3985c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3985c-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="3985c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3985c-136">响应</span><span class="sxs-lookup"><span data-stu-id="3985c-136">Response</span></span>
<span data-ttu-id="3985c-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3985c-137">The following is an example of the response.</span></span> 

><span data-ttu-id="3985c-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3985c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
