---
title: 删除设备
description: 删除已注册的设备。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b6f225cc410515b40952e64fb13d053b2eeb25fa
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "36417695"
---
# <a name="delete-device"></a><span data-ttu-id="cfbfa-103">删除设备</span><span class="sxs-lookup"><span data-stu-id="cfbfa-103">Delete device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfbfa-104">删除已注册的设备。</span><span class="sxs-lookup"><span data-stu-id="cfbfa-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfbfa-105">权限</span><span class="sxs-lookup"><span data-stu-id="cfbfa-105">Permissions</span></span>
<span data-ttu-id="cfbfa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cfbfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cfbfa-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cfbfa-108">Permission type</span></span>      | <span data-ttu-id="cfbfa-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cfbfa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfbfa-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cfbfa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cfbfa-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cfbfa-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="cfbfa-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cfbfa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfbfa-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfbfa-113">Not supported.</span></span>    |
|<span data-ttu-id="cfbfa-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cfbfa-114">Application</span></span> | <span data-ttu-id="cfbfa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfbfa-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfbfa-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cfbfa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}

```

> <span data-ttu-id="cfbfa-117">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="cfbfa-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cfbfa-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cfbfa-118">Request headers</span></span>
| <span data-ttu-id="cfbfa-119">名称</span><span class="sxs-lookup"><span data-stu-id="cfbfa-119">Name</span></span>       | <span data-ttu-id="cfbfa-120">类型</span><span class="sxs-lookup"><span data-stu-id="cfbfa-120">Type</span></span> | <span data-ttu-id="cfbfa-121">说明</span><span class="sxs-lookup"><span data-stu-id="cfbfa-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cfbfa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfbfa-122">Authorization</span></span>  | <span data-ttu-id="cfbfa-123">string</span><span class="sxs-lookup"><span data-stu-id="cfbfa-123">string</span></span>  | <span data-ttu-id="cfbfa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cfbfa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfbfa-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cfbfa-126">Request body</span></span>
<span data-ttu-id="cfbfa-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cfbfa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfbfa-128">响应</span><span class="sxs-lookup"><span data-stu-id="cfbfa-128">Response</span></span>

<span data-ttu-id="cfbfa-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cfbfa-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfbfa-131">示例</span><span class="sxs-lookup"><span data-stu-id="cfbfa-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cfbfa-132">请求</span><span class="sxs-lookup"><span data-stu-id="cfbfa-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cfbfa-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfbfa-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/beta/devices/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cfbfa-134">C#</span><span class="sxs-lookup"><span data-stu-id="cfbfa-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cfbfa-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfbfa-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cfbfa-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfbfa-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cfbfa-137">响应</span><span class="sxs-lookup"><span data-stu-id="cfbfa-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
