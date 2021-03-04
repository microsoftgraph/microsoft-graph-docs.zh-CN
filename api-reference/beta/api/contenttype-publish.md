---
author: swapnil1993
title: contentType： publish
description: 发布内容类型中心网站中的内容类型。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 072fb067114f9693f18a63c2d1e881fa55a7ca6b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446114"
---
# <a name="contenttype-publish"></a><span data-ttu-id="131d6-103">contentType： publish</span><span class="sxs-lookup"><span data-stu-id="131d6-103">contentType: publish</span></span>
<span data-ttu-id="131d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="131d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="131d6-105">发布内容类型中心网站中的[contentType。][]</span><span class="sxs-lookup"><span data-stu-id="131d6-105">Publishes a [contentType][] present in content type hub site.</span></span>

## <a name="permissions"></a><span data-ttu-id="131d6-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="131d6-106">Permissions</span></span>

<span data-ttu-id="131d6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="131d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="131d6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="131d6-109">Permission type</span></span>      | <span data-ttu-id="131d6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="131d6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="131d6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="131d6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="131d6-112">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="131d6-112">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="131d6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="131d6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="131d6-114">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="131d6-114">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="131d6-115">Application</span><span class="sxs-lookup"><span data-stu-id="131d6-115">Application</span></span> | <span data-ttu-id="131d6-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="131d6-116">Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="131d6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="131d6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /sites/{siteId}/contentTypes/{contentTypeId}/publish
```

><span data-ttu-id="131d6-118">**注意：** siteId 表示内容类型中心网站。</span><span class="sxs-lookup"><span data-stu-id="131d6-118">**Note:** The siteId represents a content type hub site.</span></span>

## <a name="request-headers"></a><span data-ttu-id="131d6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="131d6-119">Request headers</span></span>
|<span data-ttu-id="131d6-120">名称</span><span class="sxs-lookup"><span data-stu-id="131d6-120">Name</span></span>|<span data-ttu-id="131d6-121">说明</span><span class="sxs-lookup"><span data-stu-id="131d6-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="131d6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="131d6-122">Authorization</span></span>|<span data-ttu-id="131d6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="131d6-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="131d6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="131d6-125">Request body</span></span>
<span data-ttu-id="131d6-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="131d6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="131d6-127">响应</span><span class="sxs-lookup"><span data-stu-id="131d6-127">Response</span></span>
<span data-ttu-id="131d6-128">如果成功，此调用将返回 `204 No Content` 响应。</span><span class="sxs-lookup"><span data-stu-id="131d6-128">If successful, this call returns a `204 No Content` response.</span></span>

## <a name="example"></a><span data-ttu-id="131d6-129">示例</span><span class="sxs-lookup"><span data-stu-id="131d6-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="131d6-130">请求</span><span class="sxs-lookup"><span data-stu-id="131d6-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "contenttype_publish"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/{siteId}/contentTypes/{contentTypeId}/publish
```

### <a name="response"></a><span data-ttu-id="131d6-131">响应</span><span class="sxs-lookup"><span data-stu-id="131d6-131">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[contentType]: ../resources/contentType.md
