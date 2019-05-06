---
title: 列出 registeredUser
description: 检索已注册为设备用户的用户列表。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 857e41899c36cf7dc9600fa788e400770333d6ec
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33590894"
---
# <a name="list-registeredusers"></a><span data-ttu-id="df54e-103">列出 registeredUser</span><span class="sxs-lookup"><span data-stu-id="df54e-103">List registeredUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df54e-104">检索已注册为设备用户的用户列表。</span><span class="sxs-lookup"><span data-stu-id="df54e-104">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="df54e-105">对于云加入设备和已注册的个人设备，已注册用户在设备注册时设置为与已注册所有者相同的值。</span><span class="sxs-lookup"><span data-stu-id="df54e-105">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="df54e-106">权限</span><span class="sxs-lookup"><span data-stu-id="df54e-106">Permissions</span></span>
<span data-ttu-id="df54e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df54e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df54e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="df54e-109">Permission type</span></span>      | <span data-ttu-id="df54e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="df54e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df54e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df54e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="df54e-112">"Directory"、"all" 或 "Directory.accessasuser.all"</span><span class="sxs-lookup"><span data-stu-id="df54e-112">Directory.Read.All or Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="df54e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df54e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df54e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="df54e-114">Not supported.</span></span> |
|<span data-ttu-id="df54e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="df54e-115">Application</span></span> | <span data-ttu-id="df54e-116">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df54e-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="df54e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df54e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```

> <span data-ttu-id="df54e-118">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="df54e-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="df54e-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="df54e-119">Optional query parameters</span></span>
<span data-ttu-id="df54e-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="df54e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="df54e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="df54e-121">Request headers</span></span>
| <span data-ttu-id="df54e-122">名称</span><span class="sxs-lookup"><span data-stu-id="df54e-122">Name</span></span>       | <span data-ttu-id="df54e-123">类型</span><span class="sxs-lookup"><span data-stu-id="df54e-123">Type</span></span> | <span data-ttu-id="df54e-124">说明</span><span class="sxs-lookup"><span data-stu-id="df54e-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="df54e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="df54e-125">Authorization</span></span>  | <span data-ttu-id="df54e-126">string</span><span class="sxs-lookup"><span data-stu-id="df54e-126">string</span></span>  | <span data-ttu-id="df54e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="df54e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df54e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="df54e-129">Request body</span></span>
<span data-ttu-id="df54e-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="df54e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df54e-131">响应</span><span class="sxs-lookup"><span data-stu-id="df54e-131">Response</span></span>

<span data-ttu-id="df54e-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="df54e-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="df54e-133">示例</span><span class="sxs-lookup"><span data-stu-id="df54e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df54e-134">请求</span><span class="sxs-lookup"><span data-stu-id="df54e-134">Request</span></span>
<span data-ttu-id="df54e-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df54e-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="df54e-136">响应</span><span class="sxs-lookup"><span data-stu-id="df54e-136">Response</span></span>
<span data-ttu-id="df54e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="df54e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="df54e-140">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="df54e-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="df54e-141">语言</span><span class="sxs-lookup"><span data-stu-id="df54e-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_registeredusers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="df54e-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="df54e-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_registeredusers-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/device-list-registeredusers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/device-list-registeredusers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
