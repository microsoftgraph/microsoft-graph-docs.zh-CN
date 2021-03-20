---
title: 获取 educationUser
description: 检索用户的属性和关系。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6ad690ccb21d49196ee52cf69f9832d87b7a6a7c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951148"
---
# <a name="get-educationuser"></a><span data-ttu-id="90f74-103">获取 educationUser</span><span class="sxs-lookup"><span data-stu-id="90f74-103">Get educationUser</span></span>

<span data-ttu-id="90f74-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90f74-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90f74-105">检索用户的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="90f74-105">Retrieve the properties and relationships of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="90f74-106">权限</span><span class="sxs-lookup"><span data-stu-id="90f74-106">Permissions</span></span>

<span data-ttu-id="90f74-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90f74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> [!NOTE]
> <span data-ttu-id="90f74-109">如果使用委派令牌，成员只能看到有关其自己的帐户的信息。</span><span class="sxs-lookup"><span data-stu-id="90f74-109">If the delegated token is used, members can only see information about their own account.</span></span> <span data-ttu-id="90f74-110">在这种情况下，使用 `beta/education/me/users` 资源。</span><span class="sxs-lookup"><span data-stu-id="90f74-110">Use the `beta/education/me/users` resource in this case.</span></span>

| <span data-ttu-id="90f74-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="90f74-111">Permission type</span></span>                        | <span data-ttu-id="90f74-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="90f74-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="90f74-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90f74-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="90f74-114">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="90f74-114">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="90f74-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90f74-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90f74-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="90f74-116">Not supported.</span></span>                              |
| <span data-ttu-id="90f74-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="90f74-117">Application</span></span>                            | <span data-ttu-id="90f74-118">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90f74-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

> [!IMPORTANT]
> <span data-ttu-id="90f74-119">使用委派权限范围时，Graph 将仅返回一组有限的属性 `id` `primaryRole` `accountEnabled` `displayName` `givenName` `surname` `userPrincipalName` `userType` `onPremisesInfo` `student/externalId` `teacher/externalId` ：、。</span><span class="sxs-lookup"><span data-stu-id="90f74-119">When using Delegated permission scopes, Graph will only return a limited set of properties: `id`, `primaryRole`, `accountEnabled`, `displayName`, `givenName`, `surname`, `userPrincipalName`, `userType`, `onPremisesInfo`, `student/externalId`, `teacher/externalId`.</span></span> <span data-ttu-id="90f74-120">如果应用程序需要其他属性，则必须使用应用程序权限范围。</span><span class="sxs-lookup"><span data-stu-id="90f74-120">If your application requires additional properties, you must use Application permission scopes.</span></span>

## <a name="http-request"></a><span data-ttu-id="90f74-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90f74-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me
GET /education/users/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="90f74-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="90f74-122">Optional query parameters</span></span>

<span data-ttu-id="90f74-123">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="90f74-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="90f74-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="90f74-124">Request headers</span></span>

| <span data-ttu-id="90f74-125">标头</span><span class="sxs-lookup"><span data-stu-id="90f74-125">Header</span></span>        | <span data-ttu-id="90f74-126">值</span><span class="sxs-lookup"><span data-stu-id="90f74-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="90f74-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="90f74-127">Authorization</span></span> | <span data-ttu-id="90f74-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="90f74-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90f74-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="90f74-130">Request body</span></span>

<span data-ttu-id="90f74-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="90f74-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90f74-132">响应</span><span class="sxs-lookup"><span data-stu-id="90f74-132">Response</span></span>

<span data-ttu-id="90f74-133">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="90f74-133">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90f74-134">示例</span><span class="sxs-lookup"><span data-stu-id="90f74-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="90f74-135">请求</span><span class="sxs-lookup"><span data-stu-id="90f74-135">Request</span></span>

<span data-ttu-id="90f74-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="90f74-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="90f74-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="90f74-137">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_educationuser_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/users/13012
```

# <a name="c"></a>[<span data-ttu-id="90f74-138">C#</span><span class="sxs-lookup"><span data-stu-id="90f74-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-2-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90f74-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90f74-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-2-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90f74-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90f74-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-2-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90f74-141">Java</span><span class="sxs-lookup"><span data-stu-id="90f74-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationuser-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="90f74-142">响应</span><span class="sxs-lookup"><span data-stu-id="90f74-142">Response</span></span>

<span data-ttu-id="90f74-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="90f74-143">The following is an example of the response.</span></span>

> <span data-ttu-id="90f74-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="90f74-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
