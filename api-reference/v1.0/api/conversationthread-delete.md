---
title: 删除 conversationThread
description: 删除 conversationThread。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 486752a88a3d9b632b430e46a7fd9d155ab989fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566141"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="74329-103">删除 conversationThread</span><span class="sxs-lookup"><span data-stu-id="74329-103">Delete conversationThread</span></span>

<span data-ttu-id="74329-104">删除 conversationThread。</span><span class="sxs-lookup"><span data-stu-id="74329-104">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="74329-105">权限</span><span class="sxs-lookup"><span data-stu-id="74329-105">Permissions</span></span>
<span data-ttu-id="74329-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74329-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74329-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="74329-108">Permission type</span></span>      | <span data-ttu-id="74329-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="74329-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74329-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74329-110">Delegated (work or school account)</span></span> | <span data-ttu-id="74329-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74329-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="74329-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74329-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74329-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="74329-113">Not supported.</span></span>    |
|<span data-ttu-id="74329-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="74329-114">Application</span></span> | <span data-ttu-id="74329-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74329-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="74329-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74329-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="74329-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="74329-117">Request headers</span></span>
| <span data-ttu-id="74329-118">标头</span><span class="sxs-lookup"><span data-stu-id="74329-118">Header</span></span>       | <span data-ttu-id="74329-119">值</span><span class="sxs-lookup"><span data-stu-id="74329-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="74329-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="74329-120">Authorization</span></span>  | <span data-ttu-id="74329-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="74329-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="74329-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="74329-123">Request body</span></span>
<span data-ttu-id="74329-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="74329-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74329-125">响应</span><span class="sxs-lookup"><span data-stu-id="74329-125">Response</span></span>

<span data-ttu-id="74329-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="74329-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74329-128">示例</span><span class="sxs-lookup"><span data-stu-id="74329-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74329-129">请求</span><span class="sxs-lookup"><span data-stu-id="74329-129">Request</span></span>
<span data-ttu-id="74329-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="74329-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="74329-131">响应</span><span class="sxs-lookup"><span data-stu-id="74329-131">Response</span></span>
<span data-ttu-id="74329-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="74329-132">Here is an example of the response.</span></span> 
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
  "description": "Delete conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
