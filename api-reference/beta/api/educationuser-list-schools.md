---
title: 列出学校
description: 检索用户所在的学校列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4486dce1155bf63eecf5ad5c4b1aa0f4fa20b4d7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259323"
---
# <a name="list-schools"></a><span data-ttu-id="b4df8-103">列出学校</span><span class="sxs-lookup"><span data-stu-id="b4df8-103">List schools</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4df8-104">检索用户所在的学校列表。</span><span class="sxs-lookup"><span data-stu-id="b4df8-104">Retrieve a list of schools for a user.</span></span>

><span data-ttu-id="b4df8-105">**注意：** 如果使用委派令牌，成员只能看到有关自己学校的信息。</span><span class="sxs-lookup"><span data-stu-id="b4df8-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="b4df8-106">在这种情况下，使用 `...beta/education/me/schools` 资源。</span><span class="sxs-lookup"><span data-stu-id="b4df8-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4df8-107">权限</span><span class="sxs-lookup"><span data-stu-id="b4df8-107">Permissions</span></span>
<span data-ttu-id="b4df8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4df8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4df8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4df8-110">Permission type</span></span>      | <span data-ttu-id="b4df8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4df8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4df8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4df8-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="b4df8-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="b4df8-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="b4df8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4df8-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b4df8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4df8-115">Not supported.</span></span>  |
|<span data-ttu-id="b4df8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4df8-116">Application</span></span> | <span data-ttu-id="b4df8-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4df8-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b4df8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4df8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b4df8-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b4df8-119">Optional query parameters</span></span>
<span data-ttu-id="b4df8-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b4df8-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4df8-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4df8-121">Request headers</span></span>
| <span data-ttu-id="b4df8-122">标头</span><span class="sxs-lookup"><span data-stu-id="b4df8-122">Header</span></span>       | <span data-ttu-id="b4df8-123">值</span><span class="sxs-lookup"><span data-stu-id="b4df8-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b4df8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4df8-124">Authorization</span></span>  | <span data-ttu-id="b4df8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4df8-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b4df8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4df8-127">Request body</span></span>
<span data-ttu-id="b4df8-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b4df8-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b4df8-129">响应</span><span class="sxs-lookup"><span data-stu-id="b4df8-129">Response</span></span>
<span data-ttu-id="b4df8-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationSchool](../resources/educationschool.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="b4df8-130">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b4df8-131">示例</span><span class="sxs-lookup"><span data-stu-id="b4df8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4df8-132">请求</span><span class="sxs-lookup"><span data-stu-id="b4df8-132">Request</span></span>
<span data-ttu-id="b4df8-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b4df8-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/schools
```
##### <a name="response"></a><span data-ttu-id="b4df8-134">响应</span><span class="sxs-lookup"><span data-stu-id="b4df8-134">Response</span></span>
<span data-ttu-id="b4df8-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b4df8-135">The following is an example of the response.</span></span> 

><span data-ttu-id="b4df8-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b4df8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b4df8-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="b4df8-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b4df8-139">C#</span><span class="sxs-lookup"><span data-stu-id="b4df8-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_schools-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b4df8-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="b4df8-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_schools-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b4df8-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="b4df8-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_schools-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/educationuser-list-schools.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationuser-list-schools.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationuser-list-schools.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
