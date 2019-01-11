---
author: chackman
ms.author: chackman
title: 取消追随驱动器项目
localization_priority: Normal
ms.openlocfilehash: 6d2b47b0d243f2b13b390a9e0121e4174d8f75bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883704"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="6be32-102">取消追随驱动器项目</span><span class="sxs-lookup"><span data-stu-id="6be32-102">Unfollow drive item</span></span>

> <span data-ttu-id="6be32-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6be32-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6be32-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6be32-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6be32-105">取消追随[driveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="6be32-105">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="6be32-106">**注意：** 若要执行项目，请参阅[按照项目](driveitem-follow.md)。</span><span class="sxs-lookup"><span data-stu-id="6be32-106">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6be32-107">权限</span><span class="sxs-lookup"><span data-stu-id="6be32-107">Permissions</span></span>

<span data-ttu-id="6be32-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6be32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6be32-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6be32-110">Permission type</span></span>      | <span data-ttu-id="6be32-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6be32-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6be32-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6be32-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6be32-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6be32-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6be32-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6be32-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6be32-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6be32-115">Not supported.</span></span>    |
|<span data-ttu-id="6be32-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6be32-116">Application</span></span> | <span data-ttu-id="6be32-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6be32-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6be32-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6be32-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id} 
DELETE /users/{user-id}/drive/following/{item-id}
```

## <a name="request-body"></a><span data-ttu-id="6be32-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="6be32-119">Request body</span></span>

<span data-ttu-id="6be32-120">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="6be32-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="6be32-121">响应</span><span class="sxs-lookup"><span data-stu-id="6be32-121">Response</span></span>

<span data-ttu-id="6be32-122">如果成功，该 API 调用会返回 `204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="6be32-122">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="6be32-123">示例</span><span class="sxs-lookup"><span data-stu-id="6be32-123">Example</span></span>

<span data-ttu-id="6be32-124">本示例 unfollows 由标识项`{item-id}`。</span><span class="sxs-lookup"><span data-stu-id="6be32-124">This example unfollows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/following/{item-id}
```


<!-- {
  "type": "#page.annotation",
  "description": "Unfollow an item that the user is following.",
  "keywords": "unfollow item",
  "section": "documentation",
  "tocPath": "Items/Unfollow"
} -->
