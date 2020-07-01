---
title: 获取 educationUser
description: 检索用户的属性和关系。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c2def2d5df4f2ae8d3c2d0656a1149a050b6fbe6
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006764"
---
# <a name="get-educationuser"></a><span data-ttu-id="fcde0-103">获取 educationUser</span><span class="sxs-lookup"><span data-stu-id="fcde0-103">Get educationUser</span></span>

<span data-ttu-id="fcde0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcde0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcde0-105">检索用户的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fcde0-105">Retrieve the properties and relationships of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="fcde0-106">权限</span><span class="sxs-lookup"><span data-stu-id="fcde0-106">Permissions</span></span>

<span data-ttu-id="fcde0-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="fcde0-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="fcde0-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcde0-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> [!NOTE]
> <span data-ttu-id="fcde0-109">如果使用委派的令牌，则成员只能查看有关其自己的帐户的信息。</span><span class="sxs-lookup"><span data-stu-id="fcde0-109">If the delegated token is used, members can only see information about their own account.</span></span> <span data-ttu-id="fcde0-110">在这种情况下，使用 `beta/education/me/users` 资源。</span><span class="sxs-lookup"><span data-stu-id="fcde0-110">Use the `beta/education/me/users` resource in this case.</span></span>

| <span data-ttu-id="fcde0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fcde0-111">Permission type</span></span>                        | <span data-ttu-id="fcde0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fcde0-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="fcde0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fcde0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="fcde0-114">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="fcde0-114">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="fcde0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fcde0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcde0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fcde0-116">Not supported.</span></span>                              |
| <span data-ttu-id="fcde0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fcde0-117">Application</span></span>                            | <span data-ttu-id="fcde0-118">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcde0-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

> [!IMPORTANT]
> <span data-ttu-id="fcde0-119">使用委派权限作用域时，Graph 将仅返回一组有限的属性：、、、、、、、、、、 `id` `primaryRole` `accountEnabled` `displayName` `givenName` `surname` `userPrincipalName` `userType` `onPremisesInfo` `student/externalId` `teacher/externalId` 。</span><span class="sxs-lookup"><span data-stu-id="fcde0-119">When using Delegated permission scopes, Graph will only return a limited set of properties: `id`, `primaryRole`, `accountEnabled`, `displayName`, `givenName`, `surname`, `userPrincipalName`, `userType`, `onPremisesInfo`, `student/externalId`, `teacher/externalId`.</span></span> <span data-ttu-id="fcde0-120">如果您的应用程序需要其他属性，则必须使用应用程序权限范围。</span><span class="sxs-lookup"><span data-stu-id="fcde0-120">If your application requires additional properties, you must use Application permission scopes.</span></span>

## <a name="http-request"></a><span data-ttu-id="fcde0-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fcde0-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me
GET /education/users/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fcde0-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fcde0-122">Optional query parameters</span></span>

<span data-ttu-id="fcde0-123">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fcde0-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fcde0-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="fcde0-124">Request headers</span></span>

| <span data-ttu-id="fcde0-125">标头</span><span class="sxs-lookup"><span data-stu-id="fcde0-125">Header</span></span>        | <span data-ttu-id="fcde0-126">值</span><span class="sxs-lookup"><span data-stu-id="fcde0-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="fcde0-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcde0-127">Authorization</span></span> | <span data-ttu-id="fcde0-128">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="fcde0-128">Bearer {token}.</span></span> <span data-ttu-id="fcde0-129">Required.</span><span class="sxs-lookup"><span data-stu-id="fcde0-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fcde0-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="fcde0-130">Request body</span></span>

<span data-ttu-id="fcde0-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fcde0-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcde0-132">响应</span><span class="sxs-lookup"><span data-stu-id="fcde0-132">Response</span></span>

<span data-ttu-id="fcde0-133">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fcde0-133">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcde0-134">示例</span><span class="sxs-lookup"><span data-stu-id="fcde0-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fcde0-135">请求</span><span class="sxs-lookup"><span data-stu-id="fcde0-135">Request</span></span>

<span data-ttu-id="fcde0-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fcde0-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fcde0-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="fcde0-137">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/users/13012
```

# <a name="c"></a>[<span data-ttu-id="fcde0-138">C#</span><span class="sxs-lookup"><span data-stu-id="fcde0-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fcde0-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fcde0-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fcde0-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fcde0-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fcde0-141">响应</span><span class="sxs-lookup"><span data-stu-id="fcde0-141">Response</span></span>

<span data-ttu-id="fcde0-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fcde0-142">The following is an example of the response.</span></span>

> <span data-ttu-id="fcde0-143">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="fcde0-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fcde0-144">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="fcde0-144">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 508

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
  },
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
