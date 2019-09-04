---
title: 列出用户
description: 检索 user 对象列表。 这些 user 对象将包含特定于教育的属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6f594654f1ba0b980acbc5ea61dc0a7a898f7a71
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720408"
---
# <a name="list-users"></a><span data-ttu-id="92975-104">列出用户</span><span class="sxs-lookup"><span data-stu-id="92975-104">List users</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92975-105">检索 user 对象列表。</span><span class="sxs-lookup"><span data-stu-id="92975-105">Retrieve a list of user objects.</span></span> <span data-ttu-id="92975-106">这些 user 对象将包含特定于教育的属性。</span><span class="sxs-lookup"><span data-stu-id="92975-106">These user objects will include education-specific properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="92975-107">权限</span><span class="sxs-lookup"><span data-stu-id="92975-107">Permissions</span></span>
<span data-ttu-id="92975-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92975-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92975-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="92975-110">Permission type</span></span>      | <span data-ttu-id="92975-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="92975-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92975-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92975-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="92975-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="92975-113">Not supported.</span></span>  |
|<span data-ttu-id="92975-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92975-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="92975-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="92975-115">Not supported.</span></span>  |
|<span data-ttu-id="92975-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="92975-116">Application</span></span> | <span data-ttu-id="92975-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92975-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="92975-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92975-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="92975-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="92975-119">Optional query parameters</span></span>
<span data-ttu-id="92975-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="92975-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92975-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="92975-121">Request headers</span></span>
| <span data-ttu-id="92975-122">标头</span><span class="sxs-lookup"><span data-stu-id="92975-122">Header</span></span>       | <span data-ttu-id="92975-123">值</span><span class="sxs-lookup"><span data-stu-id="92975-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="92975-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="92975-124">Authorization</span></span>  | <span data-ttu-id="92975-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="92975-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="92975-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="92975-127">Request body</span></span>
<span data-ttu-id="92975-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="92975-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="92975-129">响应</span><span class="sxs-lookup"><span data-stu-id="92975-129">Response</span></span>
<span data-ttu-id="92975-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="92975-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="92975-131">示例</span><span class="sxs-lookup"><span data-stu-id="92975-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92975-132">请求</span><span class="sxs-lookup"><span data-stu-id="92975-132">Request</span></span>
<span data-ttu-id="92975-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="92975-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="92975-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="92975-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationroot_get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="92975-135">C#</span><span class="sxs-lookup"><span data-stu-id="92975-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationroot-get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="92975-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92975-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationroot-get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="92975-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="92975-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationroot-get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="92975-138">响应</span><span class="sxs-lookup"><span data-stu-id="92975-138">Response</span></span>
<span data-ttu-id="92975-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="92975-139">The following is an example of the response.</span></span> 

><span data-ttu-id="92975-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="92975-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "middleName": null,
      "surname": "Matheson",
      "mail": "DionM@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012"
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
