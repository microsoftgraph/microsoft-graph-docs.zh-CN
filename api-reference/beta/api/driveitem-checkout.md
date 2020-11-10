---
author: JeremyKelley
description: 签出 driveItem 资源，以防止其他人编辑该文档，并且在文档签入前，您所做的更改将一直可见。
title: driveItem：签出
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8697f139243c59bd05d88612293645bfb42733ef
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963843"
---
# <a name="driveitem-checkout"></a><span data-ttu-id="dba85-103">driveItem：签出</span><span class="sxs-lookup"><span data-stu-id="dba85-103">driveItem: checkout</span></span>

<span data-ttu-id="dba85-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dba85-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dba85-105">签出 **driveItem** 资源，以防止其他人编辑该文档，并在 [签](driveitem-checkin.md)入所记录的文档之前阻止您的更改可见。</span><span class="sxs-lookup"><span data-stu-id="dba85-105">Check out a **driveItem** resource to prevent others from editing the document, and prevent your changes from being visible until the documented is [checked in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dba85-106">权限</span><span class="sxs-lookup"><span data-stu-id="dba85-106">Permissions</span></span>

<span data-ttu-id="dba85-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dba85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dba85-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dba85-109">Permission type</span></span>      | <span data-ttu-id="dba85-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dba85-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dba85-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dba85-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dba85-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dba85-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="dba85-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dba85-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dba85-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dba85-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="dba85-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dba85-115">Application</span></span> | <span data-ttu-id="dba85-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dba85-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dba85-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dba85-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="dba85-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="dba85-118">Request body</span></span>

<span data-ttu-id="dba85-119">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="dba85-119">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="dba85-120">示例</span><span class="sxs-lookup"><span data-stu-id="dba85-120">Example</span></span>

<span data-ttu-id="dba85-121">本示例签出由 `{item-id}` 标识的文件。</span><span class="sxs-lookup"><span data-stu-id="dba85-121">This example checks out a file identified by `{item-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="dba85-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="dba85-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```
# <a name="c"></a>[<span data-ttu-id="dba85-123">C#</span><span class="sxs-lookup"><span data-stu-id="dba85-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkout-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dba85-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dba85-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkout-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dba85-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dba85-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkout-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dba85-126">Java</span><span class="sxs-lookup"><span data-stu-id="dba85-126">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/checkout-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="dba85-127">响应</span><span class="sxs-lookup"><span data-stu-id="dba85-127">Response</span></span>

<span data-ttu-id="dba85-128">如果成功，API 调用将返回 `204 No content` 。</span><span class="sxs-lookup"><span data-stu-id="dba85-128">If successful, the API call returns `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="dba85-129">注解</span><span class="sxs-lookup"><span data-stu-id="dba85-129">Remarks</span></span>


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


