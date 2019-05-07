---
title: 删除照片
description: 删除照片。
localization_priority: Normal
ms.openlocfilehash: 05a679217aea32ee026ef1786c7d6a21689d1cab
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611415"
---
# <a name="delete-photo"></a><span data-ttu-id="3c690-103">删除照片</span><span class="sxs-lookup"><span data-stu-id="3c690-103">Delete photo</span></span>

<span data-ttu-id="3c690-104">删除照片。</span><span class="sxs-lookup"><span data-stu-id="3c690-104">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="3c690-105">权限</span><span class="sxs-lookup"><span data-stu-id="3c690-105">Permissions</span></span>
<span data-ttu-id="3c690-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c690-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c690-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c690-108">Permission type</span></span>      | <span data-ttu-id="3c690-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c690-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c690-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c690-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3c690-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c690-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3c690-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c690-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c690-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c690-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3c690-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c690-114">Application</span></span> | <span data-ttu-id="3c690-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c690-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c690-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c690-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="3c690-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c690-117">Request headers</span></span>
| <span data-ttu-id="3c690-118">名称</span><span class="sxs-lookup"><span data-stu-id="3c690-118">Name</span></span>       | <span data-ttu-id="3c690-119">类型</span><span class="sxs-lookup"><span data-stu-id="3c690-119">Type</span></span> | <span data-ttu-id="3c690-120">说明</span><span class="sxs-lookup"><span data-stu-id="3c690-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3c690-121">if-match</span><span class="sxs-lookup"><span data-stu-id="3c690-121">if-match</span></span>  | <span data-ttu-id="3c690-122">string</span><span class="sxs-lookup"><span data-stu-id="3c690-122">string</span></span>  | <span data-ttu-id="3c690-123">如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="3c690-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="3c690-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c690-124">Authorization</span></span>  | <span data-ttu-id="3c690-125">string</span><span class="sxs-lookup"><span data-stu-id="3c690-125">string</span></span>  | <span data-ttu-id="3c690-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3c690-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c690-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c690-128">Request body</span></span>
<span data-ttu-id="3c690-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3c690-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c690-130">响应</span><span class="sxs-lookup"><span data-stu-id="3c690-130">Response</span></span>

<span data-ttu-id="3c690-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3c690-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c690-133">示例</span><span class="sxs-lookup"><span data-stu-id="3c690-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c690-134">请求</span><span class="sxs-lookup"><span data-stu-id="3c690-134">Request</span></span>
<span data-ttu-id="3c690-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3c690-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
"name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="3c690-136">响应</span><span class="sxs-lookup"><span data-stu-id="3c690-136">Response</span></span>
<span data-ttu-id="3c690-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3c690-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3c690-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="3c690-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3c690-139">语言</span><span class="sxs-lookup"><span data-stu-id="3c690-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_photo-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c690-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="3c690-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_photo-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/photo-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/photo-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
