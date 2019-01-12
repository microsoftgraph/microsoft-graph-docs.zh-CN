---
author: chackman
ms.author: chackman
title: 按照驱动器项目
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 2323511604937366e9fd69c24f369523e5e6aebc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926188"
---
# <a name="follow-drive-item"></a><span data-ttu-id="74287-102">按照驱动器项目</span><span class="sxs-lookup"><span data-stu-id="74287-102">Follow drive item</span></span>

> <span data-ttu-id="74287-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="74287-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74287-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="74287-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="74287-105">按照[driveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="74287-105">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="74287-106">**注意：** 若要取消追随项目，请参阅[于取消追随项目](driveitem-unfollow.md)。</span><span class="sxs-lookup"><span data-stu-id="74287-106">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="74287-107">权限</span><span class="sxs-lookup"><span data-stu-id="74287-107">Permissions</span></span>

<span data-ttu-id="74287-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74287-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74287-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="74287-110">Permission type</span></span>      | <span data-ttu-id="74287-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="74287-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74287-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74287-112">Delegated (work or school account)</span></span> | <span data-ttu-id="74287-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74287-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="74287-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74287-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74287-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="74287-115">Not supported.</span></span>    |
|<span data-ttu-id="74287-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="74287-116">Application</span></span> | <span data-ttu-id="74287-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74287-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="74287-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74287-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="74287-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="74287-119">Request body</span></span>

<span data-ttu-id="74287-120">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="74287-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="74287-121">响应</span><span class="sxs-lookup"><span data-stu-id="74287-121">Response</span></span>

<span data-ttu-id="74287-122">此方法返回[DriveItem](../resources/driveitem.md)正在关注的项目。</span><span class="sxs-lookup"><span data-stu-id="74287-122">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="74287-123">示例</span><span class="sxs-lookup"><span data-stu-id="74287-123">Example</span></span>

<span data-ttu-id="74287-124">本示例遵循由标识项`{item-id}`。</span><span class="sxs-lookup"><span data-stu-id="74287-124">This example follows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "follow-item", "scopes": "files.read", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/follow
```

<!-- {
  "type": "#page.annotation",
  "description": "Follow an item.",
  "keywords": "follow item",
  "section": "documentation",
  "tocPath": "Items/Follow"
} -->

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
