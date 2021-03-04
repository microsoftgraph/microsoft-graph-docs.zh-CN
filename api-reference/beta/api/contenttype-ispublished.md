---
author: swapnil1993
title: contentType： isPublished
description: 检查内容类型中心网站中内容类型的发布状态。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: d6f5700015dcb69ce3440be187654941816e0a9d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446123"
---
# <a name="contenttype-ispublished"></a><span data-ttu-id="8de0a-103">contentType： isPublished</span><span class="sxs-lookup"><span data-stu-id="8de0a-103">contentType: isPublished</span></span>
<span data-ttu-id="8de0a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8de0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="8de0a-105">检查内容类型中心网站 [中 contentType][] 的发布状态。</span><span class="sxs-lookup"><span data-stu-id="8de0a-105">Check the publishing status of a [contentType][] in a content type hub site.</span></span>

## <a name="permissions"></a><span data-ttu-id="8de0a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="8de0a-106">Permissions</span></span>

<span data-ttu-id="8de0a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8de0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8de0a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8de0a-109">Permission type</span></span>      | <span data-ttu-id="8de0a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8de0a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8de0a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8de0a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8de0a-112">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="8de0a-112">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="8de0a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8de0a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8de0a-114">不支持</span><span class="sxs-lookup"><span data-stu-id="8de0a-114">Not Supported</span></span>   |
|<span data-ttu-id="8de0a-115">Application</span><span class="sxs-lookup"><span data-stu-id="8de0a-115">Application</span></span> | <span data-ttu-id="8de0a-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="8de0a-116">Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8de0a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8de0a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{siteId}/contentTypes/{contentTypeId}/isPublished
```
><span data-ttu-id="8de0a-118">**注意：** siteId 表示内容类型中心网站。</span><span class="sxs-lookup"><span data-stu-id="8de0a-118">**Note:** The siteId represents a content type hub site.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8de0a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8de0a-119">Request headers</span></span>
|<span data-ttu-id="8de0a-120">名称</span><span class="sxs-lookup"><span data-stu-id="8de0a-120">Name</span></span>|<span data-ttu-id="8de0a-121">说明</span><span class="sxs-lookup"><span data-stu-id="8de0a-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8de0a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8de0a-122">Authorization</span></span>|<span data-ttu-id="8de0a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8de0a-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="8de0a-125">响应</span><span class="sxs-lookup"><span data-stu-id="8de0a-125">Response</span></span>
<span data-ttu-id="8de0a-126">如果成功，此调用将返回一个响应和一个指定内容类型的发布状态 `200 OK` 布尔值。</span><span class="sxs-lookup"><span data-stu-id="8de0a-126">If successful, this call returns a `200 OK` response and a boolean value specifying the publishing state of the content type.</span></span>

## <a name="request-body"></a><span data-ttu-id="8de0a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8de0a-127">Request body</span></span>
<span data-ttu-id="8de0a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8de0a-128">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="8de0a-129">示例</span><span class="sxs-lookup"><span data-stu-id="8de0a-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="8de0a-130">请求</span><span class="sxs-lookup"><span data-stu-id="8de0a-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "contenttype_ispublished"
}
-->
```http
GET https://graph.microsoft.com/beta/sites/{siteId}/contentTypes/{contentTypeId}/isPublished
```
### <a name="response"></a><span data-ttu-id="8de0a-131">响应</span><span class="sxs-lookup"><span data-stu-id="8de0a-131">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": true 
}
```

[contentType]: ../resources/contentType.md
