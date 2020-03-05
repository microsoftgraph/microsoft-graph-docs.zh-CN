---
author: JeremyKelley
description: 签出 driveItem 资源以防止在签入文档前其他人编辑文档和看到所做的更改。
ms.date: 09/10/2017
title: 签出文件
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 4159882b29dc69429a7b99bb89d1e8051d6e9c03
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42432941"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="f7c70-103">签出 DriveItem 资源</span><span class="sxs-lookup"><span data-stu-id="f7c70-103">Check-out a DriveItem resource</span></span>

<span data-ttu-id="f7c70-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f7c70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7c70-105">签出 driveItem 资源以防止在[签入](driveitem-checkin.md)文档前其他人编辑文档和看到所做的更改。</span><span class="sxs-lookup"><span data-stu-id="f7c70-105">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f7c70-106">权限</span><span class="sxs-lookup"><span data-stu-id="f7c70-106">Permissions</span></span>

<span data-ttu-id="f7c70-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7c70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7c70-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7c70-109">Permission type</span></span>      | <span data-ttu-id="f7c70-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7c70-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7c70-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7c70-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f7c70-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7c70-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7c70-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7c70-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7c70-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7c70-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7c70-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7c70-115">Application</span></span> | <span data-ttu-id="f7c70-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7c70-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7c70-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7c70-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="f7c70-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7c70-118">Request body</span></span>

<span data-ttu-id="f7c70-119">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="f7c70-119">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="f7c70-120">示例</span><span class="sxs-lookup"><span data-stu-id="f7c70-120">Example</span></span>

<span data-ttu-id="f7c70-121">本示例签出由 `{item-id}` 标识的文件。</span><span class="sxs-lookup"><span data-stu-id="f7c70-121">This example checks out a file identified by `{item-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="f7c70-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7c70-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```
# <a name="c"></a>[<span data-ttu-id="f7c70-123">C#</span><span class="sxs-lookup"><span data-stu-id="f7c70-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkout-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7c70-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7c70-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkout-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7c70-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7c70-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkout-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="f7c70-126">响应</span><span class="sxs-lookup"><span data-stu-id="f7c70-126">Response</span></span>

<span data-ttu-id="f7c70-127">如果成功，该 API 调用会返回 `204 No content`。</span><span class="sxs-lookup"><span data-stu-id="f7c70-127">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="f7c70-128">注解</span><span class="sxs-lookup"><span data-stu-id="f7c70-128">Remarks</span></span>


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
