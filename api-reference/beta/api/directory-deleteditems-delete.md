---
title: 永久删除项目
description: 从已删除的项目中永久删除项目。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7eb499efa6aca193ddcf4d641798c37f11c2d14b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937096"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="30e7d-103">永久删除项目</span><span class="sxs-lookup"><span data-stu-id="30e7d-103">Permanently delete item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30e7d-104">从[已删除的项目](../resources/directory.md)中永久删除项目。</span><span class="sxs-lookup"><span data-stu-id="30e7d-104">Permanently delete an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="30e7d-105">目前，仅支持[应用程序](../resources/application.md)、[组](../resources/group.md)和[用户](../resources/user.md)资源的 "已删除邮件" 功能。</span><span class="sxs-lookup"><span data-stu-id="30e7d-105">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="30e7d-106">可以永久删除“已删除的项目”中的项目。</span><span class="sxs-lookup"><span data-stu-id="30e7d-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="30e7d-107">但当某个项目永久删除后，将**无法**还原。</span><span class="sxs-lookup"><span data-stu-id="30e7d-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="30e7d-108">权限</span><span class="sxs-lookup"><span data-stu-id="30e7d-108">Permissions</span></span>
<span data-ttu-id="30e7d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="30e7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="30e7d-111">对于应用程序：</span><span class="sxs-lookup"><span data-stu-id="30e7d-111">For applications:</span></span>

|<span data-ttu-id="30e7d-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="30e7d-112">Permission type</span></span>      | <span data-ttu-id="30e7d-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="30e7d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30e7d-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30e7d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="30e7d-115">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="30e7d-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="30e7d-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30e7d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30e7d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="30e7d-117">Not supported.</span></span>    |
|<span data-ttu-id="30e7d-118">Application</span><span class="sxs-lookup"><span data-stu-id="30e7d-118">Application</span></span> | <span data-ttu-id="30e7d-119">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="30e7d-119">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

<span data-ttu-id="30e7d-120">对于用户：</span><span class="sxs-lookup"><span data-stu-id="30e7d-120">For users:</span></span>

|<span data-ttu-id="30e7d-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="30e7d-121">Permission type</span></span>      | <span data-ttu-id="30e7d-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="30e7d-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30e7d-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30e7d-123">Delegated (work or school account)</span></span> | <span data-ttu-id="30e7d-124">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="30e7d-124">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="30e7d-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30e7d-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30e7d-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="30e7d-126">Not supported.</span></span> |
|<span data-ttu-id="30e7d-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="30e7d-127">Application</span></span> | <span data-ttu-id="30e7d-128">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30e7d-128">User.ReadWrite.All</span></span> |

<span data-ttu-id="30e7d-129">对于组：</span><span class="sxs-lookup"><span data-stu-id="30e7d-129">For groups:</span></span>

|<span data-ttu-id="30e7d-130">权限类型</span><span class="sxs-lookup"><span data-stu-id="30e7d-130">Permission type</span></span>      | <span data-ttu-id="30e7d-131">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="30e7d-131">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30e7d-132">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30e7d-132">Delegated (work or school account)</span></span> | <span data-ttu-id="30e7d-133">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="30e7d-133">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="30e7d-134">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30e7d-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30e7d-135">不支持。</span><span class="sxs-lookup"><span data-stu-id="30e7d-135">Not supported.</span></span>    |
|<span data-ttu-id="30e7d-136">Application</span><span class="sxs-lookup"><span data-stu-id="30e7d-136">Application</span></span> | <span data-ttu-id="30e7d-137">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30e7d-137">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="30e7d-138">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30e7d-138">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="30e7d-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="30e7d-139">Request headers</span></span>
| <span data-ttu-id="30e7d-140">名称</span><span class="sxs-lookup"><span data-stu-id="30e7d-140">Name</span></span>       | <span data-ttu-id="30e7d-141">说明</span><span class="sxs-lookup"><span data-stu-id="30e7d-141">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="30e7d-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="30e7d-142">Authorization</span></span>  | <span data-ttu-id="30e7d-143">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="30e7d-143">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="30e7d-144">接受</span><span class="sxs-lookup"><span data-stu-id="30e7d-144">Accept</span></span>  | <span data-ttu-id="30e7d-145">application/json</span><span class="sxs-lookup"><span data-stu-id="30e7d-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="30e7d-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="30e7d-146">Request body</span></span>
<span data-ttu-id="30e7d-147">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="30e7d-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30e7d-148">响应</span><span class="sxs-lookup"><span data-stu-id="30e7d-148">Response</span></span>

<span data-ttu-id="30e7d-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="30e7d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30e7d-151">示例</span><span class="sxs-lookup"><span data-stu-id="30e7d-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30e7d-152">请求</span><span class="sxs-lookup"><span data-stu-id="30e7d-152">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="30e7d-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="30e7d-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="30e7d-154">C#</span><span class="sxs-lookup"><span data-stu-id="30e7d-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="30e7d-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30e7d-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="30e7d-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30e7d-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="30e7d-157">响应</span><span class="sxs-lookup"><span data-stu-id="30e7d-157">Response</span></span>
<span data-ttu-id="30e7d-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="30e7d-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
