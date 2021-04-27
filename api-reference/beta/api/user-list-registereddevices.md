---
title: List registeredDevices
description: 获取用户的注册设备列表。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: e11b39156f7a1c2a6f807c19b6ee474ca6113cbb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048874"
---
# <a name="list-registereddevices"></a><span data-ttu-id="05e3d-103">List registeredDevices</span><span class="sxs-lookup"><span data-stu-id="05e3d-103">List registeredDevices</span></span>

<span data-ttu-id="05e3d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05e3d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05e3d-105">获取用户的注册设备列表。</span><span class="sxs-lookup"><span data-stu-id="05e3d-105">Get the list of user's registered devices.</span></span>
## <a name="permissions"></a><span data-ttu-id="05e3d-106">权限</span><span class="sxs-lookup"><span data-stu-id="05e3d-106">Permissions</span></span>
<span data-ttu-id="05e3d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05e3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05e3d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="05e3d-109">Permission type</span></span>      | <span data-ttu-id="05e3d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="05e3d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05e3d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05e3d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="05e3d-112">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="05e3d-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="05e3d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05e3d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05e3d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="05e3d-114">Not supported.</span></span>    |
|<span data-ttu-id="05e3d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="05e3d-115">Application</span></span> | <span data-ttu-id="05e3d-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05e3d-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="05e3d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05e3d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/registeredDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="05e3d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="05e3d-118">Optional query parameters</span></span>
<span data-ttu-id="05e3d-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="05e3d-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="05e3d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="05e3d-120">Request headers</span></span>
| <span data-ttu-id="05e3d-121">标头</span><span class="sxs-lookup"><span data-stu-id="05e3d-121">Header</span></span>       | <span data-ttu-id="05e3d-122">值</span><span class="sxs-lookup"><span data-stu-id="05e3d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="05e3d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="05e3d-123">Authorization</span></span>  | <span data-ttu-id="05e3d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="05e3d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="05e3d-126">接受</span><span class="sxs-lookup"><span data-stu-id="05e3d-126">Accept</span></span>  | <span data-ttu-id="05e3d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="05e3d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05e3d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="05e3d-128">Request body</span></span>
<span data-ttu-id="05e3d-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="05e3d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05e3d-130">响应</span><span class="sxs-lookup"><span data-stu-id="05e3d-130">Response</span></span>

<span data-ttu-id="05e3d-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="05e3d-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="05e3d-132">示例</span><span class="sxs-lookup"><span data-stu-id="05e3d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="05e3d-133">请求</span><span class="sxs-lookup"><span data-stu-id="05e3d-133">Request</span></span>
<span data-ttu-id="05e3d-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="05e3d-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="05e3d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="05e3d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registereddevices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/registeredDevices
```
# <a name="c"></a>[<span data-ttu-id="05e3d-136">C#</span><span class="sxs-lookup"><span data-stu-id="05e3d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registereddevices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="05e3d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05e3d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registereddevices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05e3d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05e3d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registereddevices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="05e3d-139">Java</span><span class="sxs-lookup"><span data-stu-id="05e3d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registereddevices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="05e3d-140">响应</span><span class="sxs-lookup"><span data-stu-id="05e3d-140">Response</span></span>
<span data-ttu-id="05e3d-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="05e3d-141">Here is an example of the response.</span></span> <span data-ttu-id="05e3d-142">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="05e3d-142">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List registeredDevices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
