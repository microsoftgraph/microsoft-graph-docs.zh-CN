---
author: chackman
ms.author: chackman
title: 取消追随驱动器项目
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 064ab2d5ad86df5341a0f2f5a46fe7c227ff35fb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513107"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="e4f2d-102">取消追随驱动器项目</span><span class="sxs-lookup"><span data-stu-id="e4f2d-102">Unfollow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4f2d-103">取消追随[driveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="e4f2d-103">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="e4f2d-104">**注意：** 若要执行项目，请参阅[按照项目](driveitem-follow.md)。</span><span class="sxs-lookup"><span data-stu-id="e4f2d-104">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e4f2d-105">权限</span><span class="sxs-lookup"><span data-stu-id="e4f2d-105">Permissions</span></span>

<span data-ttu-id="e4f2d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4f2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4f2d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4f2d-108">Permission type</span></span>      | <span data-ttu-id="e4f2d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e4f2d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4f2d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4f2d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e4f2d-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4f2d-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e4f2d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4f2d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4f2d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4f2d-113">Not supported.</span></span>    |
|<span data-ttu-id="e4f2d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4f2d-114">Application</span></span> | <span data-ttu-id="e4f2d-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4f2d-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4f2d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4f2d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id} 
DELETE /users/{user-id}/drive/following/{item-id}
```

## <a name="request-body"></a><span data-ttu-id="e4f2d-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4f2d-117">Request body</span></span>

<span data-ttu-id="e4f2d-118">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="e4f2d-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="e4f2d-119">响应</span><span class="sxs-lookup"><span data-stu-id="e4f2d-119">Response</span></span>

<span data-ttu-id="e4f2d-120">如果成功，该 API 调用会返回 `204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="e4f2d-120">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="e4f2d-121">示例</span><span class="sxs-lookup"><span data-stu-id="e4f2d-121">Example</span></span>

<span data-ttu-id="e4f2d-122">本示例 unfollows 由标识项`{item-id}`。</span><span class="sxs-lookup"><span data-stu-id="e4f2d-122">This example unfollows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/following/{item-id}
```


<!--
{
  "type": "#page.annotation",
  "description": "Unfollow an item that the user is following.",
  "keywords": "unfollow item",
  "section": "documentation",
  "tocPath": "Items/Unfollow",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-unfollow.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
