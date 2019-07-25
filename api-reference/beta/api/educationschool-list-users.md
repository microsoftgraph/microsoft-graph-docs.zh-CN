---
title: 列出 educationUsers
description: 检索学校中的用户列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 154d3a9dcb2e3dd3a4203677d2eb57eae44daafd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860267"
---
# <a name="list-educationusers"></a><span data-ttu-id="0616a-103">列出 educationUsers</span><span class="sxs-lookup"><span data-stu-id="0616a-103">List educationUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0616a-104">检索学校中的用户列表。</span><span class="sxs-lookup"><span data-stu-id="0616a-104">Retrieve a list of users at a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="0616a-105">权限</span><span class="sxs-lookup"><span data-stu-id="0616a-105">Permissions</span></span>
<span data-ttu-id="0616a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0616a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0616a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0616a-108">Permission type</span></span>      | <span data-ttu-id="0616a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0616a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0616a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0616a-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="0616a-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="0616a-111">Not supported.</span></span>  |
|<span data-ttu-id="0616a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0616a-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0616a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0616a-113">Not supported.</span></span>  |
|<span data-ttu-id="0616a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0616a-114">Application</span></span> | <span data-ttu-id="0616a-115">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0616a-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0616a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0616a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0616a-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0616a-117">Optional query parameters</span></span>
<span data-ttu-id="0616a-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0616a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0616a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0616a-119">Request headers</span></span>
| <span data-ttu-id="0616a-120">标头</span><span class="sxs-lookup"><span data-stu-id="0616a-120">Header</span></span>       | <span data-ttu-id="0616a-121">值</span><span class="sxs-lookup"><span data-stu-id="0616a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0616a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0616a-122">Authorization</span></span>  | <span data-ttu-id="0616a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0616a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0616a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0616a-125">Request body</span></span>
<span data-ttu-id="0616a-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0616a-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0616a-127">响应</span><span class="sxs-lookup"><span data-stu-id="0616a-127">Response</span></span>
<span data-ttu-id="0616a-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="0616a-128">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0616a-129">示例</span><span class="sxs-lookup"><span data-stu-id="0616a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0616a-130">请求</span><span class="sxs-lookup"><span data-stu-id="0616a-130">Request</span></span>
<span data-ttu-id="0616a-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0616a-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0616a-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0616a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationschool_get_users"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/10002/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0616a-133">C#</span><span class="sxs-lookup"><span data-stu-id="0616a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationschool-get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0616a-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="0616a-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationschool-get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0616a-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="0616a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationschool-get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0616a-136">Java</span><span class="sxs-lookup"><span data-stu-id="0616a-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationschool-get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0616a-137">响应</span><span class="sxs-lookup"><span data-stu-id="0616a-137">Response</span></span>
<span data-ttu-id="0616a-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0616a-138">The following is an example of the response.</span></span> 

><span data-ttu-id="0616a-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0616a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 593

{
  "value": [
    {
      "id": "13012",
      "displayName": "Dion Matheson",
      "givenName": "Dion",
      "middleName": " ",
      "surname": "Matheson",
      "mail": "DionM@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "sis",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "student",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
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
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
