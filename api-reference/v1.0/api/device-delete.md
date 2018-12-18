---
title: 删除设备
description: 删除已注册的设备。
author: tfitzmac
ms.openlocfilehash: ae2f4b458ebd18c366c2b8aecf6b203ff5d42cda
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342901"
---
# <a name="delete-device"></a><span data-ttu-id="89a6c-103">删除设备</span><span class="sxs-lookup"><span data-stu-id="89a6c-103">Delete device</span></span>

<span data-ttu-id="89a6c-104">删除已注册的设备。</span><span class="sxs-lookup"><span data-stu-id="89a6c-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="89a6c-105">权限</span><span class="sxs-lookup"><span data-stu-id="89a6c-105">Permissions</span></span>
<span data-ttu-id="89a6c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89a6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="89a6c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="89a6c-108">Permission type</span></span>      | <span data-ttu-id="89a6c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="89a6c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89a6c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89a6c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="89a6c-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="89a6c-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="89a6c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89a6c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89a6c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="89a6c-113">Not supported.</span></span>    |
|<span data-ttu-id="89a6c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="89a6c-114">Application</span></span> | <span data-ttu-id="89a6c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="89a6c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89a6c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89a6c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="89a6c-117">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="89a6c-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="89a6c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="89a6c-118">Request headers</span></span>
| <span data-ttu-id="89a6c-119">Name</span><span class="sxs-lookup"><span data-stu-id="89a6c-119">Name</span></span>       | <span data-ttu-id="89a6c-120">类型</span><span class="sxs-lookup"><span data-stu-id="89a6c-120">Type</span></span> | <span data-ttu-id="89a6c-121">说明</span><span class="sxs-lookup"><span data-stu-id="89a6c-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="89a6c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="89a6c-122">Authorization</span></span>  | <span data-ttu-id="89a6c-123">string</span><span class="sxs-lookup"><span data-stu-id="89a6c-123">string</span></span>  | <span data-ttu-id="89a6c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="89a6c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89a6c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="89a6c-126">Request body</span></span>
<span data-ttu-id="89a6c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="89a6c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89a6c-128">响应</span><span class="sxs-lookup"><span data-stu-id="89a6c-128">Response</span></span>

<span data-ttu-id="89a6c-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="89a6c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89a6c-131">示例</span><span class="sxs-lookup"><span data-stu-id="89a6c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89a6c-132">请求</span><span class="sxs-lookup"><span data-stu-id="89a6c-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="89a6c-133">响应</span><span class="sxs-lookup"><span data-stu-id="89a6c-133">Response</span></span>

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
