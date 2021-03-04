---
author: swapnil1993
title: 删除 columnDefinition
description: 从内容类型中删除列。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: fb5df6389c4723cf48185a74f72c1009a3ac031b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446130"
---
# <a name="delete-columndefinition"></a><span data-ttu-id="2c97e-103">删除 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="2c97e-103">Delete columnDefinition</span></span>
<span data-ttu-id="2c97e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c97e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="2c97e-105">从[列表][columndefinition]或[网站][]内容类型[中删除][][列][contentType]。</span><span class="sxs-lookup"><span data-stu-id="2c97e-105">Remove a [column][columndefinition] from a [list][] or a [site][] [content type][contentType].</span></span>


## <a name="permissions"></a><span data-ttu-id="2c97e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="2c97e-106">Permissions</span></span>
<span data-ttu-id="2c97e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2c97e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="2c97e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c97e-109">Permission type</span></span>      | <span data-ttu-id="2c97e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c97e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c97e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c97e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2c97e-112">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="2c97e-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="2c97e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c97e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c97e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c97e-114">Not supported.</span></span>    |
|<span data-ttu-id="2c97e-115">Application</span><span class="sxs-lookup"><span data-stu-id="2c97e-115">Application</span></span> | <span data-ttu-id="2c97e-116">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="2c97e-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c97e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c97e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
DELETE /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns/{column-id}
```
## <a name="request-headers"></a><span data-ttu-id="2c97e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c97e-118">Request headers</span></span>
|<span data-ttu-id="2c97e-119">名称</span><span class="sxs-lookup"><span data-stu-id="2c97e-119">Name</span></span>|<span data-ttu-id="2c97e-120">说明</span><span class="sxs-lookup"><span data-stu-id="2c97e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2c97e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c97e-121">Authorization</span></span>|<span data-ttu-id="2c97e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2c97e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c97e-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c97e-124">Request body</span></span>
<span data-ttu-id="2c97e-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2c97e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c97e-126">响应</span><span class="sxs-lookup"><span data-stu-id="2c97e-126">Response</span></span>

<span data-ttu-id="2c97e-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2c97e-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2c97e-128">示例</span><span class="sxs-lookup"><span data-stu-id="2c97e-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c97e-129">请求</span><span class="sxs-lookup"><span data-stu-id="2c97e-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_columns_from_contenttype"
}
-->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
```

### <a name="response"></a><span data-ttu-id="2c97e-130">响应</span><span class="sxs-lookup"><span data-stu-id="2c97e-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
```http
HTTP/1.1 204 No Content
```

[list]: ../resources/list.md
[columndefinition]: ../resources/columndefinition.md
[contentType]: ../resources/contentType.md
[网站]: ../resources/site.md
[site]: ../resources/site.md
