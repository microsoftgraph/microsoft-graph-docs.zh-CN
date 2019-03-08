---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 还原 SharePoint 列表项的以前版本
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 20cf0460aa679fc40a4bb11d0887bc4946ddcd74
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482082"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="fa4eb-102">还原 ListItem 的以前版本</span><span class="sxs-lookup"><span data-stu-id="fa4eb-102">Restore a previous version of a ListItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa4eb-103">将 ListItem 的以前版本还原为当前版本。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-103">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="fa4eb-104">这将使用以前版本的内容创建一个新版本，但保留项的所有现有版本。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-104">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa4eb-105">权限</span><span class="sxs-lookup"><span data-stu-id="fa4eb-105">Permissions</span></span>

<span data-ttu-id="fa4eb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="fa4eb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa4eb-108">Permission type</span></span>             |         <span data-ttu-id="fa4eb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa4eb-109">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="fa4eb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa4eb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa4eb-111">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="fa4eb-111">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="fa4eb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa4eb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa4eb-113">无</span><span class="sxs-lookup"><span data-stu-id="fa4eb-113">n/a</span></span>                                                          |
| <span data-ttu-id="fa4eb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa4eb-114">Application</span></span>                            | <span data-ttu-id="fa4eb-115">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="fa4eb-115">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa4eb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa4eb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="fa4eb-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa4eb-117">Request body</span></span>

<span data-ttu-id="fa4eb-118">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="fa4eb-119">示例</span><span class="sxs-lookup"><span data-stu-id="fa4eb-119">Example</span></span>

<span data-ttu-id="fa4eb-120">本示例还原由 `{item-id}` 和 `{version-id}` 标识的 listItem 的一个版本。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-120">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="fa4eb-121">响应</span><span class="sxs-lookup"><span data-stu-id="fa4eb-121">Response</span></span>

<span data-ttu-id="fa4eb-122">如果成功，该 API 调用会返回 `204 No content`。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-122">If successful, the API call returns a `204 No content`.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/listitemversion-restore.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
