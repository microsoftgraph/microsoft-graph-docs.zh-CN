---
author: chackman
description: 关注 driveItem。
title: 关注驱动器项
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 1c54d52760882ae35838ebadc11717a76c3b5fc8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963773"
---
# <a name="follow-drive-item"></a><span data-ttu-id="b3e6c-103">关注驱动器项</span><span class="sxs-lookup"><span data-stu-id="b3e6c-103">Follow drive item</span></span>

<span data-ttu-id="b3e6c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3e6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3e6c-105">关注 [driveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b3e6c-105">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="b3e6c-106">**注意：** 若要取消追随某个项目，请参阅取消 [追随项目](driveitem-unfollow.md)。</span><span class="sxs-lookup"><span data-stu-id="b3e6c-106">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b3e6c-107">权限</span><span class="sxs-lookup"><span data-stu-id="b3e6c-107">Permissions</span></span>

<span data-ttu-id="b3e6c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b3e6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3e6c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3e6c-110">Permission type</span></span>      | <span data-ttu-id="b3e6c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b3e6c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3e6c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3e6c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b3e6c-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3e6c-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b3e6c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3e6c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3e6c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3e6c-115">Not supported.</span></span>    |
|<span data-ttu-id="b3e6c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3e6c-116">Application</span></span> | <span data-ttu-id="b3e6c-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3e6c-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3e6c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3e6c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="b3e6c-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3e6c-119">Request body</span></span>

<span data-ttu-id="b3e6c-120">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="b3e6c-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="b3e6c-121">响应</span><span class="sxs-lookup"><span data-stu-id="b3e6c-121">Response</span></span>

<span data-ttu-id="b3e6c-122">此方法返回正在遵循的项的 [DriveItem](../resources/driveitem.md) 。</span><span class="sxs-lookup"><span data-stu-id="b3e6c-122">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="b3e6c-123">示例</span><span class="sxs-lookup"><span data-stu-id="b3e6c-123">Example</span></span>

<span data-ttu-id="b3e6c-124">本示例将遵循由标识的项目 `{item-id}` 。</span><span class="sxs-lookup"><span data-stu-id="b3e6c-124">This example follows an item identified by `{item-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="b3e6c-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3e6c-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "follow-item", "scopes": "files.read", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/follow
```
# <a name="c"></a>[<span data-ttu-id="b3e6c-126">C#</span><span class="sxs-lookup"><span data-stu-id="b3e6c-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/follow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3e6c-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3e6c-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/follow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3e6c-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3e6c-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/follow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3e6c-129">Java</span><span class="sxs-lookup"><span data-stu-id="b3e6c-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/follow-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!--
{
  "type": "#page.annotation",
  "description": "Follow an item.",
  "keywords": "follow item",
  "section": "documentation",
  "tocPath": "Items/Follow",
  "suppressions": [
  ]
}
-->

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1312abc!1231",
  "name": "March Proposal.docx",
  "size": 19121,
  "lastModifiedDateTime": "2017-12-12T10:40:59Z"
}
```


