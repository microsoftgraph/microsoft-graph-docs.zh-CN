---
author: JeremyKelley
description: 将 ListItem 的以前版本还原为当前版本。 这将使用以前版本的内容创建一个新版本，但保留项的所有现有版本。
ms.date: 09/10/2017
title: 还原 SharePoint 列表项的以前版本
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 22e00628b10e268ef8eada5be6cb195ca62cc454
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993016"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="3f89d-104">还原 ListItem 的以前版本</span><span class="sxs-lookup"><span data-stu-id="3f89d-104">Restore a previous version of a ListItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f89d-105">将 ListItem 的以前版本还原为当前版本。</span><span class="sxs-lookup"><span data-stu-id="3f89d-105">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="3f89d-106">这将使用以前版本的内容创建一个新版本，但保留项的所有现有版本。</span><span class="sxs-lookup"><span data-stu-id="3f89d-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f89d-107">权限</span><span class="sxs-lookup"><span data-stu-id="3f89d-107">Permissions</span></span>

<span data-ttu-id="3f89d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3f89d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="3f89d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f89d-110">Permission type</span></span>             |         <span data-ttu-id="3f89d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3f89d-111">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="3f89d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f89d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3f89d-113">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="3f89d-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="3f89d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f89d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f89d-115">无</span><span class="sxs-lookup"><span data-stu-id="3f89d-115">n/a</span></span>                                                          |
| <span data-ttu-id="3f89d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3f89d-116">Application</span></span>                            | <span data-ttu-id="3f89d-117">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="3f89d-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f89d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f89d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="3f89d-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f89d-119">Request body</span></span>

<span data-ttu-id="3f89d-120">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="3f89d-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="3f89d-121">示例</span><span class="sxs-lookup"><span data-stu-id="3f89d-121">Example</span></span>

<span data-ttu-id="3f89d-122">本示例还原由 `{item-id}` 和 `{version-id}` 标识的 listItem 的一个版本。</span><span class="sxs-lookup"><span data-stu-id="3f89d-122">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="3f89d-123">响应</span><span class="sxs-lookup"><span data-stu-id="3f89d-123">Response</span></span>

<span data-ttu-id="3f89d-124">如果成功，该 API 调用会返回 `204 No content`。</span><span class="sxs-lookup"><span data-stu-id="3f89d-124">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": []
}
-->
