---
author: chackman
ms.author: chackman
title: 列出关注的项
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1892b6c9adac3c41cf99bf755aa8d67d51a0066e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589748"
---
# <a name="list-followed-items"></a><span data-ttu-id="04d68-102">列出关注的项</span><span class="sxs-lookup"><span data-stu-id="04d68-102">List followed items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04d68-103">列出已登录用户的后续[项目](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="04d68-103">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="04d68-104">此集合包含用户驱动器中的项目，以及他们有从其他驱动器进行访问的权限的项目。</span><span class="sxs-lookup"><span data-stu-id="04d68-104">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="04d68-105">权限</span><span class="sxs-lookup"><span data-stu-id="04d68-105">Permissions</span></span>

<span data-ttu-id="04d68-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="04d68-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04d68-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="04d68-108">Permission type</span></span>      | <span data-ttu-id="04d68-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="04d68-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04d68-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04d68-110">Delegated (work or school account)</span></span> | <span data-ttu-id="04d68-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04d68-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="04d68-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04d68-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04d68-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="04d68-113">Not supported.</span></span>    |
|<span data-ttu-id="04d68-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="04d68-114">Application</span></span> | <span data-ttu-id="04d68-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04d68-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04d68-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04d68-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```

## <a name="response"></a><span data-ttu-id="04d68-117">响应</span><span class="sxs-lookup"><span data-stu-id="04d68-117">Response</span></span>

<span data-ttu-id="04d68-118">此方法返回驱动器所有者正在关注的项目的[driveItem](../resources/driveitem.md)资源的集合。</span><span class="sxs-lookup"><span data-stu-id="04d68-118">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="04d68-119">如果未找到任何项目，则返回一个空集合。</span><span class="sxs-lookup"><span data-stu-id="04d68-119">If no items were found, an empty collection is returned.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="04d68-120">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="04d68-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="04d68-121">语言</span><span class="sxs-lookup"><span data-stu-id="04d68-121">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-followed-items-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="04d68-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="04d68-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-followed-items-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "List the items a user is following.",
  "keywords": "drive,onedrive.drive,list followed items",
  "section": "documentation",
  "tocPath": "Drives/List followed items",
  "suppressions": [
    "Error: /api-reference/beta/api/drive-list-following.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-list-following.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
