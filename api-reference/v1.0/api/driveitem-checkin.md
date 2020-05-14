---
author: learafa
description: 签入已签出的 driveItem 资源，使其他用户可以使用该文档的版本。
title: driveItem：签入
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 7cf999dc338c4a16a4040e8b48b4824c6da09e94
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "43511119"
---
# <a name="driveitem-checkin"></a><span data-ttu-id="70cf9-103">driveItem：签入</span><span class="sxs-lookup"><span data-stu-id="70cf9-103">driveItem: checkin</span></span>

<span data-ttu-id="70cf9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70cf9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70cf9-105">签入已签出的**driveItem**资源，使其他用户可以使用该文档的版本。</span><span class="sxs-lookup"><span data-stu-id="70cf9-105">Check in a checked out **driveItem** resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="70cf9-106">权限</span><span class="sxs-lookup"><span data-stu-id="70cf9-106">Permissions</span></span>

<span data-ttu-id="70cf9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70cf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70cf9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="70cf9-109">Permission type</span></span>      | <span data-ttu-id="70cf9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70cf9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70cf9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70cf9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="70cf9-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70cf9-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="70cf9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70cf9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70cf9-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70cf9-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="70cf9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="70cf9-115">Application</span></span> | <span data-ttu-id="70cf9-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70cf9-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70cf9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70cf9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

## <a name="request-body"></a><span data-ttu-id="70cf9-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="70cf9-118">Request body</span></span>

<span data-ttu-id="70cf9-119">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="70cf9-119">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="70cf9-120">名称</span><span class="sxs-lookup"><span data-stu-id="70cf9-120">Name</span></span>    | <span data-ttu-id="70cf9-121">值</span><span class="sxs-lookup"><span data-stu-id="70cf9-121">Value</span></span>  |                                                <span data-ttu-id="70cf9-122">说明</span><span class="sxs-lookup"><span data-stu-id="70cf9-122">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="70cf9-123">checkInAs</span><span class="sxs-lookup"><span data-stu-id="70cf9-123">checkInAs</span></span> | <span data-ttu-id="70cf9-124">字符串</span><span class="sxs-lookup"><span data-stu-id="70cf9-124">string</span></span> | <span data-ttu-id="70cf9-125">可选。</span><span class="sxs-lookup"><span data-stu-id="70cf9-125">Optional.</span></span> <span data-ttu-id="70cf9-126">签入操作完成后的文档状态。</span><span class="sxs-lookup"><span data-stu-id="70cf9-126">The status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="70cf9-127">可以是 `published` 或未指定。</span><span class="sxs-lookup"><span data-stu-id="70cf9-127">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="70cf9-128">comment</span><span class="sxs-lookup"><span data-stu-id="70cf9-128">comment</span></span>   | <span data-ttu-id="70cf9-129">string</span><span class="sxs-lookup"><span data-stu-id="70cf9-129">string</span></span> | <span data-ttu-id="70cf9-130">与此版本相关联的签入注释。</span><span class="sxs-lookup"><span data-stu-id="70cf9-130">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="response"></a><span data-ttu-id="70cf9-131">响应</span><span class="sxs-lookup"><span data-stu-id="70cf9-131">Response</span></span>

<span data-ttu-id="70cf9-132">如果成功，API 调用将返回 `204 No content` 。</span><span class="sxs-lookup"><span data-stu-id="70cf9-132">If successful, the API call returns `204 No content`.</span></span>

## <a name="example"></a><span data-ttu-id="70cf9-133">示例</span><span class="sxs-lookup"><span data-stu-id="70cf9-133">Example</span></span>

<span data-ttu-id="70cf9-134">本示例签入由 `{item-id}` 标识的文件。</span><span class="sxs-lookup"><span data-stu-id="70cf9-134">This example checks in a file identified by `{item-id}`.</span></span>

### <a name="request"></a><span data-ttu-id="70cf9-135">请求</span><span class="sxs-lookup"><span data-stu-id="70cf9-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="70cf9-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="70cf9-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```
# <a name="c"></a>[<span data-ttu-id="70cf9-137">C#</span><span class="sxs-lookup"><span data-stu-id="70cf9-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkin-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70cf9-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70cf9-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkin-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70cf9-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70cf9-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkin-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70cf9-140">Java</span><span class="sxs-lookup"><span data-stu-id="70cf9-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/checkin-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="70cf9-141">响应</span><span class="sxs-lookup"><span data-stu-id="70cf9-141">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
}
-->
