---
title: 删除设备
description: 删除已注册的设备。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3fac5ac3e7d12d1a6a124cf7c56491b204a59361
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657460"
---
# <a name="delete-device"></a><span data-ttu-id="36fd0-103">删除设备</span><span class="sxs-lookup"><span data-stu-id="36fd0-103">Delete device</span></span>

<span data-ttu-id="36fd0-104">删除已注册的设备。</span><span class="sxs-lookup"><span data-stu-id="36fd0-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="36fd0-105">权限</span><span class="sxs-lookup"><span data-stu-id="36fd0-105">Permissions</span></span>
<span data-ttu-id="36fd0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36fd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="36fd0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="36fd0-108">Permission type</span></span>      | <span data-ttu-id="36fd0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="36fd0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36fd0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36fd0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="36fd0-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="36fd0-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="36fd0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36fd0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36fd0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="36fd0-113">Not supported.</span></span>    |
|<span data-ttu-id="36fd0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="36fd0-114">Application</span></span> | <span data-ttu-id="36fd0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="36fd0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36fd0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36fd0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="36fd0-117">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="36fd0-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36fd0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="36fd0-118">Request headers</span></span>
| <span data-ttu-id="36fd0-119">名称</span><span class="sxs-lookup"><span data-stu-id="36fd0-119">Name</span></span>       | <span data-ttu-id="36fd0-120">类型</span><span class="sxs-lookup"><span data-stu-id="36fd0-120">Type</span></span> | <span data-ttu-id="36fd0-121">说明</span><span class="sxs-lookup"><span data-stu-id="36fd0-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="36fd0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="36fd0-122">Authorization</span></span>  | <span data-ttu-id="36fd0-123">string</span><span class="sxs-lookup"><span data-stu-id="36fd0-123">string</span></span>  | <span data-ttu-id="36fd0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="36fd0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36fd0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="36fd0-126">Request body</span></span>
<span data-ttu-id="36fd0-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="36fd0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36fd0-128">响应</span><span class="sxs-lookup"><span data-stu-id="36fd0-128">Response</span></span>

<span data-ttu-id="36fd0-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="36fd0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36fd0-131">示例</span><span class="sxs-lookup"><span data-stu-id="36fd0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36fd0-132">请求</span><span class="sxs-lookup"><span data-stu-id="36fd0-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="36fd0-133">响应</span><span class="sxs-lookup"><span data-stu-id="36fd0-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="36fd0-134">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="36fd0-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="36fd0-135">C#</span><span class="sxs-lookup"><span data-stu-id="36fd0-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_device-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36fd0-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="36fd0-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_device-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/device-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/device-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
