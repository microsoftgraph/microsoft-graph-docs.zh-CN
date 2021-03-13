---
author: swapnil1993
title: contentType： isPublished
description: 检查内容类型中心网站中内容类型的发布状态。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 150caec3be0740d82563e280e6425d0d3b827ecd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770570"
---
# <a name="contenttype-ispublished"></a><span data-ttu-id="efe65-103">contentType： isPublished</span><span class="sxs-lookup"><span data-stu-id="efe65-103">contentType: isPublished</span></span>
<span data-ttu-id="efe65-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efe65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="efe65-105">检查内容类型中心 [网站中 contentType][] 的发布状态。</span><span class="sxs-lookup"><span data-stu-id="efe65-105">Check the publishing status of a [contentType][] in a content type hub site.</span></span>

## <a name="permissions"></a><span data-ttu-id="efe65-106">权限</span><span class="sxs-lookup"><span data-stu-id="efe65-106">Permissions</span></span>

<span data-ttu-id="efe65-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="efe65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efe65-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="efe65-109">Permission type</span></span>      | <span data-ttu-id="efe65-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="efe65-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efe65-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="efe65-111">Delegated (work or school account)</span></span> | <span data-ttu-id="efe65-112">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="efe65-112">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="efe65-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="efe65-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efe65-114">不支持</span><span class="sxs-lookup"><span data-stu-id="efe65-114">Not Supported</span></span>   |
|<span data-ttu-id="efe65-115">Application</span><span class="sxs-lookup"><span data-stu-id="efe65-115">Application</span></span> | <span data-ttu-id="efe65-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="efe65-116">Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="efe65-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="efe65-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{siteId}/contentTypes/{contentTypeId}/isPublished
```
><span data-ttu-id="efe65-118">**注意：** siteId 表示内容类型中心网站。</span><span class="sxs-lookup"><span data-stu-id="efe65-118">**Note:** The siteId represents a content type hub site.</span></span>

## <a name="request-headers"></a><span data-ttu-id="efe65-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="efe65-119">Request headers</span></span>
|<span data-ttu-id="efe65-120">名称</span><span class="sxs-lookup"><span data-stu-id="efe65-120">Name</span></span>|<span data-ttu-id="efe65-121">说明</span><span class="sxs-lookup"><span data-stu-id="efe65-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="efe65-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="efe65-122">Authorization</span></span>|<span data-ttu-id="efe65-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="efe65-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="efe65-125">响应</span><span class="sxs-lookup"><span data-stu-id="efe65-125">Response</span></span>
<span data-ttu-id="efe65-126">如果成功，此调用将返回 响应和指定内容类型的发布状态 `200 OK` 的布尔值。</span><span class="sxs-lookup"><span data-stu-id="efe65-126">If successful, this call returns a `200 OK` response and a boolean value specifying the publishing state of the content type.</span></span>

## <a name="request-body"></a><span data-ttu-id="efe65-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="efe65-127">Request body</span></span>
<span data-ttu-id="efe65-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="efe65-128">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="efe65-129">示例</span><span class="sxs-lookup"><span data-stu-id="efe65-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="efe65-130">请求</span><span class="sxs-lookup"><span data-stu-id="efe65-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="efe65-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="efe65-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_ispublished"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{siteId}/contentTypes/{contentTypeId}/isPublished
```
# <a name="c"></a>[<span data-ttu-id="efe65-132">C#</span><span class="sxs-lookup"><span data-stu-id="efe65-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-ispublished-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="efe65-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="efe65-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-ispublished-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="efe65-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="efe65-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-ispublished-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="efe65-135">Java</span><span class="sxs-lookup"><span data-stu-id="efe65-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-ispublished-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="efe65-136">响应</span><span class="sxs-lookup"><span data-stu-id="efe65-136">Response</span></span>
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
