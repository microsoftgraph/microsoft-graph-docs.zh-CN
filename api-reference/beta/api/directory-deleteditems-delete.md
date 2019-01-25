---
title: 永久删除项目
description: 永久删除已删除的项目中的项目
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 048008e31bc5cd7884dd3d7e9259412070404d9d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528198"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="edd79-103">永久删除项目</span><span class="sxs-lookup"><span data-stu-id="edd79-103">Permanently delete item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edd79-104">永久删除[已删除的项目](../resources/directory.md)中的项目</span><span class="sxs-lookup"><span data-stu-id="edd79-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="edd79-105">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="edd79-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="edd79-106">可以永久删除“已删除的项目”中的项目。</span><span class="sxs-lookup"><span data-stu-id="edd79-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="edd79-107">但当某个项目永久删除后，将**无法**还原。</span><span class="sxs-lookup"><span data-stu-id="edd79-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="edd79-108">权限</span><span class="sxs-lookup"><span data-stu-id="edd79-108">Permissions</span></span>
<span data-ttu-id="edd79-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="edd79-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="edd79-111">用户： User.ReadWrite.All、 Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="edd79-111">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="edd79-112">组： Group.ReadWrite.All、 Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="edd79-112">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="edd79-113">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="edd79-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="edd79-114">请求标头</span><span class="sxs-lookup"><span data-stu-id="edd79-114">Request headers</span></span>
| <span data-ttu-id="edd79-115">名称</span><span class="sxs-lookup"><span data-stu-id="edd79-115">Name</span></span>       | <span data-ttu-id="edd79-116">说明</span><span class="sxs-lookup"><span data-stu-id="edd79-116">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="edd79-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="edd79-117">Authorization</span></span>  | <span data-ttu-id="edd79-118">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="edd79-118">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="edd79-119">Accept</span><span class="sxs-lookup"><span data-stu-id="edd79-119">Accept</span></span>  | <span data-ttu-id="edd79-120">application/json</span><span class="sxs-lookup"><span data-stu-id="edd79-120">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="edd79-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="edd79-121">Request body</span></span>
<span data-ttu-id="edd79-122">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="edd79-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="edd79-123">响应</span><span class="sxs-lookup"><span data-stu-id="edd79-123">Response</span></span>

<span data-ttu-id="edd79-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="edd79-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edd79-126">示例</span><span class="sxs-lookup"><span data-stu-id="edd79-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="edd79-127">请求</span><span class="sxs-lookup"><span data-stu-id="edd79-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="edd79-128">响应</span><span class="sxs-lookup"><span data-stu-id="edd79-128">Response</span></span>
<span data-ttu-id="edd79-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="edd79-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/directory-deleteditems-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
