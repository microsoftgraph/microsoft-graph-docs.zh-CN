---
title: 永久删除项目
description: 永久删除已删除的项目中的项目
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cb2738de749cf5b35188792c440d7189d788dc3a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260898"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="02d3c-103">永久删除项目</span><span class="sxs-lookup"><span data-stu-id="02d3c-103">Permanently delete item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02d3c-104">永久删除[已删除的项目](../resources/directory.md)中的项目</span><span class="sxs-lookup"><span data-stu-id="02d3c-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="02d3c-105">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="02d3c-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="02d3c-106">可以永久删除“已删除的项目”中的项目。</span><span class="sxs-lookup"><span data-stu-id="02d3c-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="02d3c-107">但当某个项目永久删除后，将**无法**还原。</span><span class="sxs-lookup"><span data-stu-id="02d3c-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="02d3c-108">权限</span><span class="sxs-lookup"><span data-stu-id="02d3c-108">Permissions</span></span>
<span data-ttu-id="02d3c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="02d3c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="02d3c-111">对于用户: Directory.accessasuser.all 的所有用户。</span><span class="sxs-lookup"><span data-stu-id="02d3c-111">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="02d3c-112">对于组: Directory.accessasuser.all 和 all 的组</span><span class="sxs-lookup"><span data-stu-id="02d3c-112">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="02d3c-113">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02d3c-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="02d3c-114">请求标头</span><span class="sxs-lookup"><span data-stu-id="02d3c-114">Request headers</span></span>
| <span data-ttu-id="02d3c-115">名称</span><span class="sxs-lookup"><span data-stu-id="02d3c-115">Name</span></span>       | <span data-ttu-id="02d3c-116">说明</span><span class="sxs-lookup"><span data-stu-id="02d3c-116">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="02d3c-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="02d3c-117">Authorization</span></span>  | <span data-ttu-id="02d3c-118">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="02d3c-118">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="02d3c-119">接受</span><span class="sxs-lookup"><span data-stu-id="02d3c-119">Accept</span></span>  | <span data-ttu-id="02d3c-120">application/json</span><span class="sxs-lookup"><span data-stu-id="02d3c-120">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="02d3c-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="02d3c-121">Request body</span></span>
<span data-ttu-id="02d3c-122">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="02d3c-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02d3c-123">响应</span><span class="sxs-lookup"><span data-stu-id="02d3c-123">Response</span></span>

<span data-ttu-id="02d3c-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="02d3c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02d3c-126">示例</span><span class="sxs-lookup"><span data-stu-id="02d3c-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02d3c-127">请求</span><span class="sxs-lookup"><span data-stu-id="02d3c-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="02d3c-128">响应</span><span class="sxs-lookup"><span data-stu-id="02d3c-128">Response</span></span>
<span data-ttu-id="02d3c-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="02d3c-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="02d3c-131">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="02d3c-131">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="02d3c-132">C#</span><span class="sxs-lookup"><span data-stu-id="02d3c-132">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_directory-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="02d3c-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="02d3c-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_directory-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="02d3c-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="02d3c-134">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_directory-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/directory-deleteditems-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directory-deleteditems-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directory-deleteditems-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
