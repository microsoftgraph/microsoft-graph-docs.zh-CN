---
author: JeremyKelley
description: 签入已签出的 DriveItem 资源，为其他人提供文档版本。
ms.date: 09/10/2017
title: 签入文件
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: ffdddf5e3800d2bfb14038c7bec5b1b8fdcb0809
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321058"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="3e372-103">签入对 DriveItem 资源的更改</span><span class="sxs-lookup"><span data-stu-id="3e372-103">Check-in changes to a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e372-104">签入已签出的 DriveItem 资源，为其他人提供文档版本。</span><span class="sxs-lookup"><span data-stu-id="3e372-104">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e372-105">权限</span><span class="sxs-lookup"><span data-stu-id="3e372-105">Permissions</span></span>

<span data-ttu-id="3e372-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e372-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e372-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e372-108">Permission type</span></span>      | <span data-ttu-id="3e372-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e372-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e372-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e372-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3e372-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e372-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3e372-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e372-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e372-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e372-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="3e372-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e372-114">Application</span></span> | <span data-ttu-id="3e372-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e372-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e372-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e372-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="3e372-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e372-117">Request body</span></span>

<span data-ttu-id="3e372-118">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3e372-118">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="3e372-119">名称</span><span class="sxs-lookup"><span data-stu-id="3e372-119">Name</span></span>    | <span data-ttu-id="3e372-120">值</span><span class="sxs-lookup"><span data-stu-id="3e372-120">Value</span></span>  |                                                <span data-ttu-id="3e372-121">说明</span><span class="sxs-lookup"><span data-stu-id="3e372-121">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="3e372-122">checkInAs</span><span class="sxs-lookup"><span data-stu-id="3e372-122">checkInAs</span></span> | <span data-ttu-id="3e372-123">字符串</span><span class="sxs-lookup"><span data-stu-id="3e372-123">string</span></span> | <span data-ttu-id="3e372-124">可选。</span><span class="sxs-lookup"><span data-stu-id="3e372-124">Optional.</span></span> <span data-ttu-id="3e372-125">完成签入操作后文档的所需状态。</span><span class="sxs-lookup"><span data-stu-id="3e372-125">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="3e372-126">可以是 `published` 或未指定。</span><span class="sxs-lookup"><span data-stu-id="3e372-126">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="3e372-127">comment</span><span class="sxs-lookup"><span data-stu-id="3e372-127">comment</span></span>   | <span data-ttu-id="3e372-128">string</span><span class="sxs-lookup"><span data-stu-id="3e372-128">string</span></span> | <span data-ttu-id="3e372-129">与此版本相关联的签入注释。</span><span class="sxs-lookup"><span data-stu-id="3e372-129">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="3e372-130">示例</span><span class="sxs-lookup"><span data-stu-id="3e372-130">Example</span></span>

<span data-ttu-id="3e372-131">本示例签入由 `{item-id}` 标识的文件。</span><span class="sxs-lookup"><span data-stu-id="3e372-131">This example checks in a file identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3e372-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="3e372-132">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3e372-133">C#</span><span class="sxs-lookup"><span data-stu-id="3e372-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkin-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3e372-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e372-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkin-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3e372-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="3e372-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkin-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3e372-136">Java</span><span class="sxs-lookup"><span data-stu-id="3e372-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/checkin-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="3e372-137">响应</span><span class="sxs-lookup"><span data-stu-id="3e372-137">Response</span></span>

<span data-ttu-id="3e372-138">如果成功，该 API 调用会返回 `204 No content`。</span><span class="sxs-lookup"><span data-stu-id="3e372-138">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="3e372-139">注解</span><span class="sxs-lookup"><span data-stu-id="3e372-139">Remarks</span></span>


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
