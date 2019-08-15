---
author: JeremyKelley
description: 签出 driveItem 资源以防止在签入文档前其他人编辑文档和看到所做的更改。
ms.date: 09/10/2017
title: 签出文件
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: adde2c3deb03bf1f45a673ff6cc5d6d7a844544e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416861"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="16e7e-103">签出 DriveItem 资源</span><span class="sxs-lookup"><span data-stu-id="16e7e-103">Check-out a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16e7e-104">签出 driveItem 资源以防止在[签入](driveitem-checkin.md)文档前其他人编辑文档和看到所做的更改。</span><span class="sxs-lookup"><span data-stu-id="16e7e-104">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="16e7e-105">权限</span><span class="sxs-lookup"><span data-stu-id="16e7e-105">Permissions</span></span>

<span data-ttu-id="16e7e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16e7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16e7e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="16e7e-108">Permission type</span></span>      | <span data-ttu-id="16e7e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16e7e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16e7e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16e7e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="16e7e-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16e7e-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="16e7e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16e7e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16e7e-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16e7e-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="16e7e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="16e7e-114">Application</span></span> | <span data-ttu-id="16e7e-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16e7e-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16e7e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16e7e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="16e7e-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="16e7e-117">Request body</span></span>

<span data-ttu-id="16e7e-118">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="16e7e-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="16e7e-119">示例</span><span class="sxs-lookup"><span data-stu-id="16e7e-119">Example</span></span>

<span data-ttu-id="16e7e-120">本示例签出由 `{item-id}` 标识的文件。</span><span class="sxs-lookup"><span data-stu-id="16e7e-120">This example checks out a file identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="16e7e-121">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="16e7e-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="16e7e-122">C#</span><span class="sxs-lookup"><span data-stu-id="16e7e-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkout-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="16e7e-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16e7e-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkout-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="16e7e-124">目标-C</span><span class="sxs-lookup"><span data-stu-id="16e7e-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkout-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="16e7e-125">响应</span><span class="sxs-lookup"><span data-stu-id="16e7e-125">Response</span></span>

<span data-ttu-id="16e7e-126">如果成功，该 API 调用会返回 `204 No content`。</span><span class="sxs-lookup"><span data-stu-id="16e7e-126">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="16e7e-127">注解</span><span class="sxs-lookup"><span data-stu-id="16e7e-127">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
}
-->
