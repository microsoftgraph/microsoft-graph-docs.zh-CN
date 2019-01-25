---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 还原以前版本
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7e430a3daf17ecf51500d258cc86a3dbbfcd108b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522453"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="b4d45-102">还原 DriveItem 的以前版本</span><span class="sxs-lookup"><span data-stu-id="b4d45-102">Restore a previous version of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4d45-103">将 DriveItem 的以前版本还原为当前版本。</span><span class="sxs-lookup"><span data-stu-id="b4d45-103">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="b4d45-104">这将使用以前版本的内容创建一个新版本，但保留该文件的所有现有版本。</span><span class="sxs-lookup"><span data-stu-id="b4d45-104">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4d45-105">权限</span><span class="sxs-lookup"><span data-stu-id="b4d45-105">Permissions</span></span>

<span data-ttu-id="b4d45-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4d45-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4d45-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4d45-108">Permission type</span></span>      | <span data-ttu-id="b4d45-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4d45-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4d45-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4d45-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b4d45-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4d45-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b4d45-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4d45-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4d45-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4d45-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b4d45-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4d45-114">Application</span></span> | <span data-ttu-id="b4d45-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4d45-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4d45-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4d45-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="b4d45-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4d45-117">Request body</span></span>

<span data-ttu-id="b4d45-118">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="b4d45-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="b4d45-119">示例</span><span class="sxs-lookup"><span data-stu-id="b4d45-119">Example</span></span>

<span data-ttu-id="b4d45-120">本示例还原由 `{item-id}` 和 `{version-id}` 标识的文件的一个版本。</span><span class="sxs-lookup"><span data-stu-id="b4d45-120">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="b4d45-121">响应</span><span class="sxs-lookup"><span data-stu-id="b4d45-121">Response</span></span>

<span data-ttu-id="b4d45-122">如果成功，该 API 调用会返回 `204 No content`。</span><span class="sxs-lookup"><span data-stu-id="b4d45-122">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitemversion-restore.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
