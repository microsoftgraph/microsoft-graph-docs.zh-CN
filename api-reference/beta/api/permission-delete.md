---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 删除对项目的访问权限
localization_priority: Normal
ms.openlocfilehash: 3cc4f6a151d2990c5180e02888484e1260704f04
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539464"
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a><span data-ttu-id="ad0e1-102">从文件或文件夹中删除共享权限</span><span class="sxs-lookup"><span data-stu-id="ad0e1-102">Delete a sharing permission from a file or folder</span></span>

<span data-ttu-id="ad0e1-103">删除 [DriveItem](../resources/driveitem.md) 访问权限。</span><span class="sxs-lookup"><span data-stu-id="ad0e1-103">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="ad0e1-104">只能删除**非**继承的共享权限。</span><span class="sxs-lookup"><span data-stu-id="ad0e1-104">Only sharing permissions that are **not** inherited can be deleted.</span></span>
<span data-ttu-id="ad0e1-105">**InheritedFrom** 属性必须为 `null`。</span><span class="sxs-lookup"><span data-stu-id="ad0e1-105">The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad0e1-106">权限</span><span class="sxs-lookup"><span data-stu-id="ad0e1-106">Permissions</span></span>

<span data-ttu-id="ad0e1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad0e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad0e1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad0e1-109">Permission type</span></span>      | <span data-ttu-id="ad0e1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad0e1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad0e1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad0e1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ad0e1-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad0e1-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad0e1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad0e1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad0e1-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad0e1-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad0e1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad0e1-115">Application</span></span> | <span data-ttu-id="ad0e1-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad0e1-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad0e1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad0e1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="ad0e1-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="ad0e1-118">Optional request headers</span></span>

| <span data-ttu-id="ad0e1-119">名称</span><span class="sxs-lookup"><span data-stu-id="ad0e1-119">Name</span></span>          | <span data-ttu-id="ad0e1-120">类型</span><span class="sxs-lookup"><span data-stu-id="ad0e1-120">Type</span></span>   | <span data-ttu-id="ad0e1-121">说明</span><span class="sxs-lookup"><span data-stu-id="ad0e1-121">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ad0e1-122">if-match</span><span class="sxs-lookup"><span data-stu-id="ad0e1-122">if-match</span></span>      | <span data-ttu-id="ad0e1-123">string</span><span class="sxs-lookup"><span data-stu-id="ad0e1-123">string</span></span> | <span data-ttu-id="ad0e1-124">如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="ad0e1-124">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="ad0e1-125">响应</span><span class="sxs-lookup"><span data-stu-id="ad0e1-125">Response</span></span>

<span data-ttu-id="ad0e1-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ad0e1-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ad0e1-127">示例</span><span class="sxs-lookup"><span data-stu-id="ad0e1-127">Example</span></span>

<span data-ttu-id="ad0e1-128">本示例从当前用户 OneDrive 的项 {item-id} 中删除标识为 {perm-id} 的权限。</span><span class="sxs-lookup"><span data-stu-id="ad0e1-128">This example removes the permission identified as {perm-id} from the item {item-id} in the current user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "delete-permission", "scopes": "files.readwrite", "tags": "service.graph" }-->

```http
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
```

### <a name="response"></a><span data-ttu-id="ad0e1-129">响应</span><span class="sxs-lookup"><span data-stu-id="ad0e1-129">Response</span></span>

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="ad0e1-130">注解</span><span class="sxs-lookup"><span data-stu-id="ad0e1-130">Remarks</span></span>

* <span data-ttu-id="ad0e1-131">具有 `personal`（OneDrive 个人版）**driveType** 的 [驱动器](../resources/drive.md) 无法创建或修改根 DriveItem 上的权限。</span><span class="sxs-lookup"><span data-stu-id="ad0e1-131">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove an item's sharing permissions",
  "keywords": "permission, permissions, sharing, remove permissions, delete permissions",
  "section": "documentation",
  "tocPath": "Sharing/Remove permissions"
} -->
