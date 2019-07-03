---
title: 永久删除项目
description: 永久删除已删除的项目中的项目
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7b65c4f2667e7acdb6a6ca5240df7ab68e66f594
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455992"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="fb30f-103">永久删除项目</span><span class="sxs-lookup"><span data-stu-id="fb30f-103">Permanently delete item</span></span>

<span data-ttu-id="fb30f-104">永久删除[已删除的项目](../resources/directory.md)中的项目</span><span class="sxs-lookup"><span data-stu-id="fb30f-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="fb30f-105">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="fb30f-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="fb30f-106">可以永久删除“已删除的项目”中的项目。</span><span class="sxs-lookup"><span data-stu-id="fb30f-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="fb30f-107">但当某个项目永久删除后，将**无法**还原。</span><span class="sxs-lookup"><span data-stu-id="fb30f-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb30f-108">权限</span><span class="sxs-lookup"><span data-stu-id="fb30f-108">Permissions</span></span>
<span data-ttu-id="fb30f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb30f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="fb30f-111">对于用户：</span><span class="sxs-lookup"><span data-stu-id="fb30f-111">For users:</span></span>

|<span data-ttu-id="fb30f-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb30f-112">Permission type</span></span>      | <span data-ttu-id="fb30f-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb30f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb30f-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb30f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="fb30f-115">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fb30f-115">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="fb30f-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb30f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb30f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb30f-117">Not supported.</span></span> |
|<span data-ttu-id="fb30f-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb30f-118">Application</span></span> | <span data-ttu-id="fb30f-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb30f-119">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="fb30f-120">对于组：</span><span class="sxs-lookup"><span data-stu-id="fb30f-120">For groups:</span></span>

|<span data-ttu-id="fb30f-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb30f-121">Permission type</span></span>      | <span data-ttu-id="fb30f-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb30f-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb30f-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb30f-123">Delegated (work or school account)</span></span> | <span data-ttu-id="fb30f-124">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fb30f-124">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="fb30f-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb30f-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb30f-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb30f-126">Not supported.</span></span>    |
|<span data-ttu-id="fb30f-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb30f-127">Application</span></span> | <span data-ttu-id="fb30f-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb30f-128">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb30f-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb30f-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deletedItems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fb30f-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb30f-130">Request headers</span></span>
| <span data-ttu-id="fb30f-131">名称</span><span class="sxs-lookup"><span data-stu-id="fb30f-131">Name</span></span>       | <span data-ttu-id="fb30f-132">说明</span><span class="sxs-lookup"><span data-stu-id="fb30f-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fb30f-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb30f-133">Authorization</span></span>  | <span data-ttu-id="fb30f-134">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="fb30f-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="fb30f-135">接受</span><span class="sxs-lookup"><span data-stu-id="fb30f-135">Accept</span></span>  | <span data-ttu-id="fb30f-136">application/json</span><span class="sxs-lookup"><span data-stu-id="fb30f-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb30f-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb30f-137">Request body</span></span>
<span data-ttu-id="fb30f-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fb30f-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb30f-139">响应</span><span class="sxs-lookup"><span data-stu-id="fb30f-139">Response</span></span>

<span data-ttu-id="fb30f-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fb30f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb30f-142">示例</span><span class="sxs-lookup"><span data-stu-id="fb30f-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb30f-143">请求</span><span class="sxs-lookup"><span data-stu-id="fb30f-143">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fb30f-144">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="fb30f-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fb30f-145">C#</span><span class="sxs-lookup"><span data-stu-id="fb30f-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fb30f-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="fb30f-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fb30f-147">目标-C</span><span class="sxs-lookup"><span data-stu-id="fb30f-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fb30f-148">响应</span><span class="sxs-lookup"><span data-stu-id="fb30f-148">Response</span></span>
<span data-ttu-id="fb30f-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fb30f-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
