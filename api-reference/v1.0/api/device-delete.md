---
title: 删除设备
description: 删除已注册的设备。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 51adc59b901a2a639360fe12c8a80e2fe6114808
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276382"
---
# <a name="delete-device"></a><span data-ttu-id="6ea6a-103">删除设备</span><span class="sxs-lookup"><span data-stu-id="6ea6a-103">Delete device</span></span>

<span data-ttu-id="6ea6a-104">删除已注册的设备。</span><span class="sxs-lookup"><span data-stu-id="6ea6a-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ea6a-105">权限</span><span class="sxs-lookup"><span data-stu-id="6ea6a-105">Permissions</span></span>
<span data-ttu-id="6ea6a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ea6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6ea6a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ea6a-108">Permission type</span></span>      | <span data-ttu-id="6ea6a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6ea6a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ea6a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ea6a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6ea6a-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6ea6a-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="6ea6a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ea6a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ea6a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ea6a-113">Not supported.</span></span>    |
|<span data-ttu-id="6ea6a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ea6a-114">Application</span></span> | <span data-ttu-id="6ea6a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ea6a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ea6a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ea6a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="6ea6a-117">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="6ea6a-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ea6a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ea6a-118">Request headers</span></span>
| <span data-ttu-id="6ea6a-119">名称</span><span class="sxs-lookup"><span data-stu-id="6ea6a-119">Name</span></span>       | <span data-ttu-id="6ea6a-120">类型</span><span class="sxs-lookup"><span data-stu-id="6ea6a-120">Type</span></span> | <span data-ttu-id="6ea6a-121">说明</span><span class="sxs-lookup"><span data-stu-id="6ea6a-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6ea6a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ea6a-122">Authorization</span></span>  | <span data-ttu-id="6ea6a-123">string</span><span class="sxs-lookup"><span data-stu-id="6ea6a-123">string</span></span>  | <span data-ttu-id="6ea6a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6ea6a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ea6a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ea6a-126">Request body</span></span>
<span data-ttu-id="6ea6a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6ea6a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ea6a-128">响应</span><span class="sxs-lookup"><span data-stu-id="6ea6a-128">Response</span></span>

<span data-ttu-id="6ea6a-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6ea6a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ea6a-131">示例</span><span class="sxs-lookup"><span data-stu-id="6ea6a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ea6a-132">请求</span><span class="sxs-lookup"><span data-stu-id="6ea6a-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="6ea6a-133">响应</span><span class="sxs-lookup"><span data-stu-id="6ea6a-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6ea6a-134">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="6ea6a-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6ea6a-135">C#</span><span class="sxs-lookup"><span data-stu-id="6ea6a-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_device-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6ea6a-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="6ea6a-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_device-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6ea6a-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="6ea6a-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_device-Objective-C-snippets.md)]
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
    "Error: /api-reference/v1.0/api/device-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/device-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/device-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
