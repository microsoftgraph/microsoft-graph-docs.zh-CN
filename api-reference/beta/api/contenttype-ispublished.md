---
author: swapnil1993
title: contentType： isPublished
description: 检查内容类型中心网站中内容类型的发布状态。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: e61d488dddc9797c3f0623a3e534f54b1bab4708
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439407"
---
# <a name="contenttype-ispublished"></a><span data-ttu-id="87a95-103">contentType： isPublished</span><span class="sxs-lookup"><span data-stu-id="87a95-103">contentType: isPublished</span></span>
<span data-ttu-id="87a95-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87a95-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="87a95-105">检查内容类型中心 [网站中 contentType][] 的发布状态。</span><span class="sxs-lookup"><span data-stu-id="87a95-105">Check the publishing status of a [contentType][] in a content type hub site.</span></span>

## <a name="permissions"></a><span data-ttu-id="87a95-106">权限</span><span class="sxs-lookup"><span data-stu-id="87a95-106">Permissions</span></span>

<span data-ttu-id="87a95-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="87a95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87a95-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="87a95-109">Permission type</span></span>      | <span data-ttu-id="87a95-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="87a95-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87a95-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="87a95-111">Delegated (work or school account)</span></span> | <span data-ttu-id="87a95-112">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="87a95-112">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="87a95-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="87a95-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87a95-114">不支持</span><span class="sxs-lookup"><span data-stu-id="87a95-114">Not Supported</span></span>   |
|<span data-ttu-id="87a95-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="87a95-115">Application</span></span> | <span data-ttu-id="87a95-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="87a95-116">Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87a95-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="87a95-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{siteId}/contentTypes/{contentTypeId}/isPublished
```
><span data-ttu-id="87a95-118">**注意**_：siteId_ 表示内容类型中心网站。</span><span class="sxs-lookup"><span data-stu-id="87a95-118">**Note:** _siteId_ represents a content type hub site.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87a95-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="87a95-119">Request headers</span></span>
|<span data-ttu-id="87a95-120">名称</span><span class="sxs-lookup"><span data-stu-id="87a95-120">Name</span></span>|<span data-ttu-id="87a95-121">说明</span><span class="sxs-lookup"><span data-stu-id="87a95-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="87a95-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="87a95-122">Authorization</span></span>|<span data-ttu-id="87a95-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="87a95-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="87a95-125">响应</span><span class="sxs-lookup"><span data-stu-id="87a95-125">Response</span></span>
<span data-ttu-id="87a95-126">如果成功，此调用将返回 响应和一个布尔值，该值指定 `200 OK` 内容类型的发布状态。</span><span class="sxs-lookup"><span data-stu-id="87a95-126">If successful, this call returns a `200 OK` response and a boolean value that specifies the publishing state of the content type.</span></span>

## <a name="request-body"></a><span data-ttu-id="87a95-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="87a95-127">Request body</span></span>
<span data-ttu-id="87a95-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="87a95-128">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="87a95-129">示例</span><span class="sxs-lookup"><span data-stu-id="87a95-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="87a95-130">请求</span><span class="sxs-lookup"><span data-stu-id="87a95-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="87a95-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="87a95-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_ispublished"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{siteId}/contentTypes/{contentTypeId}/isPublished
```
# <a name="c"></a>[<span data-ttu-id="87a95-132">C#</span><span class="sxs-lookup"><span data-stu-id="87a95-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-ispublished-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87a95-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87a95-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-ispublished-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87a95-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87a95-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-ispublished-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="87a95-135">Java</span><span class="sxs-lookup"><span data-stu-id="87a95-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-ispublished-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="87a95-136">响应</span><span class="sxs-lookup"><span data-stu-id="87a95-136">Response</span></span>
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
