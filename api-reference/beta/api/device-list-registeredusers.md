---
title: 列出 registeredUser
description: 检索已注册为设备用户的用户列表。
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9ebeb558e4c969d9249bbfbca7779b4a0213765e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962856"
---
# <a name="list-registeredusers"></a><span data-ttu-id="ff2c7-103">列出 registeredUser</span><span class="sxs-lookup"><span data-stu-id="ff2c7-103">List registeredUsers</span></span>

<span data-ttu-id="ff2c7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff2c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff2c7-105">检索已注册为设备用户的用户列表。</span><span class="sxs-lookup"><span data-stu-id="ff2c7-105">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="ff2c7-106">对于云加入设备和已注册的个人设备，已注册用户在设备注册时设置为与已注册所有者相同的值。</span><span class="sxs-lookup"><span data-stu-id="ff2c7-106">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff2c7-107">权限</span><span class="sxs-lookup"><span data-stu-id="ff2c7-107">Permissions</span></span>
<span data-ttu-id="ff2c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff2c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff2c7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff2c7-110">Permission type</span></span>      | <span data-ttu-id="ff2c7-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ff2c7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff2c7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff2c7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ff2c7-113">"Directory"、"all" 或 "Directory.accessasuser.all"</span><span class="sxs-lookup"><span data-stu-id="ff2c7-113">Directory.Read.All or Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ff2c7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff2c7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff2c7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff2c7-115">Not supported.</span></span> |
|<span data-ttu-id="ff2c7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff2c7-116">Application</span></span> | <span data-ttu-id="ff2c7-117">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff2c7-117">Directory.Read.All or Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="ff2c7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff2c7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```

> <span data-ttu-id="ff2c7-119">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="ff2c7-119">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="ff2c7-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ff2c7-120">Optional query parameters</span></span>
<span data-ttu-id="ff2c7-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ff2c7-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ff2c7-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff2c7-122">Request headers</span></span>
| <span data-ttu-id="ff2c7-123">名称</span><span class="sxs-lookup"><span data-stu-id="ff2c7-123">Name</span></span>       | <span data-ttu-id="ff2c7-124">类型</span><span class="sxs-lookup"><span data-stu-id="ff2c7-124">Type</span></span> | <span data-ttu-id="ff2c7-125">说明</span><span class="sxs-lookup"><span data-stu-id="ff2c7-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ff2c7-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff2c7-126">Authorization</span></span>  | <span data-ttu-id="ff2c7-127">string</span><span class="sxs-lookup"><span data-stu-id="ff2c7-127">string</span></span>  | <span data-ttu-id="ff2c7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ff2c7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff2c7-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff2c7-130">Request body</span></span>
<span data-ttu-id="ff2c7-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ff2c7-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff2c7-132">响应</span><span class="sxs-lookup"><span data-stu-id="ff2c7-132">Response</span></span>

<span data-ttu-id="ff2c7-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ff2c7-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ff2c7-134">示例</span><span class="sxs-lookup"><span data-stu-id="ff2c7-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff2c7-135">请求</span><span class="sxs-lookup"><span data-stu-id="ff2c7-135">Request</span></span>
<span data-ttu-id="ff2c7-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ff2c7-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ff2c7-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff2c7-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/registeredUsers
```
# <a name="c"></a>[<span data-ttu-id="ff2c7-138">C#</span><span class="sxs-lookup"><span data-stu-id="ff2c7-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff2c7-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff2c7-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff2c7-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff2c7-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ff2c7-141">Java</span><span class="sxs-lookup"><span data-stu-id="ff2c7-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ff2c7-142">响应</span><span class="sxs-lookup"><span data-stu-id="ff2c7-142">Response</span></span>
<span data-ttu-id="ff2c7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ff2c7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
