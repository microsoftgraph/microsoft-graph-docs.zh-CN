---
author: chackman
ms.author: chackman
title: 后面的列表项
localization_priority: Normal
ms.openlocfilehash: e8892bc96c53efef49f91d92b24b3ea97c937845
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849432"
---
# <a name="list-followed-items"></a><span data-ttu-id="cf58e-102">后面的列表项</span><span class="sxs-lookup"><span data-stu-id="cf58e-102">List followed items</span></span>

> <span data-ttu-id="cf58e-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cf58e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf58e-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cf58e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cf58e-105">列出跟登录用户的[项目](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="cf58e-105">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="cf58e-106">此集合包括用户的驱动器中的项目以及他们有权访问从其他驱动器的项目。</span><span class="sxs-lookup"><span data-stu-id="cf58e-106">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf58e-107">权限</span><span class="sxs-lookup"><span data-stu-id="cf58e-107">Permissions</span></span>

<span data-ttu-id="cf58e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf58e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf58e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf58e-110">Permission type</span></span>      | <span data-ttu-id="cf58e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf58e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf58e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf58e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cf58e-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf58e-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="cf58e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf58e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf58e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf58e-115">Not supported.</span></span>    |
|<span data-ttu-id="cf58e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf58e-116">Application</span></span> | <span data-ttu-id="cf58e-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf58e-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf58e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf58e-118">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```

## <a name="response"></a><span data-ttu-id="cf58e-119">响应</span><span class="sxs-lookup"><span data-stu-id="cf58e-119">Response</span></span>

<span data-ttu-id="cf58e-120">此方法返回的项目的驱动器的所有者正在关注的[driveItem](../resources/driveitem.md)资源的集合。</span><span class="sxs-lookup"><span data-stu-id="cf58e-120">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="cf58e-121">如果未不找到任何项目，则返回一个空集合。</span><span class="sxs-lookup"><span data-stu-id="cf58e-121">If no items were found, an empty collection is returned.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "List the items a user is following.",
  "keywords": "drive,onedrive.drive,list followed items",
  "section": "documentation",
  "tocPath": "Drives/List followed items"
} -->
