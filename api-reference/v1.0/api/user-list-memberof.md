---
title: 列出 memberOf
description: '返回用户是其直接成员的组和目录角色。 '
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9b323c81d471fc36da58ee0748c66ca7b9ec573d
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728998"
---
# <a name="list-memberof"></a><span data-ttu-id="0a862-103">列出 memberOf</span><span class="sxs-lookup"><span data-stu-id="0a862-103">List memberOf</span></span>

<span data-ttu-id="0a862-104">获取用户是其直接成员的[组](../resources/group.md)和[目录角色](../resources/directoryrole.md)。</span><span class="sxs-lookup"><span data-stu-id="0a862-104">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="0a862-105">权限</span><span class="sxs-lookup"><span data-stu-id="0a862-105">Permissions</span></span>
<span data-ttu-id="0a862-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a862-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a862-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a862-108">Permission type</span></span>      | <span data-ttu-id="0a862-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0a862-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a862-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a862-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0a862-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0a862-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0a862-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a862-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a862-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a862-113">Not supported.</span></span>    |
|<span data-ttu-id="0a862-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a862-114">Application</span></span> | <span data-ttu-id="0a862-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a862-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a862-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a862-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0a862-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0a862-117">Optional query parameters</span></span>
<span data-ttu-id="0a862-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0a862-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="0a862-119">$filter 不受支持。</span><span class="sxs-lookup"><span data-stu-id="0a862-119">$filter is not supported.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="0a862-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a862-120">Request headers</span></span>
| <span data-ttu-id="0a862-121">标头</span><span class="sxs-lookup"><span data-stu-id="0a862-121">Header</span></span>       | <span data-ttu-id="0a862-122">值</span><span class="sxs-lookup"><span data-stu-id="0a862-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0a862-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a862-123">Authorization</span></span>  | <span data-ttu-id="0a862-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0a862-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0a862-126">接受</span><span class="sxs-lookup"><span data-stu-id="0a862-126">Accept</span></span>  | <span data-ttu-id="0a862-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0a862-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a862-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a862-128">Request body</span></span>
<span data-ttu-id="0a862-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0a862-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a862-130">响应</span><span class="sxs-lookup"><span data-stu-id="0a862-130">Response</span></span>

<span data-ttu-id="0a862-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0a862-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0a862-132">示例</span><span class="sxs-lookup"><span data-stu-id="0a862-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a862-133">请求</span><span class="sxs-lookup"><span data-stu-id="0a862-133">Request</span></span>
<span data-ttu-id="0a862-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0a862-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0a862-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a862-135">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/memberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0a862-136">C#</span><span class="sxs-lookup"><span data-stu-id="0a862-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a862-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a862-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0a862-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a862-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0a862-139">Java</span><span class="sxs-lookup"><span data-stu-id="0a862-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0a862-140">响应</span><span class="sxs-lookup"><span data-stu-id="0a862-140">Response</span></span>
<span data-ttu-id="0a862-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0a862-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
