---
title: 删除 outlookTask
description: 删除用户的邮箱中指定的 Outlook 任务。
localization_priority: Normal
ms.openlocfilehash: cac976349f375360bf6e3dcd5e0e86d9b1a855af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807134"
---
# <a name="delete-outlooktask"></a><span data-ttu-id="deb4b-103">删除 outlookTask</span><span class="sxs-lookup"><span data-stu-id="deb4b-103">Delete outlookTask</span></span>

> <span data-ttu-id="deb4b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="deb4b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="deb4b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="deb4b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="deb4b-106">删除用户的邮箱中指定的 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="deb4b-106">Delete the specified Outlook task in the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="deb4b-107">权限</span><span class="sxs-lookup"><span data-stu-id="deb4b-107">Permissions</span></span>

<span data-ttu-id="deb4b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="deb4b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="deb4b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="deb4b-110">Permission type</span></span>      | <span data-ttu-id="deb4b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="deb4b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="deb4b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="deb4b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="deb4b-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="deb4b-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="deb4b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="deb4b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="deb4b-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="deb4b-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="deb4b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="deb4b-116">Application</span></span> | <span data-ttu-id="deb4b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="deb4b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="deb4b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="deb4b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/{id}
DELETE /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="deb4b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="deb4b-119">Request headers</span></span>

| <span data-ttu-id="deb4b-120">名称</span><span class="sxs-lookup"><span data-stu-id="deb4b-120">Name</span></span>       | <span data-ttu-id="deb4b-121">说明</span><span class="sxs-lookup"><span data-stu-id="deb4b-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="deb4b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="deb4b-122">Authorization</span></span>  | <span data-ttu-id="deb4b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="deb4b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="deb4b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="deb4b-125">Request body</span></span>

<span data-ttu-id="deb4b-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="deb4b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="deb4b-127">响应</span><span class="sxs-lookup"><span data-stu-id="deb4b-127">Response</span></span>

<span data-ttu-id="deb4b-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="deb4b-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="deb4b-130">示例</span><span class="sxs-lookup"><span data-stu-id="deb4b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="deb4b-131">请求</span><span class="sxs-lookup"><span data-stu-id="deb4b-131">Request</span></span>

<span data-ttu-id="deb4b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="deb4b-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktask"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADIyAAAhrb_QAAA=')
```

### <a name="response"></a><span data-ttu-id="deb4b-133">响应</span><span class="sxs-lookup"><span data-stu-id="deb4b-133">Response</span></span>

<span data-ttu-id="deb4b-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="deb4b-134">Here is an example of the response.</span></span>
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
  "description": "Delete outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
