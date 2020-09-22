---
author: chackman
description: 列出已登录用户的后续项目。
title: 列出关注的项
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8fcba872a289b7985a013a0cbca06a0740977dbf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982225"
---
# <a name="list-followed-items"></a><span data-ttu-id="44fe6-103">列出关注的项</span><span class="sxs-lookup"><span data-stu-id="44fe6-103">List followed items</span></span>

<span data-ttu-id="44fe6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44fe6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44fe6-105">列出已登录用户的后续 [项目](../resources/driveitem.md) 。</span><span class="sxs-lookup"><span data-stu-id="44fe6-105">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="44fe6-106">此集合包含用户驱动器中的项目，以及他们有从其他驱动器进行访问的权限的项目。</span><span class="sxs-lookup"><span data-stu-id="44fe6-106">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="44fe6-107">权限</span><span class="sxs-lookup"><span data-stu-id="44fe6-107">Permissions</span></span>

<span data-ttu-id="44fe6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44fe6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44fe6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="44fe6-110">Permission type</span></span>      | <span data-ttu-id="44fe6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="44fe6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44fe6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44fe6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="44fe6-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44fe6-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="44fe6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44fe6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44fe6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="44fe6-115">Not supported.</span></span>    |
|<span data-ttu-id="44fe6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="44fe6-116">Application</span></span> | <span data-ttu-id="44fe6-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44fe6-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44fe6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44fe6-118">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="44fe6-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="44fe6-119">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/following
```
# <a name="c"></a>[<span data-ttu-id="44fe6-120">C#</span><span class="sxs-lookup"><span data-stu-id="44fe6-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-followed-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44fe6-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44fe6-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-followed-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44fe6-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44fe6-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-followed-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="44fe6-123">响应</span><span class="sxs-lookup"><span data-stu-id="44fe6-123">Response</span></span>

<span data-ttu-id="44fe6-124">此方法返回驱动器所有者正在关注的项目的 [driveItem](../resources/driveitem.md) 资源的集合。</span><span class="sxs-lookup"><span data-stu-id="44fe6-124">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="44fe6-125">如果未找到任何项目，则返回一个空集合。</span><span class="sxs-lookup"><span data-stu-id="44fe6-125">If no items were found, an empty collection is returned.</span></span>

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
  ]
}
-->


