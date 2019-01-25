---
title: 删除设备
description: 删除已注册的设备。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0efbfe2aa06579a5c52c2cee1020e0269bc0265f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523006"
---
# <a name="delete-device"></a><span data-ttu-id="96f99-103">删除设备</span><span class="sxs-lookup"><span data-stu-id="96f99-103">Delete device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96f99-104">删除已注册的设备。</span><span class="sxs-lookup"><span data-stu-id="96f99-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="96f99-105">权限</span><span class="sxs-lookup"><span data-stu-id="96f99-105">Permissions</span></span>
<span data-ttu-id="96f99-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96f99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="96f99-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="96f99-108">Permission type</span></span>      | <span data-ttu-id="96f99-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96f99-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96f99-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96f99-110">Delegated (work or school account)</span></span> | <span data-ttu-id="96f99-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="96f99-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="96f99-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96f99-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96f99-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="96f99-113">Not supported.</span></span>    |
|<span data-ttu-id="96f99-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="96f99-114">Application</span></span> | <span data-ttu-id="96f99-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="96f99-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96f99-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96f99-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}

```

> <span data-ttu-id="96f99-117">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="96f99-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96f99-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="96f99-118">Request headers</span></span>
| <span data-ttu-id="96f99-119">名称</span><span class="sxs-lookup"><span data-stu-id="96f99-119">Name</span></span>       | <span data-ttu-id="96f99-120">类型</span><span class="sxs-lookup"><span data-stu-id="96f99-120">Type</span></span> | <span data-ttu-id="96f99-121">说明</span><span class="sxs-lookup"><span data-stu-id="96f99-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="96f99-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="96f99-122">Authorization</span></span>  | <span data-ttu-id="96f99-123">string</span><span class="sxs-lookup"><span data-stu-id="96f99-123">string</span></span>  | <span data-ttu-id="96f99-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96f99-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96f99-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="96f99-126">Request body</span></span>
<span data-ttu-id="96f99-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96f99-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96f99-128">响应</span><span class="sxs-lookup"><span data-stu-id="96f99-128">Response</span></span>

<span data-ttu-id="96f99-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="96f99-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96f99-131">示例</span><span class="sxs-lookup"><span data-stu-id="96f99-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96f99-132">请求</span><span class="sxs-lookup"><span data-stu-id="96f99-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/beta/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="96f99-133">响应</span><span class="sxs-lookup"><span data-stu-id="96f99-133">Response</span></span>

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
    "Error: /api-reference/beta/api/device-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
