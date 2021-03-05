---
title: 从已删除项目永久删除项目
description: 永久删除已删除的项目中的项目
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: fb34b77a381d22e22813539f0c186078077b3037
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442066"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="0da30-103">永久删除项目</span><span class="sxs-lookup"><span data-stu-id="0da30-103">Permanently delete item</span></span>

<span data-ttu-id="0da30-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0da30-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0da30-105">永久删除[已删除的项目](../resources/directory.md)中的项目</span><span class="sxs-lookup"><span data-stu-id="0da30-105">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="0da30-106">目前，仅应用程序、组和用户资源支持已删除的项目[](../resources/application.md)功能。 [](../resources/group.md) [](../resources/user.md)</span><span class="sxs-lookup"><span data-stu-id="0da30-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="0da30-107">可以永久删除“已删除的项目”中的项目。</span><span class="sxs-lookup"><span data-stu-id="0da30-107">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="0da30-108">但当某个项目永久删除后，将 **无法** 还原。</span><span class="sxs-lookup"><span data-stu-id="0da30-108">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="0da30-109">权限</span><span class="sxs-lookup"><span data-stu-id="0da30-109">Permissions</span></span>
<span data-ttu-id="0da30-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0da30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0da30-112">对于应用程序：</span><span class="sxs-lookup"><span data-stu-id="0da30-112">For applications:</span></span>

|<span data-ttu-id="0da30-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="0da30-113">Permission type</span></span>      | <span data-ttu-id="0da30-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0da30-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0da30-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0da30-115">Delegated (work or school account)</span></span> | <span data-ttu-id="0da30-116">Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0da30-116">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0da30-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0da30-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0da30-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0da30-118">Not supported.</span></span>    |
|<span data-ttu-id="0da30-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="0da30-119">Application</span></span> | <span data-ttu-id="0da30-120">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0da30-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

<span data-ttu-id="0da30-121">对于用户：</span><span class="sxs-lookup"><span data-stu-id="0da30-121">For users:</span></span>

|<span data-ttu-id="0da30-122">权限类型</span><span class="sxs-lookup"><span data-stu-id="0da30-122">Permission type</span></span>      | <span data-ttu-id="0da30-123">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0da30-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0da30-124">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0da30-124">Delegated (work or school account)</span></span> | <span data-ttu-id="0da30-125">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0da30-125">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="0da30-126">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0da30-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0da30-127">不支持。</span><span class="sxs-lookup"><span data-stu-id="0da30-127">Not supported.</span></span> |
|<span data-ttu-id="0da30-128">应用程序</span><span class="sxs-lookup"><span data-stu-id="0da30-128">Application</span></span> | <span data-ttu-id="0da30-129">不支持。</span><span class="sxs-lookup"><span data-stu-id="0da30-129">Not supported.</span></span> |

<span data-ttu-id="0da30-130">对于组：</span><span class="sxs-lookup"><span data-stu-id="0da30-130">For groups:</span></span>

|<span data-ttu-id="0da30-131">权限类型</span><span class="sxs-lookup"><span data-stu-id="0da30-131">Permission type</span></span>      | <span data-ttu-id="0da30-132">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0da30-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0da30-133">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0da30-133">Delegated (work or school account)</span></span> | <span data-ttu-id="0da30-134">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0da30-134">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="0da30-135">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0da30-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0da30-136">不支持。</span><span class="sxs-lookup"><span data-stu-id="0da30-136">Not supported.</span></span>    |
|<span data-ttu-id="0da30-137">应用程序</span><span class="sxs-lookup"><span data-stu-id="0da30-137">Application</span></span> | <span data-ttu-id="0da30-138">不支持。</span><span class="sxs-lookup"><span data-stu-id="0da30-138">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0da30-139">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0da30-139">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deletedItems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0da30-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="0da30-140">Request headers</span></span>
| <span data-ttu-id="0da30-141">名称</span><span class="sxs-lookup"><span data-stu-id="0da30-141">Name</span></span>       | <span data-ttu-id="0da30-142">说明</span><span class="sxs-lookup"><span data-stu-id="0da30-142">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0da30-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="0da30-143">Authorization</span></span>  | <span data-ttu-id="0da30-144">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="0da30-144">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="0da30-145">接受</span><span class="sxs-lookup"><span data-stu-id="0da30-145">Accept</span></span>  | <span data-ttu-id="0da30-146">application/json</span><span class="sxs-lookup"><span data-stu-id="0da30-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0da30-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="0da30-147">Request body</span></span>
<span data-ttu-id="0da30-148">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0da30-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0da30-149">响应</span><span class="sxs-lookup"><span data-stu-id="0da30-149">Response</span></span>

<span data-ttu-id="0da30-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0da30-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0da30-152">示例</span><span class="sxs-lookup"><span data-stu-id="0da30-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0da30-153">请求</span><span class="sxs-lookup"><span data-stu-id="0da30-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0da30-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="0da30-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="c"></a>[<span data-ttu-id="0da30-155">C#</span><span class="sxs-lookup"><span data-stu-id="0da30-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0da30-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0da30-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0da30-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0da30-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0da30-158">Java</span><span class="sxs-lookup"><span data-stu-id="0da30-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0da30-159">响应</span><span class="sxs-lookup"><span data-stu-id="0da30-159">Response</span></span>
<span data-ttu-id="0da30-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0da30-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

