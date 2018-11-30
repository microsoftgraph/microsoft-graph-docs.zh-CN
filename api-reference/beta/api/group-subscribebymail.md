---
title: 组：subscribeByMail
description: 调用此方法将使当前用户可以接收电子邮件通知，对此组，有关新帖子、 事件和文件组中。 Office 365 组仅支持。
ms.openlocfilehash: 3e43f3805974fa518bf006682e8dd1f211e20417
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048098"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="d1778-104">组：subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="d1778-104">group: subscribeByMail</span></span>

> <span data-ttu-id="d1778-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d1778-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1778-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d1778-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1778-107">调用此方法将使当前用户可以接收电子邮件通知，对此组，有关新帖子、 事件和文件组中。</span><span class="sxs-lookup"><span data-stu-id="d1778-107">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group.</span></span> <span data-ttu-id="d1778-108">Office 365 组仅支持。</span><span class="sxs-lookup"><span data-stu-id="d1778-108">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1778-109">权限</span><span class="sxs-lookup"><span data-stu-id="d1778-109">Permissions</span></span>
<span data-ttu-id="d1778-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d1778-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1778-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1778-112">Permission type</span></span>      | <span data-ttu-id="d1778-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d1778-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1778-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1778-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d1778-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1778-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d1778-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1778-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1778-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1778-117">Not supported.</span></span>    |
|<span data-ttu-id="d1778-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1778-118">Application</span></span> | <span data-ttu-id="d1778-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1778-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1778-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1778-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="d1778-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1778-121">Request headers</span></span>
| <span data-ttu-id="d1778-122">标头</span><span class="sxs-lookup"><span data-stu-id="d1778-122">Header</span></span>       | <span data-ttu-id="d1778-123">值</span><span class="sxs-lookup"><span data-stu-id="d1778-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d1778-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1778-124">Authorization</span></span>  | <span data-ttu-id="d1778-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d1778-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d1778-127">Prefer</span><span class="sxs-lookup"><span data-stu-id="d1778-127">Prefer</span></span> | <span data-ttu-id="d1778-128">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="d1778-128">return=minimal.</span></span> <span data-ttu-id="d1778-129">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="d1778-129">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="d1778-130">可选。</span><span class="sxs-lookup"><span data-stu-id="d1778-130">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="d1778-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1778-131">Request body</span></span>

## <a name="response"></a><span data-ttu-id="d1778-132">响应</span><span class="sxs-lookup"><span data-stu-id="d1778-132">Response</span></span>
<span data-ttu-id="d1778-p107">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d1778-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1778-135">示例</span><span class="sxs-lookup"><span data-stu-id="d1778-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d1778-136">请求</span><span class="sxs-lookup"><span data-stu-id="d1778-136">Request</span></span>
<span data-ttu-id="d1778-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d1778-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/subscribeByMail
```

#### <a name="response"></a><span data-ttu-id="d1778-138">响应</span><span class="sxs-lookup"><span data-stu-id="d1778-138">Response</span></span>
<span data-ttu-id="d1778-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d1778-139">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->