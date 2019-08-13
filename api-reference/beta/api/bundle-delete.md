---
author: JeremyKelley
ms.author: jeremyke
title: 删除捆绑包
description: 删除 Driveitem 的捆绑包
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b00153cecae8c3f84c1f74d83a977aed8b047cb0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318010"
---
# <a name="delete-bundle"></a><span data-ttu-id="f4267-103">删除捆绑包</span><span class="sxs-lookup"><span data-stu-id="f4267-103">Delete bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4267-104">使用**id**删除 driveitem 的[捆绑包][]。请注意, 使用此方法删除捆绑包将永久删除该捆绑包, 而不会将其移动到回收站中。</span><span class="sxs-lookup"><span data-stu-id="f4267-104">Delete a [bundle][] of driveItems by using its **id**. Note that deleting a bundle using this method permanently deletes the bundle and does not move it to the Recycle Bin.</span></span>
<span data-ttu-id="f4267-105">但是, 它不会删除捆绑包引用的项目。</span><span class="sxs-lookup"><span data-stu-id="f4267-105">It does not, however, remove the items that were referenced by the bundle.</span></span>
<span data-ttu-id="f4267-106">它们将保留在其父文件夹中。</span><span class="sxs-lookup"><span data-stu-id="f4267-106">They will remain in their parent folders.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4267-107">权限</span><span class="sxs-lookup"><span data-stu-id="f4267-107">Permissions</span></span>

<span data-ttu-id="f4267-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4267-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4267-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4267-110">Permission type</span></span>      | <span data-ttu-id="f4267-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f4267-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4267-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4267-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f4267-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4267-113">Not supported.</span></span>                             |
|<span data-ttu-id="f4267-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4267-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4267-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4267-115">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="f4267-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4267-116">Application</span></span>          | <span data-ttu-id="f4267-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4267-117">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="f4267-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4267-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drive/items/{bundle-id}
```

## <a name="request-headers"></a><span data-ttu-id="f4267-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4267-119">Request headers</span></span>

| <span data-ttu-id="f4267-120">名称</span><span class="sxs-lookup"><span data-stu-id="f4267-120">Name</span></span>          | <span data-ttu-id="f4267-121">说明</span><span class="sxs-lookup"><span data-stu-id="f4267-121">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="f4267-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4267-122">Authorization</span></span> | <span data-ttu-id="f4267-123">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="f4267-123">Bearer \{token\}.</span></span> <span data-ttu-id="f4267-124">必需。</span><span class="sxs-lookup"><span data-stu-id="f4267-124">Required.</span></span> |
| <span data-ttu-id="f4267-125">if-match</span><span class="sxs-lookup"><span data-stu-id="f4267-125">if-match</span></span>      | <span data-ttu-id="f4267-126">eTag.</span><span class="sxs-lookup"><span data-stu-id="f4267-126">eTag.</span></span> <span data-ttu-id="f4267-127">可选。</span><span class="sxs-lookup"><span data-stu-id="f4267-127">Optional.</span></span> <span data-ttu-id="f4267-128">如果包含此请求标头, 且提供的 eTag (或 cTag) 与捆绑包中的当前标记不匹配, `412 Precondition Failed`则会返回响应, 并且不会删除该捆绑包。</span><span class="sxs-lookup"><span data-stu-id="f4267-128">If this request header is included and the eTag (or cTag) provided does not match the current tag on the bundle, a `412 Precondition Failed` response is returned and the bundle will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="f4267-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4267-129">Request body</span></span>

<span data-ttu-id="f4267-130">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="f4267-130">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4267-131">响应</span><span class="sxs-lookup"><span data-stu-id="f4267-131">Response</span></span>

<span data-ttu-id="f4267-132">如果成功，此调用将返回 `204 No Content` 响应，表示资源已被删除，没有可返回的内容。</span><span class="sxs-lookup"><span data-stu-id="f4267-132">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<span data-ttu-id="f4267-133">阅读 "[错误响应][error-response]" 主题, 了解有关如何返回错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f4267-133">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="f4267-134">示例</span><span class="sxs-lookup"><span data-stu-id="f4267-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4267-135">请求</span><span class="sxs-lookup"><span data-stu-id="f4267-135">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f4267-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f4267-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-bundle" } -->

```http
DELETE https://graph.microsoft.com/beta/drive/items/{bundle-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f4267-137">C#</span><span class="sxs-lookup"><span data-stu-id="f4267-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f4267-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4267-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f4267-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="f4267-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f4267-140">Java</span><span class="sxs-lookup"><span data-stu-id="f4267-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f4267-141">响应</span><span class="sxs-lookup"><span data-stu-id="f4267-141">Response</span></span>

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
