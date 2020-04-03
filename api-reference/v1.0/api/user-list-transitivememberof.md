---
title: 列出用户可传递的 memberOf
description: 获取用户所属的组和目录角色。 此 API 请求是可传递的，并且还将返回用户是其嵌套成员的所有组。
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: caee8bd1c849d7ac38562ace7e39541810de11aa
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108716"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="1157e-104">列出用户可传递的 memberOf</span><span class="sxs-lookup"><span data-stu-id="1157e-104">List user transitive memberOf</span></span>

<span data-ttu-id="1157e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1157e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1157e-106">获取用户所属的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="1157e-106">Get groups, directory roles that the user is a member of.</span></span> <span data-ttu-id="1157e-107">此 API 请求是可传递的，并且还将返回用户是其嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="1157e-107">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="1157e-108">权限</span><span class="sxs-lookup"><span data-stu-id="1157e-108">Permissions</span></span>

<span data-ttu-id="1157e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1157e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1157e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1157e-111">Permission type</span></span>      | <span data-ttu-id="1157e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1157e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1157e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1157e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1157e-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1157e-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1157e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1157e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1157e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1157e-116">Not supported.</span></span>    |
|<span data-ttu-id="1157e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1157e-117">Application</span></span> | <span data-ttu-id="1157e-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1157e-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="1157e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1157e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1157e-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1157e-120">Optional query parameters</span></span>

<span data-ttu-id="1157e-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1157e-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1157e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1157e-122">Request headers</span></span>

| <span data-ttu-id="1157e-123">标头</span><span class="sxs-lookup"><span data-stu-id="1157e-123">Header</span></span>       | <span data-ttu-id="1157e-124">值</span><span class="sxs-lookup"><span data-stu-id="1157e-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1157e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1157e-125">Authorization</span></span>  | <span data-ttu-id="1157e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1157e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1157e-128">接受</span><span class="sxs-lookup"><span data-stu-id="1157e-128">Accept</span></span>  | <span data-ttu-id="1157e-129">application/json</span><span class="sxs-lookup"><span data-stu-id="1157e-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1157e-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="1157e-130">Request body</span></span>

<span data-ttu-id="1157e-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1157e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1157e-132">响应</span><span class="sxs-lookup"><span data-stu-id="1157e-132">Response</span></span>

<span data-ttu-id="1157e-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1157e-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1157e-134">示例</span><span class="sxs-lookup"><span data-stu-id="1157e-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="1157e-135">请求</span><span class="sxs-lookup"><span data-stu-id="1157e-135">Request</span></span>

<span data-ttu-id="1157e-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1157e-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1157e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="1157e-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="1157e-138">C#</span><span class="sxs-lookup"><span data-stu-id="1157e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1157e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1157e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1157e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1157e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1157e-141">Java</span><span class="sxs-lookup"><span data-stu-id="1157e-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1157e-142">响应</span><span class="sxs-lookup"><span data-stu-id="1157e-142">Response</span></span>

<span data-ttu-id="1157e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1157e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
