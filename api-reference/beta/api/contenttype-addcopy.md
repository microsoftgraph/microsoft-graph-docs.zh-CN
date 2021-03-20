---
author: swapnil1993
title: contentType： addCopy
description: 将网站内容类型的副本添加到列表中。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: f388799e409a5f2037182bb3bc331a6a6adbc45f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947027"
---
# <a name="contenttype-addcopy"></a><span data-ttu-id="b59bc-103">contentType： addCopy</span><span class="sxs-lookup"><span data-stu-id="b59bc-103">contentType: addCopy</span></span>
<span data-ttu-id="b59bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b59bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="b59bc-105">将内容类型[contentType] [的副本从][网站添加到][site][列表][list]。</span><span class="sxs-lookup"><span data-stu-id="b59bc-105">Add a copy of a [content type][contentType] from a [site][site] to a [list][list].</span></span>
 
  

## <a name="permissions"></a><span data-ttu-id="b59bc-106">权限</span><span class="sxs-lookup"><span data-stu-id="b59bc-106">Permissions</span></span>  

<span data-ttu-id="b59bc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b59bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="b59bc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b59bc-109">Permission type</span></span> | <span data-ttu-id="b59bc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b59bc-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b59bc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b59bc-111">Delegated (work or school account)</span></span> |<span data-ttu-id="b59bc-112">Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="b59bc-112">Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="b59bc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b59bc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b59bc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b59bc-114">Not supported.</span></span> |
|<span data-ttu-id="b59bc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b59bc-115">Application</span></span> | <span data-ttu-id="b59bc-116">Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="b59bc-116">Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="b59bc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b59bc-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
POST /sites/{site-id}/lists/{list-id}/contentTypes/addCopy
```

## <a name="request-headers"></a><span data-ttu-id="b59bc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b59bc-118">Request headers</span></span>
|<span data-ttu-id="b59bc-119">名称</span><span class="sxs-lookup"><span data-stu-id="b59bc-119">Name</span></span>|<span data-ttu-id="b59bc-120">说明</span><span class="sxs-lookup"><span data-stu-id="b59bc-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b59bc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b59bc-121">Authorization</span></span>|<span data-ttu-id="b59bc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b59bc-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b59bc-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b59bc-124">Content-Type</span></span>|<span data-ttu-id="b59bc-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b59bc-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b59bc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b59bc-127">Request body</span></span>
<span data-ttu-id="b59bc-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b59bc-128">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="b59bc-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="b59bc-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b59bc-130">参数</span><span class="sxs-lookup"><span data-stu-id="b59bc-130">Parameter</span></span>|<span data-ttu-id="b59bc-131">类型</span><span class="sxs-lookup"><span data-stu-id="b59bc-131">Type</span></span>|<span data-ttu-id="b59bc-132">说明</span><span class="sxs-lookup"><span data-stu-id="b59bc-132">Description</span></span>|
|-|-|-|
|<span data-ttu-id="b59bc-133">contentType</span><span class="sxs-lookup"><span data-stu-id="b59bc-133">contentType</span></span>| <span data-ttu-id="b59bc-134">string</span><span class="sxs-lookup"><span data-stu-id="b59bc-134">string</span></span> | <span data-ttu-id="b59bc-135">将复制到列表的网站内容类型的规范 URL。</span><span class="sxs-lookup"><span data-stu-id="b59bc-135">Canonical URL to the site content type that will be copied to the list.</span></span> <span data-ttu-id="b59bc-136">必需。</span><span class="sxs-lookup"><span data-stu-id="b59bc-136">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="b59bc-137">响应</span><span class="sxs-lookup"><span data-stu-id="b59bc-137">Response</span></span>

<span data-ttu-id="b59bc-138">如果成功，此调用在响应 `201 Created` 正文中返回 响应代码和 [contentType][] 对象。</span><span class="sxs-lookup"><span data-stu-id="b59bc-138">If successful, this call returns a `201 Created` response code and a [contentType][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b59bc-139">示例</span><span class="sxs-lookup"><span data-stu-id="b59bc-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="b59bc-140">请求</span><span class="sxs-lookup"><span data-stu-id="b59bc-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b59bc-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="b59bc-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_addcopy"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/id/lists/{list-id}/contentTypes/addCopy
Content-Type: application/json

{
  "contentType": "https://graph.microsoft.com/beta/sites/id/contentTypes/0x0101"
}
```
# <a name="c"></a>[<span data-ttu-id="b59bc-142">C#</span><span class="sxs-lookup"><span data-stu-id="b59bc-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-addcopy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b59bc-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b59bc-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-addcopy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b59bc-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b59bc-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-addcopy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b59bc-145">Java</span><span class="sxs-lookup"><span data-stu-id="b59bc-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-addcopy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a><span data-ttu-id="b59bc-146">响应</span><span class="sxs-lookup"><span data-stu-id="b59bc-146">Response</span></span>


<!-- { "blockType": "response", "@type": "microsoft.graph.contentType", "truncated": true} -->

```http
HTTP/1.1 201 Created

{
    "id": "0x0101",
    "description": "Create a new custom CSR JavaScript Display Template.",
    "group": "Display Template Content Types",
    "hidden": false,
    "name": "JavaScript Display Template",
    "parentId": "0x01",
    "readOnly": false,
    "sealed": false,
    "base": {
        "id": "0x01",
        "description": "Create a new custom CSR JavaScript Display Template.",
        "group": "Display Template Content Types",
        "hidden": false,
        "name": "JavaScript Display Template",
        "readOnly": false,
        "sealed": false
    }
}
```

[site]: ../resources/site.md
[list]: ../resources/list.md
[contentType]: ../resources/contentType.md
