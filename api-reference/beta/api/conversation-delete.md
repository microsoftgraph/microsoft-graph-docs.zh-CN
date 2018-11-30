---
title: 删除对话
description: 删除对话。
ms.openlocfilehash: 9a6e590470343afd7990d6f24672fe1824c65a90
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044265"
---
# <a name="delete-conversation"></a><span data-ttu-id="7df89-103">删除对话</span><span class="sxs-lookup"><span data-stu-id="7df89-103">Delete conversation</span></span>

> <span data-ttu-id="7df89-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7df89-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7df89-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7df89-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7df89-106">删除对话。</span><span class="sxs-lookup"><span data-stu-id="7df89-106">Delete conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="7df89-107">权限</span><span class="sxs-lookup"><span data-stu-id="7df89-107">Permissions</span></span>
<span data-ttu-id="7df89-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7df89-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7df89-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7df89-110">Permission type</span></span>      | <span data-ttu-id="7df89-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7df89-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7df89-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7df89-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7df89-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7df89-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7df89-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7df89-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7df89-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7df89-115">Not supported.</span></span>    |
|<span data-ttu-id="7df89-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7df89-116">Application</span></span> | <span data-ttu-id="7df89-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7df89-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7df89-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7df89-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7df89-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7df89-119">Request headers</span></span>
| <span data-ttu-id="7df89-120">标头</span><span class="sxs-lookup"><span data-stu-id="7df89-120">Header</span></span>       | <span data-ttu-id="7df89-121">值</span><span class="sxs-lookup"><span data-stu-id="7df89-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7df89-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7df89-122">Authorization</span></span>  | <span data-ttu-id="7df89-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7df89-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7df89-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7df89-125">Request body</span></span>
<span data-ttu-id="7df89-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7df89-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7df89-127">响应</span><span class="sxs-lookup"><span data-stu-id="7df89-127">Response</span></span>

<span data-ttu-id="7df89-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7df89-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7df89-130">示例</span><span class="sxs-lookup"><span data-stu-id="7df89-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7df89-131">请求</span><span class="sxs-lookup"><span data-stu-id="7df89-131">Request</span></span>
<span data-ttu-id="7df89-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7df89-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversation"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="7df89-133">响应</span><span class="sxs-lookup"><span data-stu-id="7df89-133">Response</span></span>
<span data-ttu-id="7df89-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7df89-134">Here is an example of the response.</span></span> 
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
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
