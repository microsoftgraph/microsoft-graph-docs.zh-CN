---
author: learafa
description: 关注 driveItem。
title: 关注驱动器项
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 86467b3acdd5e9ef70b393ecdbec2652341af5b2
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124355"
---
# <a name="follow-drive-item"></a><span data-ttu-id="6d117-103">关注驱动器项</span><span class="sxs-lookup"><span data-stu-id="6d117-103">Follow drive item</span></span>

<span data-ttu-id="6d117-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d117-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6d117-105">关注[driveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="6d117-105">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="6d117-106">**注意：** 若要取消追随某个项目，请参阅取消[追随项目](driveitem-unfollow.md)。</span><span class="sxs-lookup"><span data-stu-id="6d117-106">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6d117-107">权限</span><span class="sxs-lookup"><span data-stu-id="6d117-107">Permissions</span></span>

<span data-ttu-id="6d117-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6d117-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d117-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d117-110">Permission type</span></span>      | <span data-ttu-id="6d117-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6d117-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d117-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d117-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6d117-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d117-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6d117-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6d117-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d117-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d117-115">Not supported.</span></span>    |
|<span data-ttu-id="6d117-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d117-116">Application</span></span> | <span data-ttu-id="6d117-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d117-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d117-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d117-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="6d117-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d117-119">Request body</span></span>

<span data-ttu-id="6d117-120">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="6d117-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="6d117-121">响应</span><span class="sxs-lookup"><span data-stu-id="6d117-121">Response</span></span>

<span data-ttu-id="6d117-122">此方法返回正在遵循的项的[DriveItem](../resources/driveitem.md) 。</span><span class="sxs-lookup"><span data-stu-id="6d117-122">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="6d117-123">示例</span><span class="sxs-lookup"><span data-stu-id="6d117-123">Example</span></span>

<span data-ttu-id="6d117-124">本示例将遵循由标识的`{item-id}`项目。</span><span class="sxs-lookup"><span data-stu-id="6d117-124">This example follows an item identified by `{item-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="6d117-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d117-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "follow-item", "scopes": "files.read", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/follow
```
# <a name="c"></a>[<span data-ttu-id="6d117-126">C#</span><span class="sxs-lookup"><span data-stu-id="6d117-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/follow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d117-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d117-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/follow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d117-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d117-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/follow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6d117-129">Java</span><span class="sxs-lookup"><span data-stu-id="6d117-129">Java</span></span>](#tab/java)
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
