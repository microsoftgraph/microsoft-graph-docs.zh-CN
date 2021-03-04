---
author: swapnil1993
title: 删除 contentType
description: 从 sharepoint 列表或网站中删除内容类型。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8c27cfd2e16fc4c3bd7fade3f5546c08951f38c5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446129"
---
# <a name="delete-contenttype"></a><span data-ttu-id="ebac1-103">删除 contentType</span><span class="sxs-lookup"><span data-stu-id="ebac1-103">Delete contentType</span></span>
<span data-ttu-id="ebac1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebac1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebac1-105">从 [列表或][contentType] 网站 [中删除][] 内容 [类型][]。</span><span class="sxs-lookup"><span data-stu-id="ebac1-105">Remove a [content type][contentType] from a [list][] or a [site][].</span></span>


## <a name="permissions"></a><span data-ttu-id="ebac1-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ebac1-106">Permissions</span></span>
<span data-ttu-id="ebac1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ebac1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="ebac1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ebac1-109">Permission type</span></span>      | <span data-ttu-id="ebac1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ebac1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebac1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ebac1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ebac1-112">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="ebac1-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="ebac1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ebac1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebac1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ebac1-114">Not supported.</span></span>    |
|<span data-ttu-id="ebac1-115">Application</span><span class="sxs-lookup"><span data-stu-id="ebac1-115">Application</span></span> | <span data-ttu-id="ebac1-116">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="ebac1-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebac1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ebac1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/contentTypes/{contentType-id}
DELETE /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}
```

## <a name="request-headers"></a><span data-ttu-id="ebac1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ebac1-118">Request headers</span></span>
|<span data-ttu-id="ebac1-119">名称</span><span class="sxs-lookup"><span data-stu-id="ebac1-119">Name</span></span>|<span data-ttu-id="ebac1-120">说明</span><span class="sxs-lookup"><span data-stu-id="ebac1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ebac1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebac1-121">Authorization</span></span>|<span data-ttu-id="ebac1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ebac1-p102">Bearer {token}. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="ebac1-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ebac1-124">Request body</span></span>

<span data-ttu-id="ebac1-125">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="ebac1-125">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebac1-126">响应</span><span class="sxs-lookup"><span data-stu-id="ebac1-126">Response</span></span>

<span data-ttu-id="ebac1-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ebac1-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ebac1-128">示例</span><span class="sxs-lookup"><span data-stu-id="ebac1-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebac1-129">请求</span><span class="sxs-lookup"><span data-stu-id="ebac1-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contenttype"
}
-->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}
```

### <a name="response"></a><span data-ttu-id="ebac1-130">响应</span><span class="sxs-lookup"><span data-stu-id="ebac1-130">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```

[list]: ../resources/list.md
[contentType]: ../resources/contentType.md
[网站]: ../resources/site.md
[site]: ../resources/site.md
