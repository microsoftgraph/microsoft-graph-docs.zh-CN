---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 签出文件
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: aaee21e48cba0a317600e2d1a5ab3fc29e9c02c4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589251"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="37f55-102">签出 DriveItem 资源</span><span class="sxs-lookup"><span data-stu-id="37f55-102">Check-out a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37f55-103">签出 driveItem 资源以防止在[签入](driveitem-checkin.md)文档前其他人编辑文档和看到所做的更改。</span><span class="sxs-lookup"><span data-stu-id="37f55-103">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="37f55-104">权限</span><span class="sxs-lookup"><span data-stu-id="37f55-104">Permissions</span></span>

<span data-ttu-id="37f55-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="37f55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37f55-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="37f55-107">Permission type</span></span>      | <span data-ttu-id="37f55-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="37f55-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37f55-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37f55-109">Delegated (work or school account)</span></span> | <span data-ttu-id="37f55-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37f55-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="37f55-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37f55-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37f55-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37f55-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="37f55-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="37f55-113">Application</span></span> | <span data-ttu-id="37f55-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37f55-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37f55-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37f55-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="37f55-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="37f55-116">Request body</span></span>

<span data-ttu-id="37f55-117">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="37f55-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="37f55-118">示例</span><span class="sxs-lookup"><span data-stu-id="37f55-118">Example</span></span>

<span data-ttu-id="37f55-119">本示例签出由 `{item-id}` 标识的文件。</span><span class="sxs-lookup"><span data-stu-id="37f55-119">This example checks out a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```

## <a name="response"></a><span data-ttu-id="37f55-120">响应</span><span class="sxs-lookup"><span data-stu-id="37f55-120">Response</span></span>

<span data-ttu-id="37f55-121">如果成功，该 API 调用会返回 `204 No content`。</span><span class="sxs-lookup"><span data-stu-id="37f55-121">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="37f55-122">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="37f55-122">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="37f55-123">语言</span><span class="sxs-lookup"><span data-stu-id="37f55-123">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/checkout-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="37f55-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="37f55-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/checkout-item-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="remarks"></a><span data-ttu-id="37f55-125">注解</span><span class="sxs-lookup"><span data-stu-id="37f55-125">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-checkout.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-checkout.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
