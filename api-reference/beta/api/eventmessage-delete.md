---
title: 删除 eventMessage
description: 删除 eventMessage。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 23007501878f5c5d25af924f3a7e8e1bb618b364
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945956"
---
# <a name="delete-eventmessage"></a><span data-ttu-id="34186-103">删除 eventMessage</span><span class="sxs-lookup"><span data-stu-id="34186-103">Delete eventMessage</span></span>

> <span data-ttu-id="34186-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="34186-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34186-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="34186-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34186-106">删除 eventMessage。</span><span class="sxs-lookup"><span data-stu-id="34186-106">Delete eventMessage.</span></span>
## <a name="permissions"></a><span data-ttu-id="34186-107">权限</span><span class="sxs-lookup"><span data-stu-id="34186-107">Permissions</span></span>
<span data-ttu-id="34186-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="34186-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34186-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="34186-110">Permission type</span></span>      | <span data-ttu-id="34186-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="34186-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34186-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="34186-112">Delegated (work or school account)</span></span> | <span data-ttu-id="34186-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34186-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="34186-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="34186-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34186-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34186-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="34186-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="34186-116">Application</span></span> | <span data-ttu-id="34186-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34186-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="34186-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="34186-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="34186-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="34186-119">Request headers</span></span>
| <span data-ttu-id="34186-120">名称</span><span class="sxs-lookup"><span data-stu-id="34186-120">Name</span></span>       | <span data-ttu-id="34186-121">类型</span><span class="sxs-lookup"><span data-stu-id="34186-121">Type</span></span> | <span data-ttu-id="34186-122">说明</span><span class="sxs-lookup"><span data-stu-id="34186-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="34186-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="34186-123">Authorization</span></span>  | <span data-ttu-id="34186-124">string</span><span class="sxs-lookup"><span data-stu-id="34186-124">string</span></span>  | <span data-ttu-id="34186-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="34186-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="34186-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="34186-127">Request body</span></span>
<span data-ttu-id="34186-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="34186-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34186-129">响应</span><span class="sxs-lookup"><span data-stu-id="34186-129">Response</span></span>

<span data-ttu-id="34186-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="34186-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34186-132">示例</span><span class="sxs-lookup"><span data-stu-id="34186-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34186-133">请求</span><span class="sxs-lookup"><span data-stu-id="34186-133">Request</span></span>
<span data-ttu-id="34186-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="34186-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="34186-135">响应</span><span class="sxs-lookup"><span data-stu-id="34186-135">Response</span></span>
<span data-ttu-id="34186-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="34186-136">Here is an example of the response.</span></span> 
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
  "description": "Delete eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
