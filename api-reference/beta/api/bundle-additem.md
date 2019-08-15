---
author: JeremyKelley
ms.author: jeremyke
title: 将项目添加到捆绑包
description: 将项目添加到 Driveitem 捆绑包
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e31fed6b88164ea305d820fb227ae71da9337226
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419242"
---
# <a name="add-item-to-a-bundle"></a><span data-ttu-id="338c9-103">将项目添加到捆绑包</span><span class="sxs-lookup"><span data-stu-id="338c9-103">Add item to a bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="338c9-104">将其他[driveItem][]从驱动器添加到[捆绑包][]中。</span><span class="sxs-lookup"><span data-stu-id="338c9-104">Add an additional [driveItem][] from a drive to a [bundle][].</span></span>

[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md

## <a name="permissions"></a><span data-ttu-id="338c9-107">权限</span><span class="sxs-lookup"><span data-stu-id="338c9-107">Permissions</span></span>

<span data-ttu-id="338c9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="338c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="338c9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="338c9-110">Permission type</span></span>      | <span data-ttu-id="338c9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="338c9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="338c9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="338c9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="338c9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="338c9-113">Not supported.</span></span>                             |
|<span data-ttu-id="338c9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="338c9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="338c9-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="338c9-115">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="338c9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="338c9-116">Application</span></span>          | <span data-ttu-id="338c9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="338c9-117">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="338c9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="338c9-118">HTTP request</span></span>

```http
POST /drive/bundles/{bundle-id}/children
```

## <a name="request-headers"></a><span data-ttu-id="338c9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="338c9-119">Request headers</span></span>

| <span data-ttu-id="338c9-120">名称</span><span class="sxs-lookup"><span data-stu-id="338c9-120">Name</span></span>          | <span data-ttu-id="338c9-121">说明</span><span class="sxs-lookup"><span data-stu-id="338c9-121">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="338c9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="338c9-122">Authorization</span></span> | <span data-ttu-id="338c9-123">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="338c9-123">Bearer \{token\}.</span></span> <span data-ttu-id="338c9-124">必需。</span><span class="sxs-lookup"><span data-stu-id="338c9-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="338c9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="338c9-125">Request body</span></span>

<span data-ttu-id="338c9-126">请求正文包括应添加到捆绑的子集合中的项的标识符。</span><span class="sxs-lookup"><span data-stu-id="338c9-126">The request body includes the identifier for an item that should be added to the bundle's children collection.</span></span>

## <a name="response"></a><span data-ttu-id="338c9-127">响应</span><span class="sxs-lookup"><span data-stu-id="338c9-127">Response</span></span>

<span data-ttu-id="338c9-128">如果成功, 响应为`204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="338c9-128">If successful, the response is `204 No Content`.</span></span>

<span data-ttu-id="338c9-129">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="338c9-129">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="338c9-130">示例</span><span class="sxs-lookup"><span data-stu-id="338c9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="338c9-131">请求</span><span class="sxs-lookup"><span data-stu-id="338c9-131">Request</span></span>

<span data-ttu-id="338c9-132">此请求将现有项添加到指定的捆绑包中。</span><span class="sxs-lookup"><span data-stu-id="338c9-132">This request will add an existing item to the specified bundle.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="338c9-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="338c9-133">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "add-to-bundle", "isCollection": true, "@odata.type": "microsoft.graph.driveItem", "tags": "onedrive.only" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children
Content-Type: application/json

{
  "id": "123456!87"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="338c9-134">C#</span><span class="sxs-lookup"><span data-stu-id="338c9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-to-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="338c9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="338c9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-to-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="338c9-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="338c9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-to-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="338c9-137">响应</span><span class="sxs-lookup"><span data-stu-id="338c9-137">Response</span></span>

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
