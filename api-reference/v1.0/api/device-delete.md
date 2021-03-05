---
title: 删除设备
description: 删除已注册的设备。
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9aa477f6b5ef1505a6fe8b26a0afc980d0adc04e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434613"
---
# <a name="delete-device"></a><span data-ttu-id="9d64a-103">删除设备</span><span class="sxs-lookup"><span data-stu-id="9d64a-103">Delete device</span></span>

<span data-ttu-id="9d64a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d64a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9d64a-105">删除已注册的设备。</span><span class="sxs-lookup"><span data-stu-id="9d64a-105">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d64a-106">权限</span><span class="sxs-lookup"><span data-stu-id="9d64a-106">Permissions</span></span>
<span data-ttu-id="9d64a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9d64a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9d64a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d64a-109">Permission type</span></span>      | <span data-ttu-id="9d64a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9d64a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d64a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d64a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9d64a-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9d64a-112">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="9d64a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d64a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d64a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d64a-114">Not supported.</span></span>    |
|<span data-ttu-id="9d64a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d64a-115">Application</span></span> | <span data-ttu-id="9d64a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d64a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d64a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d64a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="9d64a-118">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="9d64a-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d64a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d64a-119">Request headers</span></span>
| <span data-ttu-id="9d64a-120">名称</span><span class="sxs-lookup"><span data-stu-id="9d64a-120">Name</span></span>       | <span data-ttu-id="9d64a-121">类型</span><span class="sxs-lookup"><span data-stu-id="9d64a-121">Type</span></span> | <span data-ttu-id="9d64a-122">说明</span><span class="sxs-lookup"><span data-stu-id="9d64a-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9d64a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d64a-123">Authorization</span></span>  | <span data-ttu-id="9d64a-124">string</span><span class="sxs-lookup"><span data-stu-id="9d64a-124">string</span></span>  | <span data-ttu-id="9d64a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9d64a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d64a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d64a-127">Request body</span></span>
<span data-ttu-id="9d64a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9d64a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d64a-129">响应</span><span class="sxs-lookup"><span data-stu-id="9d64a-129">Response</span></span>

<span data-ttu-id="9d64a-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9d64a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d64a-132">示例</span><span class="sxs-lookup"><span data-stu-id="9d64a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9d64a-133">请求</span><span class="sxs-lookup"><span data-stu-id="9d64a-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9d64a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d64a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
# <a name="c"></a>[<span data-ttu-id="9d64a-135">C#</span><span class="sxs-lookup"><span data-stu-id="9d64a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d64a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d64a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d64a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d64a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d64a-138">Java</span><span class="sxs-lookup"><span data-stu-id="9d64a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9d64a-139">响应</span><span class="sxs-lookup"><span data-stu-id="9d64a-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

