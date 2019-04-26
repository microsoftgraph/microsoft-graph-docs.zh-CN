---
author: chackman
ms.author: chackman
title: 取消追随驱动器项目
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1cd3976feb643d8553920df624e30d232c5b5ed4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325338"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="ba37d-102">取消追随驱动器项目</span><span class="sxs-lookup"><span data-stu-id="ba37d-102">Unfollow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba37d-103">取消追随[driveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="ba37d-103">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="ba37d-104">**注意:** 若要关注某个项目, 请参阅 "[关注项](driveitem-follow.md)"。</span><span class="sxs-lookup"><span data-stu-id="ba37d-104">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ba37d-105">权限</span><span class="sxs-lookup"><span data-stu-id="ba37d-105">Permissions</span></span>

<span data-ttu-id="ba37d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba37d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba37d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba37d-108">Permission type</span></span>      | <span data-ttu-id="ba37d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba37d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba37d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba37d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ba37d-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba37d-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ba37d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba37d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba37d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba37d-113">Not supported.</span></span>    |
|<span data-ttu-id="ba37d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba37d-114">Application</span></span> | <span data-ttu-id="ba37d-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba37d-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba37d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba37d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id} 
DELETE /users/{user-id}/drive/following/{item-id}
```

## <a name="request-body"></a><span data-ttu-id="ba37d-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba37d-117">Request body</span></span>

<span data-ttu-id="ba37d-118">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="ba37d-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="ba37d-119">响应</span><span class="sxs-lookup"><span data-stu-id="ba37d-119">Response</span></span>

<span data-ttu-id="ba37d-120">如果成功，该 API 调用会返回 `204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="ba37d-120">If successful, the API call returns a `204 No Content`.</span></span> <span data-ttu-id="ba37d-121">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ba37d-121">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba37d-122">示例</span><span class="sxs-lookup"><span data-stu-id="ba37d-122">Example</span></span>
### <a name="request"></a><span data-ttu-id="ba37d-123">请求</span><span class="sxs-lookup"><span data-stu-id="ba37d-123">Request</span></span>
<span data-ttu-id="ba37d-124">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ba37d-124">Here is an example of the request.</span></span>
<span data-ttu-id="ba37d-125">本示例将 unfollows 标识为的`{item-id}`项目。</span><span class="sxs-lookup"><span data-stu-id="ba37d-125">This example unfollows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/following/{item-id}
```
### <a name="response"></a><span data-ttu-id="ba37d-126">响应</span><span class="sxs-lookup"><span data-stu-id="ba37d-126">Response</span></span>
<!-- { 
    "blockType": "response", 
    "truncated": true 
} -->
```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "description": "Unfollow an item that the user is following.",
  "keywords": "unfollow item",
  "section": "documentation",
  "tocPath": "Items/Unfollow",
  "suppressions": []
}
-->
