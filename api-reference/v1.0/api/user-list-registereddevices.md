---
title: List registeredDevices
description: 获取用户的注册设备列表。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b53b3311a28ea8edc49c3119f64fcd8757dd4cc9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509029"
---
# <a name="list-registereddevices"></a><span data-ttu-id="dd5a9-103">List registeredDevices</span><span class="sxs-lookup"><span data-stu-id="dd5a9-103">List registeredDevices</span></span>

<span data-ttu-id="dd5a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd5a9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd5a9-105">获取用户的注册设备列表。</span><span class="sxs-lookup"><span data-stu-id="dd5a9-105">Get the list of user's registered devices.</span></span>
## <a name="permissions"></a><span data-ttu-id="dd5a9-106">权限</span><span class="sxs-lookup"><span data-stu-id="dd5a9-106">Permissions</span></span>
<span data-ttu-id="dd5a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd5a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd5a9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd5a9-109">Permission type</span></span>      | <span data-ttu-id="dd5a9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dd5a9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd5a9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd5a9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dd5a9-112">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dd5a9-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dd5a9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd5a9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd5a9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd5a9-114">Not supported.</span></span>    |
|<span data-ttu-id="dd5a9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd5a9-115">Application</span></span> | <span data-ttu-id="dd5a9-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd5a9-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="dd5a9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd5a9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/registeredDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dd5a9-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dd5a9-118">Optional query parameters</span></span>
<span data-ttu-id="dd5a9-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dd5a9-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="dd5a9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd5a9-120">Request headers</span></span>
| <span data-ttu-id="dd5a9-121">标头</span><span class="sxs-lookup"><span data-stu-id="dd5a9-121">Header</span></span>       | <span data-ttu-id="dd5a9-122">值</span><span class="sxs-lookup"><span data-stu-id="dd5a9-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dd5a9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd5a9-123">Authorization</span></span>  | <span data-ttu-id="dd5a9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dd5a9-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dd5a9-126">接受</span><span class="sxs-lookup"><span data-stu-id="dd5a9-126">Accept</span></span>  | <span data-ttu-id="dd5a9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="dd5a9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd5a9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd5a9-128">Request body</span></span>
<span data-ttu-id="dd5a9-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dd5a9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd5a9-130">响应</span><span class="sxs-lookup"><span data-stu-id="dd5a9-130">Response</span></span>

<span data-ttu-id="dd5a9-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dd5a9-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dd5a9-132">示例</span><span class="sxs-lookup"><span data-stu-id="dd5a9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd5a9-133">请求</span><span class="sxs-lookup"><span data-stu-id="dd5a9-133">Request</span></span>
<span data-ttu-id="dd5a9-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dd5a9-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd5a9-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd5a9-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registereddevices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/registeredDevices
```
# <a name="c"></a>[<span data-ttu-id="dd5a9-136">C#</span><span class="sxs-lookup"><span data-stu-id="dd5a9-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registereddevices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd5a9-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd5a9-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registereddevices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd5a9-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd5a9-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registereddevices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd5a9-139">Java</span><span class="sxs-lookup"><span data-stu-id="dd5a9-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registereddevices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dd5a9-140">响应</span><span class="sxs-lookup"><span data-stu-id="dd5a9-140">Response</span></span>
<span data-ttu-id="dd5a9-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dd5a9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List registeredDevices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
