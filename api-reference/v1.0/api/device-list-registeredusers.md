---
title: 列出 registeredUser
description: 检索已注册为设备用户的用户列表。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 37b42c80f483fa8ccd2aeefb70f01ba46b4be349
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721339"
---
# <a name="list-registeredusers"></a><span data-ttu-id="db5cf-103">列出 registeredUser</span><span class="sxs-lookup"><span data-stu-id="db5cf-103">List registeredUsers</span></span>

<span data-ttu-id="db5cf-104">检索已注册为设备用户的用户列表。</span><span class="sxs-lookup"><span data-stu-id="db5cf-104">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="db5cf-105">对于云加入设备和已注册的个人设备，已注册用户在设备注册时设置为与已注册所有者相同的值。</span><span class="sxs-lookup"><span data-stu-id="db5cf-105">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="db5cf-106">权限</span><span class="sxs-lookup"><span data-stu-id="db5cf-106">Permissions</span></span>
<span data-ttu-id="db5cf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db5cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="db5cf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="db5cf-109">Permission type</span></span>      | <span data-ttu-id="db5cf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db5cf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db5cf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db5cf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="db5cf-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="db5cf-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="db5cf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db5cf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db5cf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="db5cf-114">Not supported.</span></span>    |
|<span data-ttu-id="db5cf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="db5cf-115">Application</span></span> | <span data-ttu-id="db5cf-116">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db5cf-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db5cf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db5cf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="db5cf-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="db5cf-118">Optional query parameters</span></span>
<span data-ttu-id="db5cf-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="db5cf-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="db5cf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="db5cf-120">Request headers</span></span>
| <span data-ttu-id="db5cf-121">名称</span><span class="sxs-lookup"><span data-stu-id="db5cf-121">Name</span></span>       | <span data-ttu-id="db5cf-122">类型</span><span class="sxs-lookup"><span data-stu-id="db5cf-122">Type</span></span> | <span data-ttu-id="db5cf-123">说明</span><span class="sxs-lookup"><span data-stu-id="db5cf-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="db5cf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="db5cf-124">Authorization</span></span>  | <span data-ttu-id="db5cf-125">string</span><span class="sxs-lookup"><span data-stu-id="db5cf-125">string</span></span>  | <span data-ttu-id="db5cf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="db5cf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db5cf-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="db5cf-128">Request body</span></span>
<span data-ttu-id="db5cf-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="db5cf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db5cf-130">响应</span><span class="sxs-lookup"><span data-stu-id="db5cf-130">Response</span></span>

<span data-ttu-id="db5cf-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="db5cf-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="db5cf-132">示例</span><span class="sxs-lookup"><span data-stu-id="db5cf-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db5cf-133">请求</span><span class="sxs-lookup"><span data-stu-id="db5cf-133">Request</span></span>
<span data-ttu-id="db5cf-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db5cf-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="db5cf-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="db5cf-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db5cf-136">C#</span><span class="sxs-lookup"><span data-stu-id="db5cf-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db5cf-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db5cf-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db5cf-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="db5cf-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="db5cf-139">Java</span><span class="sxs-lookup"><span data-stu-id="db5cf-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="db5cf-140">响应</span><span class="sxs-lookup"><span data-stu-id="db5cf-140">Response</span></span>
<span data-ttu-id="db5cf-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db5cf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
