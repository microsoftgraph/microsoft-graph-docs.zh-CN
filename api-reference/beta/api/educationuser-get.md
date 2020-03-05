---
title: 获取 educationUser
description: 检索用户的属性和关系。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e2b63cd90478eb199d30137a171846fa2c832e2e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42423859"
---
# <a name="get-educationuser"></a><span data-ttu-id="fdb26-103">获取 educationUser</span><span class="sxs-lookup"><span data-stu-id="fdb26-103">Get educationUser</span></span>

<span data-ttu-id="fdb26-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="fdb26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdb26-105">检索用户的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fdb26-105">Retrieve the properties and relationships of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="fdb26-106">权限</span><span class="sxs-lookup"><span data-stu-id="fdb26-106">Permissions</span></span>

<span data-ttu-id="fdb26-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fdb26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fdb26-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fdb26-109">Permission type</span></span>                        | <span data-ttu-id="fdb26-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fdb26-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="fdb26-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fdb26-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fdb26-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="fdb26-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="fdb26-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fdb26-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdb26-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fdb26-114">Not supported.</span></span>                              |
| <span data-ttu-id="fdb26-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fdb26-115">Application</span></span>                            | <span data-ttu-id="fdb26-116">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdb26-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

>[!IMPORTANT]
><span data-ttu-id="fdb26-117">使用委派权限作用域时，Graph 将仅返回一组有限的属性`id`： `primaryRole`、 `accountEnabled`、 `displayName` `givenName` `surname` `userPrincipalName`、、、、 `userType`、 `onPremisesInfo`、。</span><span class="sxs-lookup"><span data-stu-id="fdb26-117">When using Delegated permission scopes, Graph will only return a limited set of properties: `id`, `primaryRole`, `accountEnabled`, `displayName`, `givenName`, `surname`, `userPrincipalName`, `userType`, `onPremisesInfo`.</span></span> <span data-ttu-id="fdb26-118">如果您的应用程序需要其他属性，则必须使用应用程序权限范围。</span><span class="sxs-lookup"><span data-stu-id="fdb26-118">If your application requires additional properties, you must use Application permission scopes.</span></span>

## <a name="http-request"></a><span data-ttu-id="fdb26-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fdb26-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/me
GET /education/users/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fdb26-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fdb26-120">Optional query parameters</span></span>

<span data-ttu-id="fdb26-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fdb26-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fdb26-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="fdb26-122">Request headers</span></span>

| <span data-ttu-id="fdb26-123">标头</span><span class="sxs-lookup"><span data-stu-id="fdb26-123">Header</span></span>        | <span data-ttu-id="fdb26-124">值</span><span class="sxs-lookup"><span data-stu-id="fdb26-124">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="fdb26-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdb26-125">Authorization</span></span> | <span data-ttu-id="fdb26-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fdb26-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fdb26-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fdb26-128">Request body</span></span>

<span data-ttu-id="fdb26-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fdb26-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdb26-130">响应</span><span class="sxs-lookup"><span data-stu-id="fdb26-130">Response</span></span>

<span data-ttu-id="fdb26-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fdb26-131">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdb26-132">示例</span><span class="sxs-lookup"><span data-stu-id="fdb26-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fdb26-133">请求</span><span class="sxs-lookup"><span data-stu-id="fdb26-133">Request</span></span>

<span data-ttu-id="fdb26-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fdb26-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fdb26-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="fdb26-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/users/13012
```

# <a name="c"></a>[<span data-ttu-id="fdb26-136">C#</span><span class="sxs-lookup"><span data-stu-id="fdb26-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fdb26-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fdb26-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fdb26-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fdb26-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fdb26-139">响应</span><span class="sxs-lookup"><span data-stu-id="fdb26-139">Response</span></span>

<span data-ttu-id="fdb26-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fdb26-140">The following is an example of the response.</span></span> 

><span data-ttu-id="fdb26-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fdb26-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
