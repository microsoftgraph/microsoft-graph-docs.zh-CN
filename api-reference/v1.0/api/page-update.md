---
title: 更新页面
description: 更新 OneNote 页面的内容。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ef51342aba7bab49fde6d69ea0c77c62dc841b7d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971709"
---
# <a name="update-page"></a><span data-ttu-id="2d9b2-103">更新页面</span><span class="sxs-lookup"><span data-stu-id="2d9b2-103">Update page</span></span>

<span data-ttu-id="2d9b2-104">更新 OneNote 页面的内容。</span><span class="sxs-lookup"><span data-stu-id="2d9b2-104">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="2d9b2-105">权限</span><span class="sxs-lookup"><span data-stu-id="2d9b2-105">Permissions</span></span>
<span data-ttu-id="2d9b2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d9b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d9b2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d9b2-108">Permission type</span></span>      | <span data-ttu-id="2d9b2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2d9b2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d9b2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d9b2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2d9b2-111">Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d9b2-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="2d9b2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d9b2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d9b2-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d9b2-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="2d9b2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d9b2-114">Application</span></span> | <span data-ttu-id="2d9b2-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d9b2-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d9b2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d9b2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="2d9b2-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d9b2-117">Request headers</span></span>
| <span data-ttu-id="2d9b2-118">名称</span><span class="sxs-lookup"><span data-stu-id="2d9b2-118">Name</span></span>       | <span data-ttu-id="2d9b2-119">类型</span><span class="sxs-lookup"><span data-stu-id="2d9b2-119">Type</span></span> | <span data-ttu-id="2d9b2-120">说明</span><span class="sxs-lookup"><span data-stu-id="2d9b2-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2d9b2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d9b2-121">Authorization</span></span>  | <span data-ttu-id="2d9b2-122">string</span><span class="sxs-lookup"><span data-stu-id="2d9b2-122">string</span></span>  | <span data-ttu-id="2d9b2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2d9b2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2d9b2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2d9b2-125">Content-Type</span></span> | <span data-ttu-id="2d9b2-126">string</span><span class="sxs-lookup"><span data-stu-id="2d9b2-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="2d9b2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d9b2-127">Request body</span></span>
<span data-ttu-id="2d9b2-p103">在请求正文中，提供表示页面更改的 [patchContentCommand](../resources/patchcontentcommand.md) 对象的数组。有关详细信息和示例，请参阅 <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">更新 OneNote 页面</a>。</span><span class="sxs-lookup"><span data-stu-id="2d9b2-p103">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page. For more information and examples, see <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Update OneNote pages</a>.</span></span>

## <a name="response"></a><span data-ttu-id="2d9b2-130">响应</span><span class="sxs-lookup"><span data-stu-id="2d9b2-130">Response</span></span>

<span data-ttu-id="2d9b2-p104">如果成功，此方法返回 `204 No Content` 响应代码。PATCH 请求未返回任何 JSON 数据。</span><span class="sxs-lookup"><span data-stu-id="2d9b2-p104">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="2d9b2-133">示例</span><span class="sxs-lookup"><span data-stu-id="2d9b2-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d9b2-134">请求</span><span class="sxs-lookup"><span data-stu-id="2d9b2-134">Request</span></span>
<span data-ttu-id="2d9b2-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2d9b2-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content
Content-type: application/json
Content-length: 312

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="image-alt-text" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
]
```
##### <a name="response"></a><span data-ttu-id="2d9b2-136">响应</span><span class="sxs-lookup"><span data-stu-id="2d9b2-136">Response</span></span>
<span data-ttu-id="2d9b2-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2d9b2-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotePage"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
