---
title: 删除页面
description: 删除 OneNote 页面。
ms.openlocfilehash: 574fa3a84a3ca18a788035e4a90bcc833907014e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009537"
---
# <a name="delete-page"></a><span data-ttu-id="d22ab-103">删除页面</span><span class="sxs-lookup"><span data-stu-id="d22ab-103">Delete page</span></span>

<span data-ttu-id="d22ab-104">删除 OneNote 页面。</span><span class="sxs-lookup"><span data-stu-id="d22ab-104">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="d22ab-105">权限</span><span class="sxs-lookup"><span data-stu-id="d22ab-105">Permissions</span></span>
<span data-ttu-id="d22ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d22ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d22ab-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d22ab-108">Permission type</span></span>      | <span data-ttu-id="d22ab-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d22ab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d22ab-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d22ab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d22ab-111">Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d22ab-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="d22ab-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d22ab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d22ab-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d22ab-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="d22ab-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d22ab-114">Application</span></span> | <span data-ttu-id="d22ab-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d22ab-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d22ab-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d22ab-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d22ab-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d22ab-117">Request headers</span></span>
| <span data-ttu-id="d22ab-118">名称</span><span class="sxs-lookup"><span data-stu-id="d22ab-118">Name</span></span>       | <span data-ttu-id="d22ab-119">类型</span><span class="sxs-lookup"><span data-stu-id="d22ab-119">Type</span></span> | <span data-ttu-id="d22ab-120">说明</span><span class="sxs-lookup"><span data-stu-id="d22ab-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d22ab-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d22ab-121">Authorization</span></span>  | <span data-ttu-id="d22ab-122">string</span><span class="sxs-lookup"><span data-stu-id="d22ab-122">string</span></span>  | <span data-ttu-id="d22ab-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d22ab-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d22ab-125">响应</span><span class="sxs-lookup"><span data-stu-id="d22ab-125">Response</span></span>

<span data-ttu-id="d22ab-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d22ab-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d22ab-128">示例</span><span class="sxs-lookup"><span data-stu-id="d22ab-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d22ab-129">请求</span><span class="sxs-lookup"><span data-stu-id="d22ab-129">Request</span></span>
<span data-ttu-id="d22ab-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d22ab-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="d22ab-131">响应</span><span class="sxs-lookup"><span data-stu-id="d22ab-131">Response</span></span>
<span data-ttu-id="d22ab-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d22ab-132">Here is an example of the response.</span></span>
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