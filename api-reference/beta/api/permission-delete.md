---
author: JeremyKelley
description: 删除 DriveItem 访问权限。
ms.date: 09/10/2017
title: 删除对项目的访问权限
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 82092233f6f7a01416ecd6f43d72b5737be45510
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775505"
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a><span data-ttu-id="f16e9-103">从文件或文件夹中删除共享权限</span><span class="sxs-lookup"><span data-stu-id="f16e9-103">Delete a sharing permission from a file or folder</span></span>

<span data-ttu-id="f16e9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f16e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f16e9-105">删除 [DriveItem](../resources/driveitem.md) 访问权限。</span><span class="sxs-lookup"><span data-stu-id="f16e9-105">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="f16e9-106">只能删除 **非** 继承的共享权限。</span><span class="sxs-lookup"><span data-stu-id="f16e9-106">Only sharing permissions that are **not** inherited can be deleted.</span></span>
<span data-ttu-id="f16e9-107">**InheritedFrom** 属性必须为 `null`。</span><span class="sxs-lookup"><span data-stu-id="f16e9-107">The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="f16e9-108">权限</span><span class="sxs-lookup"><span data-stu-id="f16e9-108">Permissions</span></span>
<span data-ttu-id="f16e9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f16e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f16e9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f16e9-111">Permission type</span></span>      | <span data-ttu-id="f16e9-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f16e9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f16e9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f16e9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f16e9-114">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f16e9-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f16e9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f16e9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f16e9-116">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f16e9-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f16e9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f16e9-117">Application</span></span> | <span data-ttu-id="f16e9-118">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f16e9-118">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f16e9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f16e9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="f16e9-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="f16e9-120">Optional request headers</span></span>

| <span data-ttu-id="f16e9-121">名称</span><span class="sxs-lookup"><span data-stu-id="f16e9-121">Name</span></span>          | <span data-ttu-id="f16e9-122">类型</span><span class="sxs-lookup"><span data-stu-id="f16e9-122">Type</span></span>   | <span data-ttu-id="f16e9-123">说明</span><span class="sxs-lookup"><span data-stu-id="f16e9-123">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f16e9-124">if-match</span><span class="sxs-lookup"><span data-stu-id="f16e9-124">if-match</span></span>      | <span data-ttu-id="f16e9-125">string</span><span class="sxs-lookup"><span data-stu-id="f16e9-125">string</span></span> | <span data-ttu-id="f16e9-126">如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="f16e9-126">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |


## <a name="response"></a><span data-ttu-id="f16e9-127">响应</span><span class="sxs-lookup"><span data-stu-id="f16e9-127">Response</span></span>

<span data-ttu-id="f16e9-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f16e9-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f16e9-129">示例</span><span class="sxs-lookup"><span data-stu-id="f16e9-129">Example</span></span>

<span data-ttu-id="f16e9-130">本示例从当前用户 OneDrive 的项 {item-id} 中删除标识为 {perm-id} 的权限。</span><span class="sxs-lookup"><span data-stu-id="f16e9-130">This example removes the permission identified as {perm-id} from the item {item-id} in the current user's OneDrive.</span></span>



# <a name="http"></a>[<span data-ttu-id="f16e9-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f16e9-131">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-permission", "scopes": "files.readwrite" }-->
```http
DELETE https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
```
# <a name="c"></a>[<span data-ttu-id="f16e9-132">C#</span><span class="sxs-lookup"><span data-stu-id="f16e9-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f16e9-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f16e9-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f16e9-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f16e9-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f16e9-135">Java</span><span class="sxs-lookup"><span data-stu-id="f16e9-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f16e9-136">响应</span><span class="sxs-lookup"><span data-stu-id="f16e9-136">Response</span></span>

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="f16e9-137">注解</span><span class="sxs-lookup"><span data-stu-id="f16e9-137">Remarks</span></span>

* <span data-ttu-id="f16e9-138">具有 `personal`（OneDrive 个人版）**driveType** 的 [驱动器](../resources/drive.md) 无法创建或修改根 DriveItem 上的权限。</span><span class="sxs-lookup"><span data-stu-id="f16e9-138">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove an item's sharing permissions",
  "keywords": "permission, permissions, sharing, remove permissions, delete permissions",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete permission",
  "suppressions": [
  ]
}
-->


