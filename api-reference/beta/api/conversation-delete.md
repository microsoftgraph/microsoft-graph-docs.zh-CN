---
title: 删除对话
description: 删除对话。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: af7aead90efdf40ce30d58dbc5c7c6b20d26f15f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455570"
---
# <a name="delete-conversation"></a><span data-ttu-id="2e004-103">删除对话</span><span class="sxs-lookup"><span data-stu-id="2e004-103">Delete conversation</span></span>

<span data-ttu-id="2e004-104">删除对话。</span><span class="sxs-lookup"><span data-stu-id="2e004-104">Delete conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="2e004-105">权限</span><span class="sxs-lookup"><span data-stu-id="2e004-105">Permissions</span></span>
<span data-ttu-id="2e004-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2e004-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e004-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e004-108">Permission type</span></span>      | <span data-ttu-id="2e004-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2e004-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e004-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e004-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2e004-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e004-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2e004-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e004-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e004-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e004-113">Not supported.</span></span>    |
|<span data-ttu-id="2e004-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e004-114">Application</span></span> | <span data-ttu-id="2e004-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e004-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e004-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e004-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2e004-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e004-117">Request headers</span></span>
| <span data-ttu-id="2e004-118">标头</span><span class="sxs-lookup"><span data-stu-id="2e004-118">Header</span></span>       | <span data-ttu-id="2e004-119">值</span><span class="sxs-lookup"><span data-stu-id="2e004-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2e004-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e004-120">Authorization</span></span>  | <span data-ttu-id="2e004-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2e004-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2e004-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e004-123">Request body</span></span>
<span data-ttu-id="2e004-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2e004-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e004-125">响应</span><span class="sxs-lookup"><span data-stu-id="2e004-125">Response</span></span>

<span data-ttu-id="2e004-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2e004-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e004-128">示例</span><span class="sxs-lookup"><span data-stu-id="2e004-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e004-129">请求</span><span class="sxs-lookup"><span data-stu-id="2e004-129">Request</span></span>
<span data-ttu-id="2e004-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2e004-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="2e004-131">响应</span><span class="sxs-lookup"><span data-stu-id="2e004-131">Response</span></span>
<span data-ttu-id="2e004-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2e004-132">Here is an example of the response.</span></span> 
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
