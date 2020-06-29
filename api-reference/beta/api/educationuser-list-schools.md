---
title: 列出学校
description: 检索用户所在的学校列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b010d56f52080e54383e1b89553060780da63cc0
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909602"
---
# <a name="list-schools"></a><span data-ttu-id="1a856-103">列出学校</span><span class="sxs-lookup"><span data-stu-id="1a856-103">List schools</span></span>

<span data-ttu-id="1a856-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a856-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a856-105">检索用户所在的学校列表。</span><span class="sxs-lookup"><span data-stu-id="1a856-105">Retrieve a list of schools for a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a856-106">权限</span><span class="sxs-lookup"><span data-stu-id="1a856-106">Permissions</span></span>

<span data-ttu-id="1a856-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="1a856-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1a856-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a856-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a856-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a856-109">Permission type</span></span>                        | <span data-ttu-id="1a856-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a856-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="1a856-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a856-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a856-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="1a856-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="1a856-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a856-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a856-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a856-114">Not supported.</span></span>                              |
| <span data-ttu-id="1a856-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a856-115">Application</span></span>                            | <span data-ttu-id="1a856-116">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a856-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="1a856-117">使用委派权限时，将仅返回身份验证用户为其成员的 educationSchool 资源。</span><span class="sxs-lookup"><span data-stu-id="1a856-117">When delegated permissions are used, only educationSchool resources that the authentication user is a member will be returned.</span></span>

## <a name="http-request"></a><span data-ttu-id="1a856-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a856-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/schools
GET /education/users/{id}/schools
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a856-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1a856-119">Optional query parameters</span></span>

<span data-ttu-id="1a856-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1a856-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a856-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a856-121">Request headers</span></span>

| <span data-ttu-id="1a856-122">标头</span><span class="sxs-lookup"><span data-stu-id="1a856-122">Header</span></span>        | <span data-ttu-id="1a856-123">值</span><span class="sxs-lookup"><span data-stu-id="1a856-123">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="1a856-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a856-124">Authorization</span></span> | <span data-ttu-id="1a856-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="1a856-125">Bearer {token}.</span></span> <span data-ttu-id="1a856-126">Required.</span><span class="sxs-lookup"><span data-stu-id="1a856-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a856-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a856-127">Request body</span></span>

<span data-ttu-id="1a856-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1a856-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a856-129">响应</span><span class="sxs-lookup"><span data-stu-id="1a856-129">Response</span></span>

<span data-ttu-id="1a856-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationSchool](../resources/educationschool.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="1a856-130">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a856-131">示例</span><span class="sxs-lookup"><span data-stu-id="1a856-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1a856-132">请求</span><span class="sxs-lookup"><span data-stu-id="1a856-132">Request</span></span>

<span data-ttu-id="1a856-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1a856-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a856-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a856-134">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/schools
```

# <a name="c"></a>[<span data-ttu-id="1a856-135">C#</span><span class="sxs-lookup"><span data-stu-id="1a856-135">C#</span></span>](#tab/csharp)

[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a856-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a856-136">JavaScript</span></span>](#tab/javascript)

[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a856-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a856-137">Objective-C</span></span>](#tab/objc)

[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1a856-138">响应</span><span class="sxs-lookup"><span data-stu-id="1a856-138">Response</span></span>

<span data-ttu-id="1a856-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1a856-139">The following is an example of the response.</span></span>

> <span data-ttu-id="1a856-140">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="1a856-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1a856-141">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="1a856-141">All the properties will be returned from an actual call.</span></span>

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
