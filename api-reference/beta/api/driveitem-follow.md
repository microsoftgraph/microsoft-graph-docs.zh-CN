---
author: chackman
ms.author: chackman
title: 关注驱动器项
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b0c8835593ed7203cc6239485f1dcd4f17f24fe7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454403"
---
# <a name="follow-drive-item"></a><span data-ttu-id="78791-102">关注驱动器项</span><span class="sxs-lookup"><span data-stu-id="78791-102">Follow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78791-103">关注[driveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="78791-103">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="78791-104">**注意:** 若要取消追随某个项目, 请参阅取消[追随项目](driveitem-unfollow.md)。</span><span class="sxs-lookup"><span data-stu-id="78791-104">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="78791-105">权限</span><span class="sxs-lookup"><span data-stu-id="78791-105">Permissions</span></span>

<span data-ttu-id="78791-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78791-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78791-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="78791-108">Permission type</span></span>      | <span data-ttu-id="78791-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="78791-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78791-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78791-110">Delegated (work or school account)</span></span> | <span data-ttu-id="78791-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78791-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="78791-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78791-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78791-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="78791-113">Not supported.</span></span>    |
|<span data-ttu-id="78791-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="78791-114">Application</span></span> | <span data-ttu-id="78791-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78791-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="78791-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78791-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="78791-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="78791-117">Request body</span></span>

<span data-ttu-id="78791-118">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="78791-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="78791-119">响应</span><span class="sxs-lookup"><span data-stu-id="78791-119">Response</span></span>

<span data-ttu-id="78791-120">此方法返回正在遵循的项的[DriveItem](../resources/driveitem.md) 。</span><span class="sxs-lookup"><span data-stu-id="78791-120">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="78791-121">示例</span><span class="sxs-lookup"><span data-stu-id="78791-121">Example</span></span>

<span data-ttu-id="78791-122">本示例将遵循由标识的`{item-id}`项目。</span><span class="sxs-lookup"><span data-stu-id="78791-122">This example follows an item identified by `{item-id}`.</span></span>

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
    "Error: /api-reference/beta/api/driveitem-follow.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
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
