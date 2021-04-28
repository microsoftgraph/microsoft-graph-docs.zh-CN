---
title: 列出 educationUsers
description: 检索学校中的用户列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 183a4ee58a4e8b3b25ce7ba526ca74af97ee00e2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035468"
---
# <a name="list-educationusers"></a><span data-ttu-id="e248a-103">列出 educationUsers</span><span class="sxs-lookup"><span data-stu-id="e248a-103">List educationUsers</span></span>

<span data-ttu-id="e248a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e248a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e248a-105">检索学校中的用户列表。</span><span class="sxs-lookup"><span data-stu-id="e248a-105">Retrieve a list of users at a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="e248a-106">权限</span><span class="sxs-lookup"><span data-stu-id="e248a-106">Permissions</span></span>
<span data-ttu-id="e248a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e248a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e248a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e248a-109">Permission type</span></span>      | <span data-ttu-id="e248a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e248a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e248a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e248a-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="e248a-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e248a-112">Not supported.</span></span>  |
|<span data-ttu-id="e248a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e248a-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e248a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e248a-114">Not supported.</span></span>  |
|<span data-ttu-id="e248a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e248a-115">Application</span></span> | <span data-ttu-id="e248a-116">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e248a-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e248a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e248a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e248a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e248a-118">Optional query parameters</span></span>
<span data-ttu-id="e248a-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e248a-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e248a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e248a-120">Request headers</span></span>
| <span data-ttu-id="e248a-121">标头</span><span class="sxs-lookup"><span data-stu-id="e248a-121">Header</span></span>       | <span data-ttu-id="e248a-122">值</span><span class="sxs-lookup"><span data-stu-id="e248a-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e248a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e248a-123">Authorization</span></span>  | <span data-ttu-id="e248a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e248a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e248a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e248a-126">Request body</span></span>
<span data-ttu-id="e248a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e248a-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e248a-128">响应</span><span class="sxs-lookup"><span data-stu-id="e248a-128">Response</span></span>
<span data-ttu-id="e248a-129">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="e248a-129">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e248a-130">示例</span><span class="sxs-lookup"><span data-stu-id="e248a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e248a-131">请求</span><span class="sxs-lookup"><span data-stu-id="e248a-131">Request</span></span>
<span data-ttu-id="e248a-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e248a-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e248a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e248a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationschool_get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}/users
```
# <a name="c"></a>[<span data-ttu-id="e248a-134">C#</span><span class="sxs-lookup"><span data-stu-id="e248a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationschool-get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e248a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e248a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationschool-get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e248a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e248a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationschool-get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e248a-137">Java</span><span class="sxs-lookup"><span data-stu-id="e248a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationschool-get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e248a-138">响应</span><span class="sxs-lookup"><span data-stu-id="e248a-138">Response</span></span>
<span data-ttu-id="e248a-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e248a-139">The following is an example of the response.</span></span> 

><span data-ttu-id="e248a-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e248a-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
