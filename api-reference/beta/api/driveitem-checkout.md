---
author: JeremyKelley
description: 签出 driveItem 资源以防止在签入文档前其他人编辑文档和看到所做的更改。
ms.date: 09/10/2017
title: 签出文件
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: eeaa36c2aa71469572a31f02b5692727508a62fe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957225"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="17a19-103">签出 DriveItem 资源</span><span class="sxs-lookup"><span data-stu-id="17a19-103">Check-out a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17a19-104">签出 driveItem 资源以防止在[签入](driveitem-checkin.md)文档前其他人编辑文档和看到所做的更改。</span><span class="sxs-lookup"><span data-stu-id="17a19-104">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="17a19-105">权限</span><span class="sxs-lookup"><span data-stu-id="17a19-105">Permissions</span></span>

<span data-ttu-id="17a19-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17a19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17a19-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="17a19-108">Permission type</span></span>      | <span data-ttu-id="17a19-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="17a19-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17a19-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17a19-110">Delegated (work or school account)</span></span> | <span data-ttu-id="17a19-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17a19-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="17a19-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17a19-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17a19-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17a19-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="17a19-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="17a19-114">Application</span></span> | <span data-ttu-id="17a19-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17a19-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17a19-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17a19-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="17a19-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="17a19-117">Request body</span></span>

<span data-ttu-id="17a19-118">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="17a19-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="17a19-119">示例</span><span class="sxs-lookup"><span data-stu-id="17a19-119">Example</span></span>

<span data-ttu-id="17a19-120">本示例签出由 `{item-id}` 标识的文件。</span><span class="sxs-lookup"><span data-stu-id="17a19-120">This example checks out a file identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="17a19-121">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="17a19-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="17a19-122">C#</span><span class="sxs-lookup"><span data-stu-id="17a19-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkout-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="17a19-123">Javascript</span><span class="sxs-lookup"><span data-stu-id="17a19-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkout-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="17a19-124">目标-C</span><span class="sxs-lookup"><span data-stu-id="17a19-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkout-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="17a19-125">Java</span><span class="sxs-lookup"><span data-stu-id="17a19-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/checkout-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="17a19-126">响应</span><span class="sxs-lookup"><span data-stu-id="17a19-126">Response</span></span>

<span data-ttu-id="17a19-127">如果成功，该 API 调用会返回 `204 No content`。</span><span class="sxs-lookup"><span data-stu-id="17a19-127">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="17a19-128">注解</span><span class="sxs-lookup"><span data-stu-id="17a19-128">Remarks</span></span>


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
