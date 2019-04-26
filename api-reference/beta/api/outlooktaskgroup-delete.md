---
title: 删除 outlookTaskGroup
description: 删除指定的 outlookTaskGroup。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 82e7b1d71bc57e9eb54232e108fed8ad230dfe9a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337822"
---
# <a name="delete-outlooktaskgroup"></a><span data-ttu-id="d2a4e-103">删除 outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="d2a4e-103">Delete outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2a4e-104">删除指定的[outlookTaskGroup](../resources/outlooktaskgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="d2a4e-104">Delete the specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="d2a4e-105">权限</span><span class="sxs-lookup"><span data-stu-id="d2a4e-105">Permissions</span></span>
<span data-ttu-id="d2a4e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2a4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2a4e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2a4e-108">Permission type</span></span>      | <span data-ttu-id="d2a4e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d2a4e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2a4e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2a4e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d2a4e-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2a4e-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d2a4e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2a4e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2a4e-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2a4e-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d2a4e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2a4e-114">Application</span></span> | <span data-ttu-id="d2a4e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2a4e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2a4e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2a4e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/taskGroups/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d2a4e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2a4e-117">Request headers</span></span>
| <span data-ttu-id="d2a4e-118">名称</span><span class="sxs-lookup"><span data-stu-id="d2a4e-118">Name</span></span>       | <span data-ttu-id="d2a4e-119">说明</span><span class="sxs-lookup"><span data-stu-id="d2a4e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d2a4e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2a4e-120">Authorization</span></span>  | <span data-ttu-id="d2a4e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d2a4e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2a4e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2a4e-123">Request body</span></span>
<span data-ttu-id="d2a4e-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d2a4e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2a4e-125">响应</span><span class="sxs-lookup"><span data-stu-id="d2a4e-125">Response</span></span>

<span data-ttu-id="d2a4e-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d2a4e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2a4e-128">示例</span><span class="sxs-lookup"><span data-stu-id="d2a4e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2a4e-129">请求</span><span class="sxs-lookup"><span data-stu-id="d2a4e-129">Request</span></span>
<span data-ttu-id="d2a4e-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d2a4e-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=
```
##### <a name="response"></a><span data-ttu-id="d2a4e-131">响应</span><span class="sxs-lookup"><span data-stu-id="d2a4e-131">Response</span></span>
<span data-ttu-id="d2a4e-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d2a4e-132">Here is an example of the response.</span></span>
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
  "description": "Delete outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
