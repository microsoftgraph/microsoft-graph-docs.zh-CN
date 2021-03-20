---
author: swapnil1993
title: 获取 columnDefinition
description: " 获取网站、列表或内容类型列。"
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 3a2e1421c92b1634ea57cbedb74c2e3244d85924
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952231"
---
# <a name="get-columndefinition"></a><span data-ttu-id="c3b1c-103">获取 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="c3b1c-103">Get columnDefinition</span></span>
<span data-ttu-id="c3b1c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3b1c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="c3b1c-105">检索网站、[列表或][] [contentType][] [列的][][元数据][columnDefinition]。</span><span class="sxs-lookup"><span data-stu-id="c3b1c-105">Retrieve the metadata for a [site][], [list][] or [contentType][] [column][columnDefinition].</span></span>

  

## <a name="permissions"></a><span data-ttu-id="c3b1c-106">权限</span><span class="sxs-lookup"><span data-stu-id="c3b1c-106">Permissions</span></span>

  

<span data-ttu-id="c3b1c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c3b1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="c3b1c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3b1c-109">Permission type</span></span> | <span data-ttu-id="c3b1c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c3b1c-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3b1c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3b1c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c3b1c-112">Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="c3b1c-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="c3b1c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c3b1c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3b1c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3b1c-114">Not supported.</span></span> |
|<span data-ttu-id="c3b1c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c3b1c-115">Application</span></span> | <span data-ttu-id="c3b1c-116">Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="c3b1c-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |

  

## <a name="http-request"></a><span data-ttu-id="c3b1c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3b1c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /sites/{site-id}/columns/{column-id}
GET /sites/{site-id}/lists/{list-id}/columns/{column-id}
GET /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
GET /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns/{column-id}
```

## <a name="request-headers"></a><span data-ttu-id="c3b1c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3b1c-118">Request headers</span></span>
|<span data-ttu-id="c3b1c-119">名称</span><span class="sxs-lookup"><span data-stu-id="c3b1c-119">Name</span></span>|<span data-ttu-id="c3b1c-120">说明</span><span class="sxs-lookup"><span data-stu-id="c3b1c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c3b1c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3b1c-121">Authorization</span></span>|<span data-ttu-id="c3b1c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c3b1c-p102">Bearer {token}. Required.</span></span>|  

## <a name="request-body"></a><span data-ttu-id="c3b1c-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="c3b1c-124">Request body</span></span>

  

<span data-ttu-id="c3b1c-125">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="c3b1c-125">Do not supply a request body with this method.</span></span>

  

## <a name="example"></a><span data-ttu-id="c3b1c-126">示例</span><span class="sxs-lookup"><span data-stu-id="c3b1c-126">Example</span></span>

  

### <a name="request"></a><span data-ttu-id="c3b1c-127">请求</span><span class="sxs-lookup"><span data-stu-id="c3b1c-127">Request</span></span>

  


# <a name="http"></a>[<span data-ttu-id="c3b1c-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3b1c-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get_column_from_contenttype" } -->

  

```msgraph-interactive
GET /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
```
# <a name="c"></a>[<span data-ttu-id="c3b1c-129">C#</span><span class="sxs-lookup"><span data-stu-id="c3b1c-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-column-from-contenttype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3b1c-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3b1c-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-column-from-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3b1c-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3b1c-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-column-from-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3b1c-132">Java</span><span class="sxs-lookup"><span data-stu-id="c3b1c-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-column-from-contenttype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


  

#### <a name="response"></a><span data-ttu-id="c3b1c-133">响应</span><span class="sxs-lookup"><span data-stu-id="c3b1c-133">Response</span></span>

  

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true } -->

  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "",
  "displayName": "Title",
  "hidden": false,
  "id": "99ddcf45-e2f7-4f17-82b0-6fba34445103",
  "indexed": false,
  "name": "Title",
  "readOnly": false,
  "required": false,
  "text": {
    "allowMultipleLines": false,
    "appendChangesToExistingText": false,
    "linesForEditing": 0,
    "maxLength": 255
  }
}
```

  

[columnDefinition]: ../resources/columnDefinition.md

[list]: ../resources/list.md

[site]: ../resources/site.md

[contentType]: ../resources/contentType.md
  
