---
author: JeremyKelley
title: 将项目添加到捆绑包
description: 将项目添加到 driveItems 捆绑包
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: f632b8054c1819c1af8bdd632c0d13092117cb30
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50774381"
---
# <a name="add-item-to-a-bundle"></a><span data-ttu-id="e7f0f-103">将项目添加到捆绑包</span><span class="sxs-lookup"><span data-stu-id="e7f0f-103">Add item to a bundle</span></span>

<span data-ttu-id="e7f0f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7f0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7f0f-105">将驱动器中的其他 [driveItem][] 添加到 [捆绑包][]。</span><span class="sxs-lookup"><span data-stu-id="e7f0f-105">Add an additional [driveItem][] from a drive to a [bundle][].</span></span>

[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md

## <a name="permissions"></a><span data-ttu-id="e7f0f-108">权限</span><span class="sxs-lookup"><span data-stu-id="e7f0f-108">Permissions</span></span>

<span data-ttu-id="e7f0f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e7f0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7f0f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7f0f-111">Permission type</span></span>      | <span data-ttu-id="e7f0f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e7f0f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7f0f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7f0f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e7f0f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7f0f-114">Not supported.</span></span>                             |
|<span data-ttu-id="e7f0f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7f0f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7f0f-116">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7f0f-116">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="e7f0f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e7f0f-117">Application</span></span>          | <span data-ttu-id="e7f0f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7f0f-118">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="e7f0f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7f0f-119">HTTP request</span></span>

```http
POST /drive/bundles/{bundle-id}/children
```

## <a name="request-headers"></a><span data-ttu-id="e7f0f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7f0f-120">Request headers</span></span>

| <span data-ttu-id="e7f0f-121">名称</span><span class="sxs-lookup"><span data-stu-id="e7f0f-121">Name</span></span>          | <span data-ttu-id="e7f0f-122">说明</span><span class="sxs-lookup"><span data-stu-id="e7f0f-122">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="e7f0f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7f0f-123">Authorization</span></span> | <span data-ttu-id="e7f0f-124">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="e7f0f-124">Bearer \{token\}.</span></span> <span data-ttu-id="e7f0f-125">必填。</span><span class="sxs-lookup"><span data-stu-id="e7f0f-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7f0f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7f0f-126">Request body</span></span>

<span data-ttu-id="e7f0f-127">请求正文包括应添加到捆绑包的子集合中的项目的标识符。</span><span class="sxs-lookup"><span data-stu-id="e7f0f-127">The request body includes the identifier for an item that should be added to the bundle's children collection.</span></span>

## <a name="response"></a><span data-ttu-id="e7f0f-128">响应</span><span class="sxs-lookup"><span data-stu-id="e7f0f-128">Response</span></span>

<span data-ttu-id="e7f0f-129">如果成功，响应为 `204 No Content` 。</span><span class="sxs-lookup"><span data-stu-id="e7f0f-129">If successful, the response is `204 No Content`.</span></span>

<span data-ttu-id="e7f0f-130">请阅读 [错误响应][error-response] 主题，了解有关如何返回错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e7f0f-130">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="e7f0f-131">示例</span><span class="sxs-lookup"><span data-stu-id="e7f0f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7f0f-132">请求</span><span class="sxs-lookup"><span data-stu-id="e7f0f-132">Request</span></span>

<span data-ttu-id="e7f0f-133">此请求将现有项添加到指定的捆绑包。</span><span class="sxs-lookup"><span data-stu-id="e7f0f-133">This request will add an existing item to the specified bundle.</span></span>


# <a name="http"></a>[<span data-ttu-id="e7f0f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7f0f-134">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "add-to-bundle", "isCollection": true, "@odata.type": "microsoft.graph.driveItem", "tags": "onedrive.only" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children
Content-Type: application/json

{
  "id": "123456!87"
}
```
# <a name="c"></a>[<span data-ttu-id="e7f0f-135">C#</span><span class="sxs-lookup"><span data-stu-id="e7f0f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-to-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e7f0f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7f0f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-to-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e7f0f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7f0f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-to-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e7f0f-138">Java</span><span class="sxs-lookup"><span data-stu-id="e7f0f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-to-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e7f0f-139">响应</span><span class="sxs-lookup"><span data-stu-id="e7f0f-139">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Add items to an existing bundle.",
  "keywords": "",
  "section": "documentation"
} -->


