---
title: 从已删除项目永久删除项目
description: 永久删除已删除的项目中的项目
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 090f41ed4f6bc1410dccede72fe432e38320de0a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053207"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="79f20-103">永久删除项目</span><span class="sxs-lookup"><span data-stu-id="79f20-103">Permanently delete item</span></span>

<span data-ttu-id="79f20-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79f20-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="79f20-105">永久删除[已删除的项目](../resources/directory.md)中的项目</span><span class="sxs-lookup"><span data-stu-id="79f20-105">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="79f20-106">目前，仅应用程序、组和用户资源支持已删除的项目[](../resources/application.md)功能。 [](../resources/group.md) [](../resources/user.md)</span><span class="sxs-lookup"><span data-stu-id="79f20-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="79f20-107">可以永久删除“已删除的项目”中的项目。</span><span class="sxs-lookup"><span data-stu-id="79f20-107">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="79f20-108">但当某个项目永久删除后，将 **无法** 还原。</span><span class="sxs-lookup"><span data-stu-id="79f20-108">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="79f20-109">权限</span><span class="sxs-lookup"><span data-stu-id="79f20-109">Permissions</span></span>
<span data-ttu-id="79f20-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79f20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="79f20-112">对于应用程序：</span><span class="sxs-lookup"><span data-stu-id="79f20-112">For applications:</span></span>

|<span data-ttu-id="79f20-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="79f20-113">Permission type</span></span>      | <span data-ttu-id="79f20-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79f20-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79f20-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79f20-115">Delegated (work or school account)</span></span> | <span data-ttu-id="79f20-116">Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="79f20-116">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="79f20-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79f20-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79f20-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="79f20-118">Not supported.</span></span>    |
|<span data-ttu-id="79f20-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="79f20-119">Application</span></span> | <span data-ttu-id="79f20-120">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="79f20-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

<span data-ttu-id="79f20-121">请求程序需要具有以下角色之一：*全局管理员或\*\*应用程序管理员*。</span><span class="sxs-lookup"><span data-stu-id="79f20-121">The requestor needs to have one of the following roles: *Global Administrator* or *Application Administrator*.</span></span>

<span data-ttu-id="79f20-122">对于用户：</span><span class="sxs-lookup"><span data-stu-id="79f20-122">For users:</span></span>

|<span data-ttu-id="79f20-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="79f20-123">Permission type</span></span>      | <span data-ttu-id="79f20-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79f20-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79f20-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79f20-125">Delegated (work or school account)</span></span> | <span data-ttu-id="79f20-126">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="79f20-126">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="79f20-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79f20-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79f20-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="79f20-128">Not supported.</span></span> |
|<span data-ttu-id="79f20-129">应用程序</span><span class="sxs-lookup"><span data-stu-id="79f20-129">Application</span></span> | <span data-ttu-id="79f20-130">不支持。</span><span class="sxs-lookup"><span data-stu-id="79f20-130">Not supported.</span></span> |

<span data-ttu-id="79f20-131">登录用户需要具有以下角色之一：全局 *管理员* 或 *用户管理员*。</span><span class="sxs-lookup"><span data-stu-id="79f20-131">The signed-in user needs to have one of the following roles: *Global Administrator* or *User Administrator*.</span></span>

<span data-ttu-id="79f20-132">对于组：</span><span class="sxs-lookup"><span data-stu-id="79f20-132">For groups:</span></span>

|<span data-ttu-id="79f20-133">权限类型</span><span class="sxs-lookup"><span data-stu-id="79f20-133">Permission type</span></span>      | <span data-ttu-id="79f20-134">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79f20-134">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79f20-135">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79f20-135">Delegated (work or school account)</span></span> | <span data-ttu-id="79f20-136">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="79f20-136">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="79f20-137">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79f20-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79f20-138">不支持。</span><span class="sxs-lookup"><span data-stu-id="79f20-138">Not supported.</span></span>    |
|<span data-ttu-id="79f20-139">应用程序</span><span class="sxs-lookup"><span data-stu-id="79f20-139">Application</span></span> | <span data-ttu-id="79f20-140">不支持。</span><span class="sxs-lookup"><span data-stu-id="79f20-140">Not supported.</span></span> |

<span data-ttu-id="79f20-141">请求程序需要具有以下角色之一： *全局管理员* 或 *组管理员*。</span><span class="sxs-lookup"><span data-stu-id="79f20-141">The requestor needs to have one of the following roles: *Global Administrator* or *Groups Administrator*.</span></span>

## <a name="http-request"></a><span data-ttu-id="79f20-142">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79f20-142">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deletedItems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="79f20-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="79f20-143">Request headers</span></span>
| <span data-ttu-id="79f20-144">名称</span><span class="sxs-lookup"><span data-stu-id="79f20-144">Name</span></span>       | <span data-ttu-id="79f20-145">说明</span><span class="sxs-lookup"><span data-stu-id="79f20-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="79f20-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="79f20-146">Authorization</span></span>  | <span data-ttu-id="79f20-147">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="79f20-147">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="79f20-148">接受</span><span class="sxs-lookup"><span data-stu-id="79f20-148">Accept</span></span>  | <span data-ttu-id="79f20-149">application/json</span><span class="sxs-lookup"><span data-stu-id="79f20-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="79f20-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="79f20-150">Request body</span></span>
<span data-ttu-id="79f20-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="79f20-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79f20-152">响应</span><span class="sxs-lookup"><span data-stu-id="79f20-152">Response</span></span>

<span data-ttu-id="79f20-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="79f20-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79f20-155">示例</span><span class="sxs-lookup"><span data-stu-id="79f20-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79f20-156">请求</span><span class="sxs-lookup"><span data-stu-id="79f20-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="79f20-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="79f20-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="c"></a>[<span data-ttu-id="79f20-158">C#</span><span class="sxs-lookup"><span data-stu-id="79f20-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79f20-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79f20-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79f20-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79f20-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79f20-161">Java</span><span class="sxs-lookup"><span data-stu-id="79f20-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="79f20-162">响应</span><span class="sxs-lookup"><span data-stu-id="79f20-162">Response</span></span>
<span data-ttu-id="79f20-163">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="79f20-163">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

