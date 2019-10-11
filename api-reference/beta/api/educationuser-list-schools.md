---
title: 列出学校
description: 检索用户所在的学校列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d55118e7a2e7c8718f506d983356b87fa007ad8e
ms.sourcegitcommit: e4b0211db9b20dfea8be964003661cd99fe064d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2019
ms.locfileid: "37439771"
---
# <a name="list-schools"></a><span data-ttu-id="16538-103">列出学校</span><span class="sxs-lookup"><span data-stu-id="16538-103">List schools</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16538-104">检索用户所在的学校列表。</span><span class="sxs-lookup"><span data-stu-id="16538-104">Retrieve a list of schools for a user.</span></span>

>[!Note]
><span data-ttu-id="16538-105">如果使用委派的令牌，则成员只能查看自己的学校的相关信息。</span><span class="sxs-lookup"><span data-stu-id="16538-105">If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="16538-106">在这种情况下，使用 `...beta/education/me/schools` 资源。</span><span class="sxs-lookup"><span data-stu-id="16538-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="16538-107">权限</span><span class="sxs-lookup"><span data-stu-id="16538-107">Permissions</span></span>

<span data-ttu-id="16538-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16538-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="16538-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="16538-110">Permission type</span></span>                        | <span data-ttu-id="16538-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16538-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="16538-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16538-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="16538-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="16538-113">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="16538-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16538-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16538-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="16538-115">Not supported.</span></span>                              |
| <span data-ttu-id="16538-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="16538-116">Application</span></span>                            | <span data-ttu-id="16538-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16538-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16538-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16538-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{id}/schools
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16538-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="16538-119">Optional query parameters</span></span>

<span data-ttu-id="16538-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="16538-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16538-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="16538-121">Request headers</span></span>

| <span data-ttu-id="16538-122">标头</span><span class="sxs-lookup"><span data-stu-id="16538-122">Header</span></span>        | <span data-ttu-id="16538-123">值</span><span class="sxs-lookup"><span data-stu-id="16538-123">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="16538-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="16538-124">Authorization</span></span> | <span data-ttu-id="16538-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="16538-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16538-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="16538-127">Request body</span></span>

<span data-ttu-id="16538-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="16538-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16538-129">响应</span><span class="sxs-lookup"><span data-stu-id="16538-129">Response</span></span>

<span data-ttu-id="16538-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationSchool](../resources/educationschool.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="16538-130">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16538-131">示例</span><span class="sxs-lookup"><span data-stu-id="16538-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="16538-132">请求</span><span class="sxs-lookup"><span data-stu-id="16538-132">Request</span></span>

<span data-ttu-id="16538-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="16538-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="16538-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="16538-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/schools
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="16538-135">C#</span><span class="sxs-lookup"><span data-stu-id="16538-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="16538-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16538-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="16538-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16538-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="16538-138">响应</span><span class="sxs-lookup"><span data-stu-id="16538-138">Response</span></span>

<span data-ttu-id="16538-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="16538-139">The following is an example of the response.</span></span>

><span data-ttu-id="16538-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="16538-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
