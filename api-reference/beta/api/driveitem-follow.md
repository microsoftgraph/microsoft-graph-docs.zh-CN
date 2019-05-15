---
author: chackman
ms.author: chackman
title: 关注驱动器项
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e62f256e9c4c0832b2f1ef71713c57b596d2a811
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2019
ms.locfileid: "33960877"
---
# <a name="follow-drive-item"></a><span data-ttu-id="847bb-102">关注驱动器项</span><span class="sxs-lookup"><span data-stu-id="847bb-102">Follow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="847bb-103">关注[driveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="847bb-103">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="847bb-104">**注意:** 若要取消追随某个项目, 请参阅取消[追随项目](driveitem-unfollow.md)。</span><span class="sxs-lookup"><span data-stu-id="847bb-104">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="847bb-105">权限</span><span class="sxs-lookup"><span data-stu-id="847bb-105">Permissions</span></span>

<span data-ttu-id="847bb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="847bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="847bb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="847bb-108">Permission type</span></span>      | <span data-ttu-id="847bb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="847bb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="847bb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="847bb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="847bb-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="847bb-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="847bb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="847bb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="847bb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="847bb-113">Not supported.</span></span>    |
|<span data-ttu-id="847bb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="847bb-114">Application</span></span> | <span data-ttu-id="847bb-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="847bb-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="847bb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="847bb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="847bb-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="847bb-117">Request body</span></span>

<span data-ttu-id="847bb-118">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="847bb-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="847bb-119">响应</span><span class="sxs-lookup"><span data-stu-id="847bb-119">Response</span></span>

<span data-ttu-id="847bb-120">此方法返回正在遵循的项的[DriveItem](../resources/driveitem.md) 。</span><span class="sxs-lookup"><span data-stu-id="847bb-120">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="847bb-121">示例</span><span class="sxs-lookup"><span data-stu-id="847bb-121">Example</span></span>

<span data-ttu-id="847bb-122">本示例将遵循由标识的`{item-id}`项目。</span><span class="sxs-lookup"><span data-stu-id="847bb-122">This example follows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "follow-item", "scopes": "files.read", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/follow
```

<!--
{
  "type": "#page.annotation",
  "description": "Follow an item.",
  "keywords": "follow item",
  "section": "documentation",
  "tocPath": "Items/Follow",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-follow.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-follow.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="847bb-123">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="847bb-123">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="847bb-124">C#</span><span class="sxs-lookup"><span data-stu-id="847bb-124">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/follow-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="847bb-125">Javascript</span><span class="sxs-lookup"><span data-stu-id="847bb-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/follow-item-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
