---
title: 组：unsubscribeByMail
description: '调用此方法将禁用当前用户接收此组的电子邮件通知。此组中的新帖子、事件和文件。 仅支持 Office 365 组。 '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5df9934706d32ff4c2103ee350b31fee37d432b1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324096"
---
# <a name="group-unsubscribebymail"></a><span data-ttu-id="42f1d-104">组：unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="42f1d-104">group: unsubscribeByMail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42f1d-105">调用此方法将禁用当前用户接收此组的电子邮件通知。此组中的新帖子、事件和文件。</span><span class="sxs-lookup"><span data-stu-id="42f1d-105">Calling this method will disable the current user to receive email notifications for this group about new posts, events, and files in that group.</span></span> <span data-ttu-id="42f1d-106">仅支持 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="42f1d-106">Supported for Office 365 groups only.</span></span> 

## <a name="permissions"></a><span data-ttu-id="42f1d-107">权限</span><span class="sxs-lookup"><span data-stu-id="42f1d-107">Permissions</span></span>
<span data-ttu-id="42f1d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42f1d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42f1d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="42f1d-110">Permission type</span></span>      | <span data-ttu-id="42f1d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="42f1d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42f1d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42f1d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="42f1d-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42f1d-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="42f1d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42f1d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42f1d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="42f1d-115">Not supported.</span></span>    |
|<span data-ttu-id="42f1d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="42f1d-116">Application</span></span> | <span data-ttu-id="42f1d-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42f1d-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="42f1d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42f1d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```

## <a name="request-headers"></a><span data-ttu-id="42f1d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="42f1d-119">Request headers</span></span>
| <span data-ttu-id="42f1d-120">标头</span><span class="sxs-lookup"><span data-stu-id="42f1d-120">Header</span></span>       | <span data-ttu-id="42f1d-121">值</span><span class="sxs-lookup"><span data-stu-id="42f1d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="42f1d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="42f1d-122">Authorization</span></span>  | <span data-ttu-id="42f1d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="42f1d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="42f1d-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="42f1d-125">Prefer</span></span> | <span data-ttu-id="42f1d-126">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="42f1d-126">return=minimal.</span></span> <span data-ttu-id="42f1d-127">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="42f1d-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="42f1d-128">可选。</span><span class="sxs-lookup"><span data-stu-id="42f1d-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="42f1d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="42f1d-129">Request body</span></span>
 <span data-ttu-id="42f1d-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="42f1d-130">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="42f1d-131">响应</span><span class="sxs-lookup"><span data-stu-id="42f1d-131">Response</span></span>
<span data-ttu-id="42f1d-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="42f1d-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42f1d-134">示例</span><span class="sxs-lookup"><span data-stu-id="42f1d-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="42f1d-135">请求</span><span class="sxs-lookup"><span data-stu-id="42f1d-135">Request</span></span>
<span data-ttu-id="42f1d-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="42f1d-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/unsubscribeByMail
```

#### <a name="response"></a><span data-ttu-id="42f1d-137">响应</span><span class="sxs-lookup"><span data-stu-id="42f1d-137">Response</span></span>
<span data-ttu-id="42f1d-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="42f1d-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: unsubscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
