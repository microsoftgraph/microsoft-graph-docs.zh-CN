---
author: JeremyKelley
ms.author: jeremyke
title: 从捆绑包中删除项目
description: 从 Driveitem 的捆绑包中删除项目
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 508dd19edcd3c1ae231c54cdb195d86661bb4259
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441023"
---
# <a name="remove-item-from-bundle"></a><span data-ttu-id="7cb86-103">从捆绑包中删除项目</span><span class="sxs-lookup"><span data-stu-id="7cb86-103">Remove item from bundle</span></span>

<span data-ttu-id="7cb86-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7cb86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cb86-105">从[捆绑包][]中删除项目。</span><span class="sxs-lookup"><span data-stu-id="7cb86-105">Remove an item from a [bundle][].</span></span>

## <a name="permissions"></a><span data-ttu-id="7cb86-106">权限</span><span class="sxs-lookup"><span data-stu-id="7cb86-106">Permissions</span></span>

<span data-ttu-id="7cb86-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7cb86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cb86-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7cb86-109">Permission type</span></span>      | <span data-ttu-id="7cb86-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7cb86-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cb86-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7cb86-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7cb86-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="7cb86-112">Not supported.</span></span>                             |
|<span data-ttu-id="7cb86-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7cb86-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cb86-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cb86-114">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="7cb86-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7cb86-115">Application</span></span>          | <span data-ttu-id="7cb86-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7cb86-116">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="7cb86-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7cb86-117">HTTP request</span></span>

```http
DELETE /drive/bundles/{bundle-id}/children/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="7cb86-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7cb86-118">Request headers</span></span>

| <span data-ttu-id="7cb86-119">名称</span><span class="sxs-lookup"><span data-stu-id="7cb86-119">Name</span></span>          | <span data-ttu-id="7cb86-120">说明</span><span class="sxs-lookup"><span data-stu-id="7cb86-120">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="7cb86-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cb86-121">Authorization</span></span> | <span data-ttu-id="7cb86-122">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="7cb86-122">Bearer \{token\}.</span></span> <span data-ttu-id="7cb86-123">必填。</span><span class="sxs-lookup"><span data-stu-id="7cb86-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7cb86-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="7cb86-124">Request body</span></span>

<span data-ttu-id="7cb86-125">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="7cb86-125">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="7cb86-126">响应</span><span class="sxs-lookup"><span data-stu-id="7cb86-126">Response</span></span>

<span data-ttu-id="7cb86-127">如果成功，响应为`204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="7cb86-127">If successful, the response is `204 No Content`.</span></span>

<span data-ttu-id="7cb86-128">阅读 "[错误响应][error-response]" 主题，了解有关如何返回错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7cb86-128">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="7cb86-129">示例</span><span class="sxs-lookup"><span data-stu-id="7cb86-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7cb86-130">请求</span><span class="sxs-lookup"><span data-stu-id="7cb86-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7cb86-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="7cb86-131">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "remove-from-bundle" } -->

```http
DELETE https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children/{item-id}
```
# <a name="c"></a>[<span data-ttu-id="7cb86-132">C#</span><span class="sxs-lookup"><span data-stu-id="7cb86-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-from-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7cb86-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7cb86-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-from-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7cb86-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7cb86-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-from-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7cb86-135">响应</span><span class="sxs-lookup"><span data-stu-id="7cb86-135">Response</span></span>

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
