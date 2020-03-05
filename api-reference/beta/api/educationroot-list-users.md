---
title: 列出用户
description: 检索用户对象列表。 这些 user 对象将包含特定于教育的属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3c7e8873446748db69fb9f3f0da086d14ab9a79f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42426099"
---
# <a name="list-users"></a><span data-ttu-id="87794-104">列出用户</span><span class="sxs-lookup"><span data-stu-id="87794-104">List users</span></span>

<span data-ttu-id="87794-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="87794-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87794-106">检索 user 对象列表。</span><span class="sxs-lookup"><span data-stu-id="87794-106">Retrieve a list of user objects.</span></span> <span data-ttu-id="87794-107">这些 user 对象将包含特定于教育的属性。</span><span class="sxs-lookup"><span data-stu-id="87794-107">These user objects will include education-specific properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="87794-108">权限</span><span class="sxs-lookup"><span data-stu-id="87794-108">Permissions</span></span>
<span data-ttu-id="87794-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="87794-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87794-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="87794-111">Permission type</span></span>      | <span data-ttu-id="87794-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="87794-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87794-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="87794-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="87794-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="87794-114">Not supported.</span></span>  |
|<span data-ttu-id="87794-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="87794-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="87794-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="87794-116">Not supported.</span></span>  |
|<span data-ttu-id="87794-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="87794-117">Application</span></span> | <span data-ttu-id="87794-118">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87794-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="87794-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="87794-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="87794-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="87794-120">Optional query parameters</span></span>
<span data-ttu-id="87794-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="87794-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87794-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="87794-122">Request headers</span></span>
| <span data-ttu-id="87794-123">标头</span><span class="sxs-lookup"><span data-stu-id="87794-123">Header</span></span>       | <span data-ttu-id="87794-124">值</span><span class="sxs-lookup"><span data-stu-id="87794-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="87794-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="87794-125">Authorization</span></span>  | <span data-ttu-id="87794-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="87794-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="87794-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="87794-128">Request body</span></span>
<span data-ttu-id="87794-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="87794-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="87794-130">响应</span><span class="sxs-lookup"><span data-stu-id="87794-130">Response</span></span>
<span data-ttu-id="87794-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="87794-131">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="87794-132">示例</span><span class="sxs-lookup"><span data-stu-id="87794-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87794-133">请求</span><span class="sxs-lookup"><span data-stu-id="87794-133">Request</span></span>
<span data-ttu-id="87794-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="87794-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="87794-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="87794-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationroot_get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/users
```
# <a name="c"></a>[<span data-ttu-id="87794-136">C#</span><span class="sxs-lookup"><span data-stu-id="87794-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationroot-get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87794-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87794-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationroot-get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87794-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87794-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationroot-get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="87794-139">响应</span><span class="sxs-lookup"><span data-stu-id="87794-139">Response</span></span>
<span data-ttu-id="87794-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="87794-140">The following is an example of the response.</span></span> 

><span data-ttu-id="87794-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="87794-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
