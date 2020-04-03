---
title: 列出 memberOf
description: '返回用户是其直接成员的组和目录角色。 '
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: dd2d649eceeb5b06c863bc8783a214b50eae0f91
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108786"
---
# <a name="list-memberof"></a><span data-ttu-id="72d9b-103">列出 memberOf</span><span class="sxs-lookup"><span data-stu-id="72d9b-103">List memberOf</span></span>

<span data-ttu-id="72d9b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72d9b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="72d9b-105">获取用户是其直接成员的[组](../resources/group.md)和[目录角色](../resources/directoryrole.md)。</span><span class="sxs-lookup"><span data-stu-id="72d9b-105">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="72d9b-106">权限</span><span class="sxs-lookup"><span data-stu-id="72d9b-106">Permissions</span></span>
<span data-ttu-id="72d9b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72d9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72d9b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="72d9b-109">Permission type</span></span>      | <span data-ttu-id="72d9b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="72d9b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72d9b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72d9b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="72d9b-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="72d9b-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="72d9b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72d9b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72d9b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="72d9b-114">Not supported.</span></span>    |
|<span data-ttu-id="72d9b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="72d9b-115">Application</span></span> | <span data-ttu-id="72d9b-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72d9b-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="72d9b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72d9b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="72d9b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="72d9b-118">Optional query parameters</span></span>
<span data-ttu-id="72d9b-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="72d9b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="72d9b-120">$filter 不受支持。</span><span class="sxs-lookup"><span data-stu-id="72d9b-120">$filter is not supported.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="72d9b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="72d9b-121">Request headers</span></span>
| <span data-ttu-id="72d9b-122">标头</span><span class="sxs-lookup"><span data-stu-id="72d9b-122">Header</span></span>       | <span data-ttu-id="72d9b-123">值</span><span class="sxs-lookup"><span data-stu-id="72d9b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="72d9b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="72d9b-124">Authorization</span></span>  | <span data-ttu-id="72d9b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="72d9b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="72d9b-127">接受</span><span class="sxs-lookup"><span data-stu-id="72d9b-127">Accept</span></span>  | <span data-ttu-id="72d9b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="72d9b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72d9b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="72d9b-129">Request body</span></span>
<span data-ttu-id="72d9b-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="72d9b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72d9b-131">响应</span><span class="sxs-lookup"><span data-stu-id="72d9b-131">Response</span></span>

<span data-ttu-id="72d9b-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="72d9b-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="72d9b-133">示例</span><span class="sxs-lookup"><span data-stu-id="72d9b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72d9b-134">请求</span><span class="sxs-lookup"><span data-stu-id="72d9b-134">Request</span></span>
<span data-ttu-id="72d9b-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="72d9b-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72d9b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="72d9b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/memberOf
```
# <a name="c"></a>[<span data-ttu-id="72d9b-137">C#</span><span class="sxs-lookup"><span data-stu-id="72d9b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72d9b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72d9b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72d9b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72d9b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72d9b-140">Java</span><span class="sxs-lookup"><span data-stu-id="72d9b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="72d9b-141">响应</span><span class="sxs-lookup"><span data-stu-id="72d9b-141">Response</span></span>
<span data-ttu-id="72d9b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="72d9b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
