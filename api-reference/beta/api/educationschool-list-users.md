---
title: 列出 educationUsers
description: 检索学校中的用户列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5b51d0816e61370d1c4da804f5b9f5f56abe28ff
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48403400"
---
# <a name="list-educationusers"></a><span data-ttu-id="5a93b-103">列出 educationUsers</span><span class="sxs-lookup"><span data-stu-id="5a93b-103">List educationUsers</span></span>

<span data-ttu-id="5a93b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a93b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a93b-105">检索学校中的用户列表。</span><span class="sxs-lookup"><span data-stu-id="5a93b-105">Retrieve a list of users at a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a93b-106">权限</span><span class="sxs-lookup"><span data-stu-id="5a93b-106">Permissions</span></span>
<span data-ttu-id="5a93b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a93b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a93b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a93b-109">Permission type</span></span>      | <span data-ttu-id="5a93b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5a93b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a93b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a93b-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="5a93b-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a93b-112">Not supported.</span></span>  |
|<span data-ttu-id="5a93b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a93b-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5a93b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a93b-114">Not supported.</span></span>  |
|<span data-ttu-id="5a93b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a93b-115">Application</span></span> | <span data-ttu-id="5a93b-116">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a93b-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5a93b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a93b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5a93b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5a93b-118">Optional query parameters</span></span>
<span data-ttu-id="5a93b-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5a93b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a93b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a93b-120">Request headers</span></span>
| <span data-ttu-id="5a93b-121">标头</span><span class="sxs-lookup"><span data-stu-id="5a93b-121">Header</span></span>       | <span data-ttu-id="5a93b-122">值</span><span class="sxs-lookup"><span data-stu-id="5a93b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5a93b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a93b-123">Authorization</span></span>  | <span data-ttu-id="5a93b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5a93b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5a93b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a93b-126">Request body</span></span>
<span data-ttu-id="5a93b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5a93b-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5a93b-128">响应</span><span class="sxs-lookup"><span data-stu-id="5a93b-128">Response</span></span>
<span data-ttu-id="5a93b-129">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="5a93b-129">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5a93b-130">示例</span><span class="sxs-lookup"><span data-stu-id="5a93b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a93b-131">请求</span><span class="sxs-lookup"><span data-stu-id="5a93b-131">Request</span></span>
<span data-ttu-id="5a93b-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5a93b-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5a93b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a93b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationschool_get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools/10002/users
```
# <a name="c"></a>[<span data-ttu-id="5a93b-134">C#</span><span class="sxs-lookup"><span data-stu-id="5a93b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationschool-get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a93b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a93b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationschool-get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a93b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a93b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationschool-get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5a93b-137">响应</span><span class="sxs-lookup"><span data-stu-id="5a93b-137">Response</span></span>
<span data-ttu-id="5a93b-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5a93b-138">The following is an example of the response.</span></span> 

><span data-ttu-id="5a93b-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5a93b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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