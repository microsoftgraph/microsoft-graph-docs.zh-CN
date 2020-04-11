---
author: learafa
description: 签出 driveItem 资源，以防止其他人编辑该文档，并且在文档签入前，您所做的更改将一直可见。
title: driveItem：签出
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 411cab13272927335d58e48112a1e2a5d856ffea
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229107"
---
# <a name="driveitem-checkout"></a><span data-ttu-id="4421e-103">driveItem：签出</span><span class="sxs-lookup"><span data-stu-id="4421e-103">driveItem: checkout</span></span>

<span data-ttu-id="4421e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4421e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4421e-105">签出**driveItem**资源，以防止其他人编辑该文档，并在[签](driveitem-checkin.md)入所记录的文档之前阻止您的更改可见。</span><span class="sxs-lookup"><span data-stu-id="4421e-105">Check out a **driveItem** resource to prevent others from editing the document, and prevent your changes from being visible until the documented is [checked in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4421e-106">权限</span><span class="sxs-lookup"><span data-stu-id="4421e-106">Permissions</span></span>

<span data-ttu-id="4421e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4421e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4421e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4421e-109">Permission type</span></span>      | <span data-ttu-id="4421e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4421e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4421e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4421e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4421e-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4421e-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4421e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4421e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4421e-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4421e-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="4421e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4421e-115">Application</span></span> | <span data-ttu-id="4421e-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4421e-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4421e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4421e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

## <a name="request-body"></a><span data-ttu-id="4421e-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="4421e-118">Request body</span></span>

<span data-ttu-id="4421e-119">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4421e-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4421e-120">响应</span><span class="sxs-lookup"><span data-stu-id="4421e-120">Response</span></span>

<span data-ttu-id="4421e-121">如果成功，API 调用将返回`204 No content`。</span><span class="sxs-lookup"><span data-stu-id="4421e-121">If successful, the API call returns `204 No content`.</span></span>

## <a name="example"></a><span data-ttu-id="4421e-122">示例</span><span class="sxs-lookup"><span data-stu-id="4421e-122">Example</span></span>

<span data-ttu-id="4421e-123">本示例签出由 `{item-id}` 标识的文件。</span><span class="sxs-lookup"><span data-stu-id="4421e-123">This example checks out a file identified by `{item-id}`.</span></span>

### <a name="request"></a><span data-ttu-id="4421e-124">请求</span><span class="sxs-lookup"><span data-stu-id="4421e-124">Request</span></span>

<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```

### <a name="response"></a><span data-ttu-id="4421e-125">响应</span><span class="sxs-lookup"><span data-stu-id="4421e-125">Response</span></span>

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
