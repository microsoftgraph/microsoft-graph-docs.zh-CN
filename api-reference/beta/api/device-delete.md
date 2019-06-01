---
title: 删除设备
description: 删除已注册的设备。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 60122fbce9117b617a31d5b61cefd60eb596129f
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656396"
---
# <a name="delete-device"></a><span data-ttu-id="fbf00-103">删除设备</span><span class="sxs-lookup"><span data-stu-id="fbf00-103">Delete device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbf00-104">删除已注册的设备。</span><span class="sxs-lookup"><span data-stu-id="fbf00-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="fbf00-105">权限</span><span class="sxs-lookup"><span data-stu-id="fbf00-105">Permissions</span></span>
<span data-ttu-id="fbf00-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fbf00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fbf00-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fbf00-108">Permission type</span></span>      | <span data-ttu-id="fbf00-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fbf00-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbf00-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fbf00-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fbf00-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fbf00-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="fbf00-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fbf00-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbf00-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbf00-113">Not supported.</span></span>    |
|<span data-ttu-id="fbf00-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fbf00-114">Application</span></span> | <span data-ttu-id="fbf00-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbf00-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbf00-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fbf00-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}

```

> <span data-ttu-id="fbf00-117">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="fbf00-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fbf00-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fbf00-118">Request headers</span></span>
| <span data-ttu-id="fbf00-119">名称</span><span class="sxs-lookup"><span data-stu-id="fbf00-119">Name</span></span>       | <span data-ttu-id="fbf00-120">类型</span><span class="sxs-lookup"><span data-stu-id="fbf00-120">Type</span></span> | <span data-ttu-id="fbf00-121">说明</span><span class="sxs-lookup"><span data-stu-id="fbf00-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fbf00-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbf00-122">Authorization</span></span>  | <span data-ttu-id="fbf00-123">string</span><span class="sxs-lookup"><span data-stu-id="fbf00-123">string</span></span>  | <span data-ttu-id="fbf00-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fbf00-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fbf00-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fbf00-126">Request body</span></span>
<span data-ttu-id="fbf00-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fbf00-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbf00-128">响应</span><span class="sxs-lookup"><span data-stu-id="fbf00-128">Response</span></span>

<span data-ttu-id="fbf00-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fbf00-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbf00-131">示例</span><span class="sxs-lookup"><span data-stu-id="fbf00-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fbf00-132">请求</span><span class="sxs-lookup"><span data-stu-id="fbf00-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/beta/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="fbf00-133">响应</span><span class="sxs-lookup"><span data-stu-id="fbf00-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fbf00-134">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="fbf00-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fbf00-135">C#</span><span class="sxs-lookup"><span data-stu-id="fbf00-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_device-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fbf00-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="fbf00-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_device-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/device-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/device-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
