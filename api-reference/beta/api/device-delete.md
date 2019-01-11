---
title: 删除设备
description: 删除已注册的设备。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c2b34cffbff6b3c627ed13d6e4b2917f6f36f4f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854570"
---
# <a name="delete-device"></a><span data-ttu-id="f1c79-103">删除设备</span><span class="sxs-lookup"><span data-stu-id="f1c79-103">Delete device</span></span>

> <span data-ttu-id="f1c79-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f1c79-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1c79-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f1c79-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f1c79-106">删除已注册的设备。</span><span class="sxs-lookup"><span data-stu-id="f1c79-106">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1c79-107">权限</span><span class="sxs-lookup"><span data-stu-id="f1c79-107">Permissions</span></span>
<span data-ttu-id="f1c79-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1c79-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f1c79-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1c79-110">Permission type</span></span>      | <span data-ttu-id="f1c79-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f1c79-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1c79-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1c79-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f1c79-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f1c79-113">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="f1c79-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1c79-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1c79-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1c79-115">Not supported.</span></span>    |
|<span data-ttu-id="f1c79-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1c79-116">Application</span></span> | <span data-ttu-id="f1c79-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1c79-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1c79-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1c79-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}

```

> <span data-ttu-id="f1c79-119">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="f1c79-119">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1c79-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1c79-120">Request headers</span></span>
| <span data-ttu-id="f1c79-121">名称</span><span class="sxs-lookup"><span data-stu-id="f1c79-121">Name</span></span>       | <span data-ttu-id="f1c79-122">类型</span><span class="sxs-lookup"><span data-stu-id="f1c79-122">Type</span></span> | <span data-ttu-id="f1c79-123">说明</span><span class="sxs-lookup"><span data-stu-id="f1c79-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f1c79-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1c79-124">Authorization</span></span>  | <span data-ttu-id="f1c79-125">string</span><span class="sxs-lookup"><span data-stu-id="f1c79-125">string</span></span>  | <span data-ttu-id="f1c79-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f1c79-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1c79-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1c79-128">Request body</span></span>
<span data-ttu-id="f1c79-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f1c79-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1c79-130">响应</span><span class="sxs-lookup"><span data-stu-id="f1c79-130">Response</span></span>

<span data-ttu-id="f1c79-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f1c79-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1c79-133">示例</span><span class="sxs-lookup"><span data-stu-id="f1c79-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1c79-134">请求</span><span class="sxs-lookup"><span data-stu-id="f1c79-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/beta/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="f1c79-135">响应</span><span class="sxs-lookup"><span data-stu-id="f1c79-135">Response</span></span>

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
  "tocPath": ""
}-->
