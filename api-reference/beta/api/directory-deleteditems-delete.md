---
title: 永久删除项目
description: 从已删除的项目中永久删除项目。
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2ef89074d46dc81eb8cf0ad7e9b9b6eb5ccb4895
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44287785"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="b9c79-103">永久删除项目</span><span class="sxs-lookup"><span data-stu-id="b9c79-103">Permanently delete item</span></span>

<span data-ttu-id="b9c79-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9c79-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9c79-105">从[已删除的项目](../resources/directory.md)中永久删除项目。</span><span class="sxs-lookup"><span data-stu-id="b9c79-105">Permanently delete an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="b9c79-106">目前，仅支持[应用程序](../resources/application.md)、[组](../resources/group.md)和[用户](../resources/user.md)资源的 "已删除邮件" 功能。</span><span class="sxs-lookup"><span data-stu-id="b9c79-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="b9c79-107">可以永久删除“已删除的项目”中的项目。</span><span class="sxs-lookup"><span data-stu-id="b9c79-107">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="b9c79-108">但当某个项目永久删除后，将**无法**还原。</span><span class="sxs-lookup"><span data-stu-id="b9c79-108">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9c79-109">权限</span><span class="sxs-lookup"><span data-stu-id="b9c79-109">Permissions</span></span>
<span data-ttu-id="b9c79-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9c79-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b9c79-112">对于应用程序：</span><span class="sxs-lookup"><span data-stu-id="b9c79-112">For applications:</span></span>

|<span data-ttu-id="b9c79-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9c79-113">Permission type</span></span>      | <span data-ttu-id="b9c79-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9c79-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9c79-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9c79-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b9c79-116">所有的 Directory.accessasuser.all，all，all，All</span><span class="sxs-lookup"><span data-stu-id="b9c79-116">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b9c79-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9c79-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9c79-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9c79-118">Not supported.</span></span>    |
|<span data-ttu-id="b9c79-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9c79-119">Application</span></span> | <span data-ttu-id="b9c79-120">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9c79-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

<span data-ttu-id="b9c79-121">对于用户：</span><span class="sxs-lookup"><span data-stu-id="b9c79-121">For users:</span></span>

|<span data-ttu-id="b9c79-122">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9c79-122">Permission type</span></span>      | <span data-ttu-id="b9c79-123">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9c79-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9c79-124">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9c79-124">Delegated (work or school account)</span></span> | <span data-ttu-id="b9c79-125">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b9c79-125">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="b9c79-126">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9c79-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9c79-127">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9c79-127">Not supported.</span></span> |
|<span data-ttu-id="b9c79-128">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9c79-128">Application</span></span> | <span data-ttu-id="b9c79-129">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9c79-129">User.ReadWrite.All</span></span> |

<span data-ttu-id="b9c79-130">对于组：</span><span class="sxs-lookup"><span data-stu-id="b9c79-130">For groups:</span></span>

|<span data-ttu-id="b9c79-131">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9c79-131">Permission type</span></span>      | <span data-ttu-id="b9c79-132">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9c79-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9c79-133">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9c79-133">Delegated (work or school account)</span></span> | <span data-ttu-id="b9c79-134">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b9c79-134">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="b9c79-135">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9c79-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9c79-136">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9c79-136">Not supported.</span></span>    |
|<span data-ttu-id="b9c79-137">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9c79-137">Application</span></span> | <span data-ttu-id="b9c79-138">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9c79-138">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9c79-139">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9c79-139">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b9c79-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9c79-140">Request headers</span></span>
| <span data-ttu-id="b9c79-141">名称</span><span class="sxs-lookup"><span data-stu-id="b9c79-141">Name</span></span>       | <span data-ttu-id="b9c79-142">说明</span><span class="sxs-lookup"><span data-stu-id="b9c79-142">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b9c79-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9c79-143">Authorization</span></span>  | <span data-ttu-id="b9c79-144">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="b9c79-144">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="b9c79-145">接受</span><span class="sxs-lookup"><span data-stu-id="b9c79-145">Accept</span></span>  | <span data-ttu-id="b9c79-146">application/json</span><span class="sxs-lookup"><span data-stu-id="b9c79-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9c79-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9c79-147">Request body</span></span>
<span data-ttu-id="b9c79-148">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b9c79-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9c79-149">响应</span><span class="sxs-lookup"><span data-stu-id="b9c79-149">Response</span></span>

<span data-ttu-id="b9c79-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b9c79-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9c79-152">示例</span><span class="sxs-lookup"><span data-stu-id="b9c79-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9c79-153">请求</span><span class="sxs-lookup"><span data-stu-id="b9c79-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b9c79-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9c79-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
# <a name="c"></a>[<span data-ttu-id="b9c79-155">C#</span><span class="sxs-lookup"><span data-stu-id="b9c79-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9c79-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9c79-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9c79-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9c79-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b9c79-158">响应</span><span class="sxs-lookup"><span data-stu-id="b9c79-158">Response</span></span>
<span data-ttu-id="b9c79-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b9c79-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
