---
author: chackman
description: 关注 driveItem。
title: 关注驱动器项
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: dfd334dfa2356c33138f566e8d591af410b832d0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324396"
---
# <a name="follow-drive-item"></a><span data-ttu-id="943db-103">关注驱动器项</span><span class="sxs-lookup"><span data-stu-id="943db-103">Follow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="943db-104">关注[driveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="943db-104">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="943db-105">**注意:** 若要取消追随某个项目, 请参阅取消[追随项目](driveitem-unfollow.md)。</span><span class="sxs-lookup"><span data-stu-id="943db-105">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="943db-106">权限</span><span class="sxs-lookup"><span data-stu-id="943db-106">Permissions</span></span>

<span data-ttu-id="943db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="943db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="943db-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="943db-109">Permission type</span></span>      | <span data-ttu-id="943db-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="943db-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="943db-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="943db-111">Delegated (work or school account)</span></span> | <span data-ttu-id="943db-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="943db-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="943db-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="943db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="943db-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="943db-114">Not supported.</span></span>    |
|<span data-ttu-id="943db-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="943db-115">Application</span></span> | <span data-ttu-id="943db-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="943db-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="943db-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="943db-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="943db-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="943db-118">Request body</span></span>

<span data-ttu-id="943db-119">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="943db-119">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="943db-120">响应</span><span class="sxs-lookup"><span data-stu-id="943db-120">Response</span></span>

<span data-ttu-id="943db-121">此方法返回正在遵循的项的[DriveItem](../resources/driveitem.md) 。</span><span class="sxs-lookup"><span data-stu-id="943db-121">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="943db-122">示例</span><span class="sxs-lookup"><span data-stu-id="943db-122">Example</span></span>

<span data-ttu-id="943db-123">本示例将遵循由标识的`{item-id}`项目。</span><span class="sxs-lookup"><span data-stu-id="943db-123">This example follows an item identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="943db-124">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="943db-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "follow-item", "scopes": "files.read", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/follow
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="943db-125">C#</span><span class="sxs-lookup"><span data-stu-id="943db-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/follow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="943db-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="943db-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/follow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="943db-127">目标-C</span><span class="sxs-lookup"><span data-stu-id="943db-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/follow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="943db-128">Java</span><span class="sxs-lookup"><span data-stu-id="943db-128">Java</span></span>](#tab/java)
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
