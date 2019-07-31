---
title: 永久删除项目
description: 永久删除已删除的项目中的项目
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 30c5cb4bc5257e4d98cbf2ee19ecfb8542a3d82e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35951288"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="cdc8d-103">永久删除项目</span><span class="sxs-lookup"><span data-stu-id="cdc8d-103">Permanently delete item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdc8d-104">永久删除[已删除的项目](../resources/directory.md)中的项目</span><span class="sxs-lookup"><span data-stu-id="cdc8d-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="cdc8d-105">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="cdc8d-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="cdc8d-106">可以永久删除“已删除的项目”中的项目。</span><span class="sxs-lookup"><span data-stu-id="cdc8d-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="cdc8d-107">但当某个项目永久删除后，将**无法**还原。</span><span class="sxs-lookup"><span data-stu-id="cdc8d-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdc8d-108">权限</span><span class="sxs-lookup"><span data-stu-id="cdc8d-108">Permissions</span></span>
<span data-ttu-id="cdc8d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cdc8d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="cdc8d-111">对于用户: Directory.accessasuser.all 的所有用户。</span><span class="sxs-lookup"><span data-stu-id="cdc8d-111">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="cdc8d-112">对于组: Directory.accessasuser.all 和 all 的组</span><span class="sxs-lookup"><span data-stu-id="cdc8d-112">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="cdc8d-113">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cdc8d-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cdc8d-114">请求标头</span><span class="sxs-lookup"><span data-stu-id="cdc8d-114">Request headers</span></span>
| <span data-ttu-id="cdc8d-115">名称</span><span class="sxs-lookup"><span data-stu-id="cdc8d-115">Name</span></span>       | <span data-ttu-id="cdc8d-116">说明</span><span class="sxs-lookup"><span data-stu-id="cdc8d-116">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cdc8d-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdc8d-117">Authorization</span></span>  | <span data-ttu-id="cdc8d-118">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="cdc8d-118">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="cdc8d-119">接受</span><span class="sxs-lookup"><span data-stu-id="cdc8d-119">Accept</span></span>  | <span data-ttu-id="cdc8d-120">application/json</span><span class="sxs-lookup"><span data-stu-id="cdc8d-120">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cdc8d-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="cdc8d-121">Request body</span></span>
<span data-ttu-id="cdc8d-122">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cdc8d-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdc8d-123">响应</span><span class="sxs-lookup"><span data-stu-id="cdc8d-123">Response</span></span>

<span data-ttu-id="cdc8d-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cdc8d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdc8d-126">示例</span><span class="sxs-lookup"><span data-stu-id="cdc8d-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cdc8d-127">请求</span><span class="sxs-lookup"><span data-stu-id="cdc8d-127">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cdc8d-128">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="cdc8d-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cdc8d-129">C#</span><span class="sxs-lookup"><span data-stu-id="cdc8d-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cdc8d-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="cdc8d-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cdc8d-131">目标-C</span><span class="sxs-lookup"><span data-stu-id="cdc8d-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cdc8d-132">Java</span><span class="sxs-lookup"><span data-stu-id="cdc8d-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cdc8d-133">响应</span><span class="sxs-lookup"><span data-stu-id="cdc8d-133">Response</span></span>
<span data-ttu-id="cdc8d-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cdc8d-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
