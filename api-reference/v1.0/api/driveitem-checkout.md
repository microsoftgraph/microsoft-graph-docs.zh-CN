---
author: learafa
description: 签出 driveItem 资源，以防止其他人编辑该文档，并且在文档签入前，您所做的更改将一直可见。
title: driveItem：签出
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 60b9f5de40f925354a0513c1b467295bf24ccb85
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009896"
---
# <a name="driveitem-checkout"></a><span data-ttu-id="dd3bb-103">driveItem：签出</span><span class="sxs-lookup"><span data-stu-id="dd3bb-103">driveItem: checkout</span></span>

<span data-ttu-id="dd3bb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd3bb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd3bb-105">签出 **driveItem** 资源，以防止其他人编辑该文档，并在 [签](driveitem-checkin.md)入所记录的文档之前阻止您的更改可见。</span><span class="sxs-lookup"><span data-stu-id="dd3bb-105">Check out a **driveItem** resource to prevent others from editing the document, and prevent your changes from being visible until the documented is [checked in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dd3bb-106">权限</span><span class="sxs-lookup"><span data-stu-id="dd3bb-106">Permissions</span></span>

<span data-ttu-id="dd3bb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd3bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd3bb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd3bb-109">Permission type</span></span>      | <span data-ttu-id="dd3bb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dd3bb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd3bb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd3bb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dd3bb-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd3bb-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="dd3bb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd3bb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd3bb-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd3bb-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="dd3bb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd3bb-115">Application</span></span> | <span data-ttu-id="dd3bb-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd3bb-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd3bb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd3bb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

## <a name="request-body"></a><span data-ttu-id="dd3bb-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd3bb-118">Request body</span></span>

<span data-ttu-id="dd3bb-119">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dd3bb-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd3bb-120">响应</span><span class="sxs-lookup"><span data-stu-id="dd3bb-120">Response</span></span>

<span data-ttu-id="dd3bb-121">如果成功，API 调用将返回 `204 No content` 。</span><span class="sxs-lookup"><span data-stu-id="dd3bb-121">If successful, the API call returns `204 No content`.</span></span>

## <a name="example"></a><span data-ttu-id="dd3bb-122">示例</span><span class="sxs-lookup"><span data-stu-id="dd3bb-122">Example</span></span>

<span data-ttu-id="dd3bb-123">本示例签出由 `{item-id}` 标识的文件。</span><span class="sxs-lookup"><span data-stu-id="dd3bb-123">This example checks out a file identified by `{item-id}`.</span></span>

### <a name="request"></a><span data-ttu-id="dd3bb-124">请求</span><span class="sxs-lookup"><span data-stu-id="dd3bb-124">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="dd3bb-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd3bb-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```
# <a name="c"></a>[<span data-ttu-id="dd3bb-126">C#</span><span class="sxs-lookup"><span data-stu-id="dd3bb-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkout-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd3bb-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd3bb-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkout-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd3bb-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd3bb-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkout-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd3bb-129">Java</span><span class="sxs-lookup"><span data-stu-id="dd3bb-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/checkout-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dd3bb-130">响应</span><span class="sxs-lookup"><span data-stu-id="dd3bb-130">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```


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

