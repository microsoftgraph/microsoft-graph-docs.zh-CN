---
title: 列出用户
description: 检索 user 对象列表。 这些 user 对象将包含特定于教育的属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 10ec2434232b963e3e88a6e52134e4550edff4b5
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33616180"
---
# <a name="list-users"></a><span data-ttu-id="1ae89-104">列出用户</span><span class="sxs-lookup"><span data-stu-id="1ae89-104">List users</span></span>

<span data-ttu-id="1ae89-105">检索 user 对象列表。</span><span class="sxs-lookup"><span data-stu-id="1ae89-105">Retrieve a list of user objects.</span></span> <span data-ttu-id="1ae89-106">这些 user 对象将包含特定于教育的属性。</span><span class="sxs-lookup"><span data-stu-id="1ae89-106">These user objects will include education-specific properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ae89-107">权限</span><span class="sxs-lookup"><span data-stu-id="1ae89-107">Permissions</span></span>
<span data-ttu-id="1ae89-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ae89-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ae89-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ae89-110">Permission type</span></span>      | <span data-ttu-id="1ae89-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ae89-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ae89-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ae89-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="1ae89-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ae89-113">Not supported.</span></span>  |
|<span data-ttu-id="1ae89-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ae89-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1ae89-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ae89-115">Not supported.</span></span>  |
|<span data-ttu-id="1ae89-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ae89-116">Application</span></span> | <span data-ttu-id="1ae89-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ae89-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1ae89-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ae89-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1ae89-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1ae89-119">Optional query parameters</span></span>
<span data-ttu-id="1ae89-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1ae89-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ae89-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ae89-121">Request headers</span></span>
| <span data-ttu-id="1ae89-122">标头</span><span class="sxs-lookup"><span data-stu-id="1ae89-122">Header</span></span>       | <span data-ttu-id="1ae89-123">值</span><span class="sxs-lookup"><span data-stu-id="1ae89-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1ae89-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ae89-124">Authorization</span></span>  | <span data-ttu-id="1ae89-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1ae89-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1ae89-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ae89-127">Request body</span></span>
<span data-ttu-id="1ae89-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1ae89-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1ae89-129">响应</span><span class="sxs-lookup"><span data-stu-id="1ae89-129">Response</span></span>
<span data-ttu-id="1ae89-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="1ae89-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1ae89-131">示例</span><span class="sxs-lookup"><span data-stu-id="1ae89-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ae89-132">请求</span><span class="sxs-lookup"><span data-stu-id="1ae89-132">Request</span></span>
<span data-ttu-id="1ae89-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1ae89-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/users
```
##### <a name="response"></a><span data-ttu-id="1ae89-134">响应</span><span class="sxs-lookup"><span data-stu-id="1ae89-134">Response</span></span>
<span data-ttu-id="1ae89-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1ae89-135">The following is an example of the response.</span></span> 

><span data-ttu-id="1ae89-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1ae89-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1ae89-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="1ae89-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1ae89-139">语言</span><span class="sxs-lookup"><span data-stu-id="1ae89-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_users-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1ae89-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="1ae89-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_users-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationroot-list-users.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationroot-list-users.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
