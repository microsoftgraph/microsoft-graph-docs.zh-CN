---
title: 列出用户可传递的 memberOf
description: 获取用户所属的组、目录角色和管理单元。 此 API 请求是可传递的，并且还将返回用户是其嵌套成员的所有组。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c33210e42d3334feec8c1c06be162e673e3c3b94
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451754"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="3e809-104">列出用户可传递的 memberOf</span><span class="sxs-lookup"><span data-stu-id="3e809-104">List user transitive memberOf</span></span>

<span data-ttu-id="3e809-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3e809-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e809-106">获取用户所属的组、目录角色和管理单元。</span><span class="sxs-lookup"><span data-stu-id="3e809-106">Get groups, directory roles and administrative units that the user is a member of.</span></span> <span data-ttu-id="3e809-107">此 API 请求是可传递的，并且还将返回用户是其嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="3e809-107">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e809-108">权限</span><span class="sxs-lookup"><span data-stu-id="3e809-108">Permissions</span></span>

<span data-ttu-id="3e809-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e809-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e809-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e809-111">Permission type</span></span>      | <span data-ttu-id="3e809-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e809-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e809-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e809-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3e809-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3e809-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3e809-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e809-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e809-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e809-116">Not supported.</span></span>    |
|<span data-ttu-id="3e809-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e809-117">Application</span></span> | <span data-ttu-id="3e809-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e809-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="3e809-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e809-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3e809-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3e809-120">Optional query parameters</span></span>

<span data-ttu-id="3e809-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3e809-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e809-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e809-122">Request headers</span></span>

| <span data-ttu-id="3e809-123">标头</span><span class="sxs-lookup"><span data-stu-id="3e809-123">Header</span></span>       | <span data-ttu-id="3e809-124">值</span><span class="sxs-lookup"><span data-stu-id="3e809-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3e809-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e809-125">Authorization</span></span>  | <span data-ttu-id="3e809-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3e809-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3e809-128">接受</span><span class="sxs-lookup"><span data-stu-id="3e809-128">Accept</span></span>  | <span data-ttu-id="3e809-129">application/json</span><span class="sxs-lookup"><span data-stu-id="3e809-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e809-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e809-130">Request body</span></span>

<span data-ttu-id="3e809-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3e809-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e809-132">响应</span><span class="sxs-lookup"><span data-stu-id="3e809-132">Response</span></span>

<span data-ttu-id="3e809-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3e809-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e809-134">示例</span><span class="sxs-lookup"><span data-stu-id="3e809-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e809-135">请求</span><span class="sxs-lookup"><span data-stu-id="3e809-135">Request</span></span>

<span data-ttu-id="3e809-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3e809-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3e809-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e809-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="3e809-138">C#</span><span class="sxs-lookup"><span data-stu-id="3e809-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3e809-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e809-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3e809-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e809-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3e809-141">响应</span><span class="sxs-lookup"><span data-stu-id="3e809-141">Response</span></span>

<span data-ttu-id="3e809-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3e809-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
