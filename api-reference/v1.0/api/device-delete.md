---
title: 删除设备
description: 删除已注册的设备。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: eec8a198c783a0c04ba1e20d73095701c471b5cb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845666"
---
# <a name="delete-device"></a><span data-ttu-id="4fa0d-103">删除设备</span><span class="sxs-lookup"><span data-stu-id="4fa0d-103">Delete device</span></span>

<span data-ttu-id="4fa0d-104">删除已注册的设备。</span><span class="sxs-lookup"><span data-stu-id="4fa0d-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="4fa0d-105">权限</span><span class="sxs-lookup"><span data-stu-id="4fa0d-105">Permissions</span></span>
<span data-ttu-id="4fa0d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4fa0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4fa0d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4fa0d-108">Permission type</span></span>      | <span data-ttu-id="4fa0d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4fa0d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4fa0d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4fa0d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4fa0d-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4fa0d-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="4fa0d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4fa0d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fa0d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fa0d-113">Not supported.</span></span>    |
|<span data-ttu-id="4fa0d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4fa0d-114">Application</span></span> | <span data-ttu-id="4fa0d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fa0d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4fa0d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4fa0d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="4fa0d-117">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="4fa0d-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4fa0d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4fa0d-118">Request headers</span></span>
| <span data-ttu-id="4fa0d-119">名称</span><span class="sxs-lookup"><span data-stu-id="4fa0d-119">Name</span></span>       | <span data-ttu-id="4fa0d-120">类型</span><span class="sxs-lookup"><span data-stu-id="4fa0d-120">Type</span></span> | <span data-ttu-id="4fa0d-121">说明</span><span class="sxs-lookup"><span data-stu-id="4fa0d-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4fa0d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fa0d-122">Authorization</span></span>  | <span data-ttu-id="4fa0d-123">string</span><span class="sxs-lookup"><span data-stu-id="4fa0d-123">string</span></span>  | <span data-ttu-id="4fa0d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4fa0d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4fa0d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4fa0d-126">Request body</span></span>
<span data-ttu-id="4fa0d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4fa0d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4fa0d-128">响应</span><span class="sxs-lookup"><span data-stu-id="4fa0d-128">Response</span></span>

<span data-ttu-id="4fa0d-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4fa0d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fa0d-131">示例</span><span class="sxs-lookup"><span data-stu-id="4fa0d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4fa0d-132">请求</span><span class="sxs-lookup"><span data-stu-id="4fa0d-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="4fa0d-133">响应</span><span class="sxs-lookup"><span data-stu-id="4fa0d-133">Response</span></span>

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
