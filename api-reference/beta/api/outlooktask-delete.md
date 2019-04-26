---
title: 删除 outlookTask
description: 删除用户邮箱中的指定 Outlook 任务。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 5cce9b291c75324796cead54cbe137d50e850075
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332739"
---
# <a name="delete-outlooktask"></a><span data-ttu-id="a9248-103">删除 outlookTask</span><span class="sxs-lookup"><span data-stu-id="a9248-103">Delete outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9248-104">删除用户邮箱中的指定 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="a9248-104">Delete the specified Outlook task in the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9248-105">权限</span><span class="sxs-lookup"><span data-stu-id="a9248-105">Permissions</span></span>

<span data-ttu-id="a9248-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9248-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9248-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9248-108">Permission type</span></span>      | <span data-ttu-id="a9248-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a9248-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9248-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9248-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a9248-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9248-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a9248-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9248-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9248-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9248-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a9248-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9248-114">Application</span></span> | <span data-ttu-id="a9248-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9248-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9248-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9248-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/{id}
DELETE /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a9248-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9248-117">Request headers</span></span>

| <span data-ttu-id="a9248-118">名称</span><span class="sxs-lookup"><span data-stu-id="a9248-118">Name</span></span>       | <span data-ttu-id="a9248-119">说明</span><span class="sxs-lookup"><span data-stu-id="a9248-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a9248-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9248-120">Authorization</span></span>  | <span data-ttu-id="a9248-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a9248-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9248-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9248-123">Request body</span></span>

<span data-ttu-id="a9248-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a9248-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9248-125">响应</span><span class="sxs-lookup"><span data-stu-id="a9248-125">Response</span></span>

<span data-ttu-id="a9248-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a9248-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9248-128">示例</span><span class="sxs-lookup"><span data-stu-id="a9248-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9248-129">请求</span><span class="sxs-lookup"><span data-stu-id="a9248-129">Request</span></span>

<span data-ttu-id="a9248-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a9248-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktask"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADIyAAAhrb_QAAA=
```

### <a name="response"></a><span data-ttu-id="a9248-131">响应</span><span class="sxs-lookup"><span data-stu-id="a9248-131">Response</span></span>

<span data-ttu-id="a9248-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a9248-132">Here is an example of the response.</span></span>
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
  "description": "Delete outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
