---
title: 列出学校
description: 检索用户所在的学校列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0d05b881f3646b16913edf349af2c8fba6e3a8cb
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48403268"
---
# <a name="list-schools"></a><span data-ttu-id="d553a-103">列出学校</span><span class="sxs-lookup"><span data-stu-id="d553a-103">List schools</span></span>

<span data-ttu-id="d553a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d553a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d553a-105">检索用户所在的学校列表。</span><span class="sxs-lookup"><span data-stu-id="d553a-105">Retrieve a list of schools for a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="d553a-106">权限</span><span class="sxs-lookup"><span data-stu-id="d553a-106">Permissions</span></span>

<span data-ttu-id="d553a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d553a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d553a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d553a-109">Permission type</span></span>                        | <span data-ttu-id="d553a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d553a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="d553a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d553a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d553a-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="d553a-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="d553a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d553a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d553a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d553a-114">Not supported.</span></span>                              |
| <span data-ttu-id="d553a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d553a-115">Application</span></span>                            | <span data-ttu-id="d553a-116">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d553a-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="d553a-117">使用委派权限时，将仅返回身份验证用户为其成员的 educationSchool 资源。</span><span class="sxs-lookup"><span data-stu-id="d553a-117">When delegated permissions are used, only educationSchool resources that the authentication user is a member will be returned.</span></span>

## <a name="http-request"></a><span data-ttu-id="d553a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d553a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/schools
GET /education/users/{id}/schools
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d553a-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d553a-119">Optional query parameters</span></span>

<span data-ttu-id="d553a-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d553a-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d553a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d553a-121">Request headers</span></span>

| <span data-ttu-id="d553a-122">标头</span><span class="sxs-lookup"><span data-stu-id="d553a-122">Header</span></span>        | <span data-ttu-id="d553a-123">值</span><span class="sxs-lookup"><span data-stu-id="d553a-123">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="d553a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d553a-124">Authorization</span></span> | <span data-ttu-id="d553a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d553a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d553a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d553a-127">Request body</span></span>

<span data-ttu-id="d553a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d553a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d553a-129">响应</span><span class="sxs-lookup"><span data-stu-id="d553a-129">Response</span></span>

<span data-ttu-id="d553a-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationSchool](../resources/educationschool.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="d553a-130">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d553a-131">示例</span><span class="sxs-lookup"><span data-stu-id="d553a-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d553a-132">请求</span><span class="sxs-lookup"><span data-stu-id="d553a-132">Request</span></span>

<span data-ttu-id="d553a-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d553a-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d553a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d553a-134">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/schools
```

# <a name="c"></a>[<span data-ttu-id="d553a-135">C#</span><span class="sxs-lookup"><span data-stu-id="d553a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d553a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d553a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d553a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d553a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d553a-138">响应</span><span class="sxs-lookup"><span data-stu-id="d553a-138">Response</span></span>

<span data-ttu-id="d553a-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d553a-139">The following is an example of the response.</span></span>

> <span data-ttu-id="d553a-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d553a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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