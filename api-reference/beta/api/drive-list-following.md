---
author: chackman
ms.author: chackman
title: 列出关注的项
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: df38a11a09f4ec86eb029f236030cc4565e5d939
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454804"
---
# <a name="list-followed-items"></a><span data-ttu-id="62514-102">列出关注的项</span><span class="sxs-lookup"><span data-stu-id="62514-102">List followed items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62514-103">列出已登录用户的后续[项目](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="62514-103">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="62514-104">此集合包含用户驱动器中的项目，以及他们有从其他驱动器进行访问的权限的项目。</span><span class="sxs-lookup"><span data-stu-id="62514-104">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="62514-105">权限</span><span class="sxs-lookup"><span data-stu-id="62514-105">Permissions</span></span>

<span data-ttu-id="62514-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62514-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62514-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="62514-108">Permission type</span></span>      | <span data-ttu-id="62514-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62514-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62514-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62514-110">Delegated (work or school account)</span></span> | <span data-ttu-id="62514-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62514-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="62514-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62514-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62514-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="62514-113">Not supported.</span></span>    |
|<span data-ttu-id="62514-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="62514-114">Application</span></span> | <span data-ttu-id="62514-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62514-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62514-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62514-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```

## <a name="response"></a><span data-ttu-id="62514-117">响应</span><span class="sxs-lookup"><span data-stu-id="62514-117">Response</span></span>

<span data-ttu-id="62514-118">此方法返回驱动器所有者正在关注的项目的[driveItem](../resources/driveitem.md)资源的集合。</span><span class="sxs-lookup"><span data-stu-id="62514-118">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="62514-119">如果未找到任何项目，则返回一个空集合。</span><span class="sxs-lookup"><span data-stu-id="62514-119">If no items were found, an empty collection is returned.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "name": "March Proposal.docx",
      "size": 19121,
      "lastModifiedDateTime": "2017-12-12T10:40:59Z"
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "size": 37810,
      "lastModifiedDateTime": "2016-10-18T10:40:59Z"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "List the items a user is following.",
  "keywords": "drive,onedrive.drive,list followed items",
  "section": "documentation",
  "tocPath": "Drives/List followed items",
  "suppressions": [
    "Error: /api-reference/beta/api/drive-list-following.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
