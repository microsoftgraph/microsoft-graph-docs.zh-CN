---
author: JeremyKelley
description: 签入已签出的 DriveItem 资源，使其他用户可以使用该文档的版本。
title: driveItem：签入
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 92200c0e079a885192f2ad1709a1e45bb15370e2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982162"
---
# <a name="driveitem-checkin"></a><span data-ttu-id="de53e-103">driveItem：签入</span><span class="sxs-lookup"><span data-stu-id="de53e-103">driveItem: checkin</span></span>

<span data-ttu-id="de53e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de53e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de53e-105">签入已签出的 **driveItem** 资源，使其他用户可以使用该文档的版本。</span><span class="sxs-lookup"><span data-stu-id="de53e-105">Check in a checked out **driveItem** resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="de53e-106">权限</span><span class="sxs-lookup"><span data-stu-id="de53e-106">Permissions</span></span>

<span data-ttu-id="de53e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de53e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de53e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="de53e-109">Permission type</span></span>      | <span data-ttu-id="de53e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="de53e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de53e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de53e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="de53e-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de53e-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="de53e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de53e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de53e-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de53e-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="de53e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="de53e-115">Application</span></span> | <span data-ttu-id="de53e-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de53e-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="de53e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de53e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="de53e-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="de53e-118">Request body</span></span>

<span data-ttu-id="de53e-119">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="de53e-119">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="de53e-120">名称</span><span class="sxs-lookup"><span data-stu-id="de53e-120">Name</span></span>    | <span data-ttu-id="de53e-121">值</span><span class="sxs-lookup"><span data-stu-id="de53e-121">Value</span></span>  |                                                <span data-ttu-id="de53e-122">说明</span><span class="sxs-lookup"><span data-stu-id="de53e-122">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="de53e-123">checkInAs</span><span class="sxs-lookup"><span data-stu-id="de53e-123">checkInAs</span></span> | <span data-ttu-id="de53e-124">string</span><span class="sxs-lookup"><span data-stu-id="de53e-124">string</span></span> | <span data-ttu-id="de53e-125">可选。</span><span class="sxs-lookup"><span data-stu-id="de53e-125">Optional.</span></span> <span data-ttu-id="de53e-126">签入操作完成后的文档状态。</span><span class="sxs-lookup"><span data-stu-id="de53e-126">The status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="de53e-127">可以是 `published` 或未指定。</span><span class="sxs-lookup"><span data-stu-id="de53e-127">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="de53e-128">comment</span><span class="sxs-lookup"><span data-stu-id="de53e-128">comment</span></span>   | <span data-ttu-id="de53e-129">string</span><span class="sxs-lookup"><span data-stu-id="de53e-129">string</span></span> | <span data-ttu-id="de53e-130">与此版本相关联的签入注释。</span><span class="sxs-lookup"><span data-stu-id="de53e-130">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="de53e-131">示例</span><span class="sxs-lookup"><span data-stu-id="de53e-131">Example</span></span>

<span data-ttu-id="de53e-132">本示例签入由 `{item-id}` 标识的文件。</span><span class="sxs-lookup"><span data-stu-id="de53e-132">This example checks in a file identified by `{item-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="de53e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="de53e-133">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```
# <a name="c"></a>[<span data-ttu-id="de53e-134">C#</span><span class="sxs-lookup"><span data-stu-id="de53e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkin-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de53e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de53e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkin-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de53e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de53e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkin-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="de53e-137">响应</span><span class="sxs-lookup"><span data-stu-id="de53e-137">Response</span></span>

<span data-ttu-id="de53e-138">如果成功，该 API 调用会返回 `204 No content`。</span><span class="sxs-lookup"><span data-stu-id="de53e-138">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="de53e-139">注解</span><span class="sxs-lookup"><span data-stu-id="de53e-139">Remarks</span></span>


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


