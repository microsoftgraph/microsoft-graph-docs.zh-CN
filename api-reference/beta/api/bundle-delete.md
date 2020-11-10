---
author: JeremyKelley
ms.author: jeremyke
title: 删除捆绑包
description: 删除 Driveitem 的捆绑包
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: d5aa0c77a755183582de8f7a798897cd192afbab
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960269"
---
# <a name="delete-bundle"></a><span data-ttu-id="5ba63-103">删除捆绑包</span><span class="sxs-lookup"><span data-stu-id="5ba63-103">Delete bundle</span></span>

<span data-ttu-id="5ba63-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ba63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ba63-105">使用 **id** 删除 driveitem 的 [捆绑包][]。请注意，使用此方法删除捆绑包将永久删除该捆绑包，而不会将其移动到回收站中。</span><span class="sxs-lookup"><span data-stu-id="5ba63-105">Delete a [bundle][] of driveItems by using its **id**. Note that deleting a bundle using this method permanently deletes the bundle and does not move it to the Recycle Bin.</span></span>
<span data-ttu-id="5ba63-106">但是，它不会删除捆绑包引用的项目。</span><span class="sxs-lookup"><span data-stu-id="5ba63-106">It does not, however, remove the items that were referenced by the bundle.</span></span>
<span data-ttu-id="5ba63-107">它们将保留在其父文件夹中。</span><span class="sxs-lookup"><span data-stu-id="5ba63-107">They will remain in their parent folders.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ba63-108">权限</span><span class="sxs-lookup"><span data-stu-id="5ba63-108">Permissions</span></span>

<span data-ttu-id="5ba63-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5ba63-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ba63-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ba63-111">Permission type</span></span>      | <span data-ttu-id="5ba63-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5ba63-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ba63-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ba63-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5ba63-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ba63-114">Not supported.</span></span>                             |
|<span data-ttu-id="5ba63-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ba63-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ba63-116">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ba63-116">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="5ba63-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ba63-117">Application</span></span>          | <span data-ttu-id="5ba63-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ba63-118">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="5ba63-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ba63-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drive/items/{bundle-id}
```

## <a name="request-headers"></a><span data-ttu-id="5ba63-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ba63-120">Request headers</span></span>

| <span data-ttu-id="5ba63-121">名称</span><span class="sxs-lookup"><span data-stu-id="5ba63-121">Name</span></span>          | <span data-ttu-id="5ba63-122">说明</span><span class="sxs-lookup"><span data-stu-id="5ba63-122">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="5ba63-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ba63-123">Authorization</span></span> | <span data-ttu-id="5ba63-124">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="5ba63-124">Bearer \{token\}.</span></span> <span data-ttu-id="5ba63-125">必需。</span><span class="sxs-lookup"><span data-stu-id="5ba63-125">Required.</span></span> |
| <span data-ttu-id="5ba63-126">if-match</span><span class="sxs-lookup"><span data-stu-id="5ba63-126">if-match</span></span>      | <span data-ttu-id="5ba63-127">eTag.</span><span class="sxs-lookup"><span data-stu-id="5ba63-127">eTag.</span></span> <span data-ttu-id="5ba63-128">可选。</span><span class="sxs-lookup"><span data-stu-id="5ba63-128">Optional.</span></span> <span data-ttu-id="5ba63-129">如果包含此请求标头且提供的 eTag (或 cTag) 与捆绑包中的当前标记不匹配， `412 Precondition Failed` 则会返回响应，并且不会删除该捆绑包。</span><span class="sxs-lookup"><span data-stu-id="5ba63-129">If this request header is included and the eTag (or cTag) provided does not match the current tag on the bundle, a `412 Precondition Failed` response is returned and the bundle will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="5ba63-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ba63-130">Request body</span></span>

<span data-ttu-id="5ba63-131">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="5ba63-131">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ba63-132">响应</span><span class="sxs-lookup"><span data-stu-id="5ba63-132">Response</span></span>

<span data-ttu-id="5ba63-133">如果成功，此调用将返回 `204 No Content` 响应，表示资源已被删除，没有可返回的内容。</span><span class="sxs-lookup"><span data-stu-id="5ba63-133">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<span data-ttu-id="5ba63-134">阅读 " [错误响应][error-response] " 主题，了解有关如何返回错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5ba63-134">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="5ba63-135">示例</span><span class="sxs-lookup"><span data-stu-id="5ba63-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ba63-136">请求</span><span class="sxs-lookup"><span data-stu-id="5ba63-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5ba63-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ba63-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-bundle" } -->

```http
DELETE https://graph.microsoft.com/beta/drive/items/{bundle-id}
```
# <a name="c"></a>[<span data-ttu-id="5ba63-138">C#</span><span class="sxs-lookup"><span data-stu-id="5ba63-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ba63-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ba63-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ba63-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ba63-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ba63-141">Java</span><span class="sxs-lookup"><span data-stu-id="5ba63-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5ba63-142">响应</span><span class="sxs-lookup"><span data-stu-id="5ba63-142">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


[bundle]: ../resources/bundle.md
[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a bundle from OneDrive",
  "keywords": "delete,existing bundle,onedrive",
  "section": "documentation",
  "tocPath": "Bundles/Delete"
} -->


