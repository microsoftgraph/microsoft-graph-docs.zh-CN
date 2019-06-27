---
author: chackman
ms.author: chackman
title: 关注驱动器项
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: fb38ce7ed2d362ec808144931d218dc1c012eeab
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260184"
---
# <a name="follow-drive-item"></a><span data-ttu-id="06cc1-102">关注驱动器项</span><span class="sxs-lookup"><span data-stu-id="06cc1-102">Follow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06cc1-103">关注[driveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="06cc1-103">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="06cc1-104">**注意:** 若要取消追随某个项目, 请参阅取消[追随项目](driveitem-unfollow.md)。</span><span class="sxs-lookup"><span data-stu-id="06cc1-104">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="06cc1-105">权限</span><span class="sxs-lookup"><span data-stu-id="06cc1-105">Permissions</span></span>

<span data-ttu-id="06cc1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06cc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06cc1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="06cc1-108">Permission type</span></span>      | <span data-ttu-id="06cc1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="06cc1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06cc1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06cc1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="06cc1-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06cc1-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="06cc1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06cc1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06cc1-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="06cc1-113">Not supported.</span></span>    |
|<span data-ttu-id="06cc1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="06cc1-114">Application</span></span> | <span data-ttu-id="06cc1-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06cc1-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06cc1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06cc1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="06cc1-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="06cc1-117">Request body</span></span>

<span data-ttu-id="06cc1-118">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="06cc1-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="06cc1-119">响应</span><span class="sxs-lookup"><span data-stu-id="06cc1-119">Response</span></span>

<span data-ttu-id="06cc1-120">此方法返回正在遵循的项的[DriveItem](../resources/driveitem.md) 。</span><span class="sxs-lookup"><span data-stu-id="06cc1-120">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="06cc1-121">示例</span><span class="sxs-lookup"><span data-stu-id="06cc1-121">Example</span></span>

<span data-ttu-id="06cc1-122">本示例将遵循由标识的`{item-id}`项目。</span><span class="sxs-lookup"><span data-stu-id="06cc1-122">This example follows an item identified by `{item-id}`.</span></span>

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
    "Error: /api-reference/beta/api/driveitem-follow.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/driveitem-follow.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/driveitem-follow.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="06cc1-123">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="06cc1-123">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="06cc1-124">C#</span><span class="sxs-lookup"><span data-stu-id="06cc1-124">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/follow-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="06cc1-125">Javascript</span><span class="sxs-lookup"><span data-stu-id="06cc1-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/follow-item-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="06cc1-126">目标-C</span><span class="sxs-lookup"><span data-stu-id="06cc1-126">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/follow-item-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
