---
title: 删除页面
description: 删除 OneNote 页面。
ms.openlocfilehash: f2e566696937ee6f7808a66f994298802be66a17
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042975"
---
# <a name="delete-page"></a><span data-ttu-id="a9e16-103">删除页面</span><span class="sxs-lookup"><span data-stu-id="a9e16-103">Delete page</span></span>

> <span data-ttu-id="a9e16-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a9e16-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9e16-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a9e16-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a9e16-106">删除 OneNote 页面。</span><span class="sxs-lookup"><span data-stu-id="a9e16-106">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="a9e16-107">权限</span><span class="sxs-lookup"><span data-stu-id="a9e16-107">Permissions</span></span>
<span data-ttu-id="a9e16-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9e16-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9e16-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9e16-110">Permission type</span></span>      | <span data-ttu-id="a9e16-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a9e16-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9e16-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9e16-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a9e16-113">Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9e16-113">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a9e16-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9e16-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9e16-115">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9e16-115">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="a9e16-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9e16-116">Application</span></span> | <span data-ttu-id="a9e16-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9e16-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9e16-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9e16-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a9e16-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9e16-119">Request headers</span></span>
| <span data-ttu-id="a9e16-120">名称</span><span class="sxs-lookup"><span data-stu-id="a9e16-120">Name</span></span>       | <span data-ttu-id="a9e16-121">类型</span><span class="sxs-lookup"><span data-stu-id="a9e16-121">Type</span></span> | <span data-ttu-id="a9e16-122">说明</span><span class="sxs-lookup"><span data-stu-id="a9e16-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a9e16-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9e16-123">Authorization</span></span>  | <span data-ttu-id="a9e16-124">string</span><span class="sxs-lookup"><span data-stu-id="a9e16-124">string</span></span>  | <span data-ttu-id="a9e16-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a9e16-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a9e16-127">响应</span><span class="sxs-lookup"><span data-stu-id="a9e16-127">Response</span></span>

<span data-ttu-id="a9e16-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a9e16-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9e16-130">示例</span><span class="sxs-lookup"><span data-stu-id="a9e16-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9e16-131">请求</span><span class="sxs-lookup"><span data-stu-id="a9e16-131">Request</span></span>
<span data-ttu-id="a9e16-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a9e16-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="a9e16-133">响应</span><span class="sxs-lookup"><span data-stu-id="a9e16-133">Response</span></span>
<span data-ttu-id="a9e16-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a9e16-134">Here is an example of the response.</span></span>
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