---
title: 删除页面
description: 删除 OneNote 页面。
localization_priority: Normal
ms.openlocfilehash: fc2a4a9e809cb3a335c795a27cb5ffe35487a880
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810008"
---
# <a name="delete-page"></a><span data-ttu-id="78414-103">删除页面</span><span class="sxs-lookup"><span data-stu-id="78414-103">Delete page</span></span>

<span data-ttu-id="78414-104">删除 OneNote 页面。</span><span class="sxs-lookup"><span data-stu-id="78414-104">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="78414-105">权限</span><span class="sxs-lookup"><span data-stu-id="78414-105">Permissions</span></span>
<span data-ttu-id="78414-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78414-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78414-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="78414-108">Permission type</span></span>      | <span data-ttu-id="78414-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="78414-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78414-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78414-110">Delegated (work or school account)</span></span> | <span data-ttu-id="78414-111">Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78414-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="78414-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78414-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78414-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78414-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="78414-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="78414-114">Application</span></span> | <span data-ttu-id="78414-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78414-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="78414-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78414-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="78414-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="78414-117">Request headers</span></span>
| <span data-ttu-id="78414-118">名称</span><span class="sxs-lookup"><span data-stu-id="78414-118">Name</span></span>       | <span data-ttu-id="78414-119">类型</span><span class="sxs-lookup"><span data-stu-id="78414-119">Type</span></span> | <span data-ttu-id="78414-120">说明</span><span class="sxs-lookup"><span data-stu-id="78414-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="78414-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="78414-121">Authorization</span></span>  | <span data-ttu-id="78414-122">string</span><span class="sxs-lookup"><span data-stu-id="78414-122">string</span></span>  | <span data-ttu-id="78414-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="78414-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="78414-125">响应</span><span class="sxs-lookup"><span data-stu-id="78414-125">Response</span></span>

<span data-ttu-id="78414-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="78414-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78414-128">示例</span><span class="sxs-lookup"><span data-stu-id="78414-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78414-129">请求</span><span class="sxs-lookup"><span data-stu-id="78414-129">Request</span></span>
<span data-ttu-id="78414-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="78414-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="78414-131">响应</span><span class="sxs-lookup"><span data-stu-id="78414-131">Response</span></span>
<span data-ttu-id="78414-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="78414-132">Here is an example of the response.</span></span>
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
