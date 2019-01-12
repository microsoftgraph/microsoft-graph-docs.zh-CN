---
title: 删除 messageRule
description: 删除指定的 messageRule 对象。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 570970296444b5bb4d5033bf26a03214d9fa8dac
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957359"
---
# <a name="delete-messagerule"></a><span data-ttu-id="6fd71-103">删除 messageRule</span><span class="sxs-lookup"><span data-stu-id="6fd71-103">Delete messageRule</span></span>


<span data-ttu-id="6fd71-104">删除指定的 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6fd71-104">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6fd71-105">权限</span><span class="sxs-lookup"><span data-stu-id="6fd71-105">Permissions</span></span>
<span data-ttu-id="6fd71-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6fd71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fd71-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6fd71-108">Permission type</span></span>      | <span data-ttu-id="6fd71-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6fd71-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fd71-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6fd71-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6fd71-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6fd71-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="6fd71-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6fd71-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fd71-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6fd71-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="6fd71-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6fd71-114">Application</span></span> | <span data-ttu-id="6fd71-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6fd71-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fd71-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6fd71-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messageRules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6fd71-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="6fd71-117">Request headers</span></span>
| <span data-ttu-id="6fd71-118">名称</span><span class="sxs-lookup"><span data-stu-id="6fd71-118">Name</span></span>       | <span data-ttu-id="6fd71-119">说明</span><span class="sxs-lookup"><span data-stu-id="6fd71-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6fd71-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fd71-120">Authorization</span></span>  | <span data-ttu-id="6fd71-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6fd71-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="6fd71-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6fd71-123">Request body</span></span>
<span data-ttu-id="6fd71-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6fd71-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="6fd71-125">响应</span><span class="sxs-lookup"><span data-stu-id="6fd71-125">Response</span></span>
<span data-ttu-id="6fd71-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6fd71-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fd71-128">示例</span><span class="sxs-lookup"><span data-stu-id="6fd71-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6fd71-129">请求</span><span class="sxs-lookup"><span data-stu-id="6fd71-129">Request</span></span>
<span data-ttu-id="6fd71-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6fd71-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZp8="],
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZp8=

```
##### <a name="response"></a><span data-ttu-id="6fd71-131">响应</span><span class="sxs-lookup"><span data-stu-id="6fd71-131">Response</span></span>
<span data-ttu-id="6fd71-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6fd71-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
