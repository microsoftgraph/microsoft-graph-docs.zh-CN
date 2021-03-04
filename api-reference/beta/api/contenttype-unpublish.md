---
author: swapnil1993
title: contentType：取消发布
description: 从内容类型中心网站取消发布内容类型。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: ca432973337ac81f3ee8e632bb0705f26c7575ea
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446113"
---
# <a name="contenttype-unpublish"></a><span data-ttu-id="c5d2a-103">contentType：取消发布</span><span class="sxs-lookup"><span data-stu-id="c5d2a-103">contentType: unpublish</span></span>
<span data-ttu-id="c5d2a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5d2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="c5d2a-105">从内容类型中心网站取消发布[contentType。][]</span><span class="sxs-lookup"><span data-stu-id="c5d2a-105">Unpublish a [contentType][] from a content type hub site.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5d2a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c5d2a-106">Permissions</span></span>

<span data-ttu-id="c5d2a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c5d2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="c5d2a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5d2a-109">Permission type</span></span>      | <span data-ttu-id="c5d2a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5d2a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5d2a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5d2a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c5d2a-112">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="c5d2a-112">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="c5d2a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5d2a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5d2a-114">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="c5d2a-114">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="c5d2a-115">Application</span><span class="sxs-lookup"><span data-stu-id="c5d2a-115">Application</span></span> | <span data-ttu-id="c5d2a-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="c5d2a-116">Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5d2a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5d2a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/contentTypes/{contentTypeId}/unpublish
```

><span data-ttu-id="c5d2a-118">**注意：** siteId 表示内容类型中心网站。</span><span class="sxs-lookup"><span data-stu-id="c5d2a-118">**Note:** The siteId represents a content type hub site.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5d2a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5d2a-119">Request headers</span></span>
|<span data-ttu-id="c5d2a-120">名称</span><span class="sxs-lookup"><span data-stu-id="c5d2a-120">Name</span></span>|<span data-ttu-id="c5d2a-121">说明</span><span class="sxs-lookup"><span data-stu-id="c5d2a-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c5d2a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5d2a-122">Authorization</span></span>|<span data-ttu-id="c5d2a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c5d2a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5d2a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5d2a-125">Request body</span></span>
<span data-ttu-id="c5d2a-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c5d2a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5d2a-127">响应</span><span class="sxs-lookup"><span data-stu-id="c5d2a-127">Response</span></span>

<span data-ttu-id="c5d2a-128">如果成功，此方法将返回 `204 No Content` 响应。</span><span class="sxs-lookup"><span data-stu-id="c5d2a-128">If successful, this method returns a `204 No Content` response.</span></span>

## <a name="example"></a><span data-ttu-id="c5d2a-129">示例</span><span class="sxs-lookup"><span data-stu-id="c5d2a-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5d2a-130">请求</span><span class="sxs-lookup"><span data-stu-id="c5d2a-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "contenttype_unpublish"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/{siteId}/contentTypes/{contentTypeId}/unpublish
```

### <a name="response"></a><span data-ttu-id="c5d2a-131">响应</span><span class="sxs-lookup"><span data-stu-id="c5d2a-131">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[contentType]: ../resources/contentType.md
