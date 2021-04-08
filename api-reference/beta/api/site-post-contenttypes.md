---
author: swapnil1993
title: 创建 contentType
description: 为网站创建内容类型。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 4eff9efd9ae4f2b2daa81356cc8d3887f7fc3c29
ms.sourcegitcommit: aa18eb8a9965f99cc97680808abba8df46f31ba5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "51638863"
---
# <a name="create-contenttype"></a><span data-ttu-id="b0886-103">创建 contentType</span><span class="sxs-lookup"><span data-stu-id="b0886-103">Create contentType</span></span>
<span data-ttu-id="b0886-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0886-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0886-105">为网站[创建新的 contentType。][] [][]</span><span class="sxs-lookup"><span data-stu-id="b0886-105">Create a new [contentType][] for a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="b0886-106">权限</span><span class="sxs-lookup"><span data-stu-id="b0886-106">Permissions</span></span>

<span data-ttu-id="b0886-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0886-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0886-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0886-109">Permission type</span></span>      | <span data-ttu-id="b0886-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b0886-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0886-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0886-111">Delegated (work or school account)</span></span> |<span data-ttu-id="b0886-112">Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="b0886-112">Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="b0886-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0886-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="b0886-114">不支持</span><span class="sxs-lookup"><span data-stu-id="b0886-114">Not Supported</span></span>    |
|<span data-ttu-id="b0886-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0886-115">Application</span></span> |<span data-ttu-id="b0886-116">Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="b0886-116">Sites.Manage.All, Sites.FullControl.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="b0886-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0886-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/contentTypes
```

## <a name="request-headers"></a><span data-ttu-id="b0886-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0886-118">Request headers</span></span>
|<span data-ttu-id="b0886-119">名称</span><span class="sxs-lookup"><span data-stu-id="b0886-119">Name</span></span>|<span data-ttu-id="b0886-120">说明</span><span class="sxs-lookup"><span data-stu-id="b0886-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b0886-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0886-121">Authorization</span></span>|<span data-ttu-id="b0886-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b0886-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b0886-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b0886-124">Content-Type</span></span>|<span data-ttu-id="b0886-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b0886-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0886-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0886-127">Request body</span></span>

<span data-ttu-id="b0886-128">在请求正文中，提供要创建的 [contentType][] 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0886-128">In the request body, supply a JSON representation of the [contentType][] resource to create.</span></span>

## <a name="response"></a><span data-ttu-id="b0886-129">响应</span><span class="sxs-lookup"><span data-stu-id="b0886-129">Response</span></span>

<span data-ttu-id="b0886-130">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [contentType][] 对象。</span><span class="sxs-lookup"><span data-stu-id="b0886-130">If successful, this method returns a `201 Created` response code and a [contentType][] object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="b0886-131">示例</span><span class="sxs-lookup"><span data-stu-id="b0886-131">Example</span></span>

<span data-ttu-id="b0886-132">以下示例演示如何创建新的泛型内容类型。</span><span class="sxs-lookup"><span data-stu-id="b0886-132">The following example shows how to create a new generic content type.</span></span>

### <a name="request"></a><span data-ttu-id="b0886-133">请求</span><span class="sxs-lookup"><span data-stu-id="b0886-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b0886-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0886-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contenttype"
}
-->

```http
POST https://graph.microsoft.com/beta/sites/{id}/contentTypes
Content-Type: application/json

{
    "name": "docSet",
    "description": "custom docset",
    "base": {
        "name": "Document Set",
        "id": "0x0120D520"
    },
    "group": "Document Set Content Types" 
}
```
# <a name="javascript"></a>[<span data-ttu-id="b0886-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0886-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="b0886-136">C#</span><span class="sxs-lookup"><span data-stu-id="b0886-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contenttype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0886-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0886-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b0886-138">Java</span><span class="sxs-lookup"><span data-stu-id="b0886-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contenttype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b0886-139">响应</span><span class="sxs-lookup"><span data-stu-id="b0886-139">Response</span></span>
><span data-ttu-id="b0886-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b0886-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType"
}
-->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "0x01002A2479FF33DD4BC3B1533A012B653717",
  "name": "docSet",
  "group":"Document Set Content Types",
  "description" : "custom docset",
  "base": {
        "name": "Document Set",
        "id": "0x0120D520"
   }
}
```


[contentType]: ../resources/contentType.md
[site]: ../resources/site.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a Content type in a site",
  "keywords": "content type",
  "section": "documentation",
  "tocPath": "sites/Create ContentType",
  "suppressions": [
  ]
}
-->
