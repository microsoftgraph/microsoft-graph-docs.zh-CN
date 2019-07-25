---
title: List registeredDevices
description: 获取用户的注册设备列表。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 00548dd85279ebb9aeb9c99c3772abfbb70c964b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882846"
---
# <a name="list-registereddevices"></a><span data-ttu-id="1f2d6-103">List registeredDevices</span><span class="sxs-lookup"><span data-stu-id="1f2d6-103">List registeredDevices</span></span>

<span data-ttu-id="1f2d6-104">获取用户的注册设备列表。</span><span class="sxs-lookup"><span data-stu-id="1f2d6-104">Get the list of user's registered devices.</span></span>
## <a name="permissions"></a><span data-ttu-id="1f2d6-105">权限</span><span class="sxs-lookup"><span data-stu-id="1f2d6-105">Permissions</span></span>
<span data-ttu-id="1f2d6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1f2d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f2d6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f2d6-108">Permission type</span></span>      | <span data-ttu-id="1f2d6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1f2d6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f2d6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f2d6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1f2d6-111">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1f2d6-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1f2d6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f2d6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f2d6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f2d6-113">Not supported.</span></span>    |
|<span data-ttu-id="1f2d6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f2d6-114">Application</span></span> | <span data-ttu-id="1f2d6-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f2d6-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f2d6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f2d6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/registeredDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1f2d6-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1f2d6-117">Optional query parameters</span></span>
<span data-ttu-id="1f2d6-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1f2d6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1f2d6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f2d6-119">Request headers</span></span>
| <span data-ttu-id="1f2d6-120">标头</span><span class="sxs-lookup"><span data-stu-id="1f2d6-120">Header</span></span>       | <span data-ttu-id="1f2d6-121">值</span><span class="sxs-lookup"><span data-stu-id="1f2d6-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1f2d6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f2d6-122">Authorization</span></span>  | <span data-ttu-id="1f2d6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1f2d6-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1f2d6-125">接受</span><span class="sxs-lookup"><span data-stu-id="1f2d6-125">Accept</span></span>  | <span data-ttu-id="1f2d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1f2d6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f2d6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f2d6-127">Request body</span></span>
<span data-ttu-id="1f2d6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1f2d6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f2d6-129">响应</span><span class="sxs-lookup"><span data-stu-id="1f2d6-129">Response</span></span>

<span data-ttu-id="1f2d6-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1f2d6-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1f2d6-131">示例</span><span class="sxs-lookup"><span data-stu-id="1f2d6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f2d6-132">请求</span><span class="sxs-lookup"><span data-stu-id="1f2d6-132">Request</span></span>
<span data-ttu-id="1f2d6-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1f2d6-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1f2d6-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="1f2d6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registereddevices"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/registeredDevices
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1f2d6-135">C#</span><span class="sxs-lookup"><span data-stu-id="1f2d6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registereddevices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1f2d6-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="1f2d6-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registereddevices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1f2d6-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="1f2d6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registereddevices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1f2d6-138">Java</span><span class="sxs-lookup"><span data-stu-id="1f2d6-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registereddevices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1f2d6-139">响应</span><span class="sxs-lookup"><span data-stu-id="1f2d6-139">Response</span></span>
<span data-ttu-id="1f2d6-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1f2d6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
