---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 签出文件
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e92af4dea2e5b0678e72bc3311042acba9266a5b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861402"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="f6dd5-102">签出 DriveItem 资源</span><span class="sxs-lookup"><span data-stu-id="f6dd5-102">Check-out a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6dd5-103">签出 driveItem 资源以防止在[签入](driveitem-checkin.md)文档前其他人编辑文档和看到所做的更改。</span><span class="sxs-lookup"><span data-stu-id="f6dd5-103">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f6dd5-104">权限</span><span class="sxs-lookup"><span data-stu-id="f6dd5-104">Permissions</span></span>

<span data-ttu-id="f6dd5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6dd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6dd5-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6dd5-107">Permission type</span></span>      | <span data-ttu-id="f6dd5-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f6dd5-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6dd5-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6dd5-109">Delegated (work or school account)</span></span> | <span data-ttu-id="f6dd5-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6dd5-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f6dd5-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6dd5-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6dd5-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6dd5-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f6dd5-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6dd5-113">Application</span></span> | <span data-ttu-id="f6dd5-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6dd5-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6dd5-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6dd5-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="f6dd5-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6dd5-116">Request body</span></span>

<span data-ttu-id="f6dd5-117">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="f6dd5-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="f6dd5-118">示例</span><span class="sxs-lookup"><span data-stu-id="f6dd5-118">Example</span></span>

<span data-ttu-id="f6dd5-119">本示例签出由 `{item-id}` 标识的文件。</span><span class="sxs-lookup"><span data-stu-id="f6dd5-119">This example checks out a file identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f6dd5-120">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f6dd5-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f6dd5-121">C#</span><span class="sxs-lookup"><span data-stu-id="f6dd5-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkout-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f6dd5-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="f6dd5-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkout-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f6dd5-123">目标-C</span><span class="sxs-lookup"><span data-stu-id="f6dd5-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkout-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f6dd5-124">Java</span><span class="sxs-lookup"><span data-stu-id="f6dd5-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/checkout-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="f6dd5-125">响应</span><span class="sxs-lookup"><span data-stu-id="f6dd5-125">Response</span></span>

<span data-ttu-id="f6dd5-126">如果成功，该 API 调用会返回 `204 No content`。</span><span class="sxs-lookup"><span data-stu-id="f6dd5-126">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="f6dd5-127">注解</span><span class="sxs-lookup"><span data-stu-id="f6dd5-127">Remarks</span></span>


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
