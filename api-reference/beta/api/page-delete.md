---
title: 删除页面
description: 删除 OneNote 页面。
localization_priority: Normal
ms.openlocfilehash: 5721f06f34be48f0c8a3126d82e858aa833d3e77
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853548"
---
# <a name="delete-page"></a><span data-ttu-id="62d0c-103">删除页面</span><span class="sxs-lookup"><span data-stu-id="62d0c-103">Delete page</span></span>

> <span data-ttu-id="62d0c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="62d0c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="62d0c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="62d0c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="62d0c-106">删除 OneNote 页面。</span><span class="sxs-lookup"><span data-stu-id="62d0c-106">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="62d0c-107">权限</span><span class="sxs-lookup"><span data-stu-id="62d0c-107">Permissions</span></span>
<span data-ttu-id="62d0c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62d0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62d0c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="62d0c-110">Permission type</span></span>      | <span data-ttu-id="62d0c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62d0c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62d0c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62d0c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="62d0c-113">Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62d0c-113">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="62d0c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62d0c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62d0c-115">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62d0c-115">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="62d0c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="62d0c-116">Application</span></span> | <span data-ttu-id="62d0c-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62d0c-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62d0c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62d0c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="62d0c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="62d0c-119">Request headers</span></span>
| <span data-ttu-id="62d0c-120">名称</span><span class="sxs-lookup"><span data-stu-id="62d0c-120">Name</span></span>       | <span data-ttu-id="62d0c-121">类型</span><span class="sxs-lookup"><span data-stu-id="62d0c-121">Type</span></span> | <span data-ttu-id="62d0c-122">说明</span><span class="sxs-lookup"><span data-stu-id="62d0c-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="62d0c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="62d0c-123">Authorization</span></span>  | <span data-ttu-id="62d0c-124">string</span><span class="sxs-lookup"><span data-stu-id="62d0c-124">string</span></span>  | <span data-ttu-id="62d0c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="62d0c-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="62d0c-127">响应</span><span class="sxs-lookup"><span data-stu-id="62d0c-127">Response</span></span>

<span data-ttu-id="62d0c-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="62d0c-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62d0c-130">示例</span><span class="sxs-lookup"><span data-stu-id="62d0c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="62d0c-131">请求</span><span class="sxs-lookup"><span data-stu-id="62d0c-131">Request</span></span>
<span data-ttu-id="62d0c-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="62d0c-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="62d0c-133">响应</span><span class="sxs-lookup"><span data-stu-id="62d0c-133">Response</span></span>
<span data-ttu-id="62d0c-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="62d0c-134">Here is an example of the response.</span></span>
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
  "description": "Delete page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
