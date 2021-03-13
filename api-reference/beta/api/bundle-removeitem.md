---
author: JeremyKelley
title: 从捆绑包中删除项目
description: 从 driveItems 捆绑包中删除项
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: edd7647be648b5eda1560157d35c6a7b2d4aa130
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50774360"
---
# <a name="remove-item-from-bundle"></a><span data-ttu-id="88438-103">从捆绑包中删除项目</span><span class="sxs-lookup"><span data-stu-id="88438-103">Remove item from bundle</span></span>

<span data-ttu-id="88438-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88438-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88438-105">从捆绑包中删除 [项][]。</span><span class="sxs-lookup"><span data-stu-id="88438-105">Remove an item from a [bundle][].</span></span>

## <a name="permissions"></a><span data-ttu-id="88438-106">权限</span><span class="sxs-lookup"><span data-stu-id="88438-106">Permissions</span></span>

<span data-ttu-id="88438-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88438-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88438-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="88438-109">Permission type</span></span>      | <span data-ttu-id="88438-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88438-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88438-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88438-111">Delegated (work or school account)</span></span> | <span data-ttu-id="88438-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="88438-112">Not supported.</span></span>                             |
|<span data-ttu-id="88438-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88438-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88438-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88438-114">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="88438-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="88438-115">Application</span></span>          | <span data-ttu-id="88438-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="88438-116">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="88438-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88438-117">HTTP request</span></span>

```http
DELETE /drive/bundles/{bundle-id}/children/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="88438-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="88438-118">Request headers</span></span>

| <span data-ttu-id="88438-119">名称</span><span class="sxs-lookup"><span data-stu-id="88438-119">Name</span></span>          | <span data-ttu-id="88438-120">说明</span><span class="sxs-lookup"><span data-stu-id="88438-120">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="88438-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="88438-121">Authorization</span></span> | <span data-ttu-id="88438-122">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="88438-122">Bearer \{token\}.</span></span> <span data-ttu-id="88438-123">必填。</span><span class="sxs-lookup"><span data-stu-id="88438-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88438-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="88438-124">Request body</span></span>

<span data-ttu-id="88438-125">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="88438-125">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="88438-126">响应</span><span class="sxs-lookup"><span data-stu-id="88438-126">Response</span></span>

<span data-ttu-id="88438-127">如果成功，响应为 `204 No Content` 。</span><span class="sxs-lookup"><span data-stu-id="88438-127">If successful, the response is `204 No Content`.</span></span>

<span data-ttu-id="88438-128">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="88438-128">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="88438-129">示例</span><span class="sxs-lookup"><span data-stu-id="88438-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="88438-130">请求</span><span class="sxs-lookup"><span data-stu-id="88438-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="88438-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="88438-131">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "remove-from-bundle" } -->

```http
DELETE https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children/{item-id}
```
# <a name="c"></a>[<span data-ttu-id="88438-132">C#</span><span class="sxs-lookup"><span data-stu-id="88438-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-from-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88438-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88438-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-from-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88438-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88438-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-from-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88438-135">Java</span><span class="sxs-lookup"><span data-stu-id="88438-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-from-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="88438-136">响应</span><span class="sxs-lookup"><span data-stu-id="88438-136">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


[bundle]: ../resources/bundle.md
[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Remove an item from a bundle.",
  "keywords": "",
  "section": "documentation"
} -->


