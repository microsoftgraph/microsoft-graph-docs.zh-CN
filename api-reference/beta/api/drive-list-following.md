---
author: chackman
description: 列出已登录用户的后续项目。
title: 列出关注的项
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: c8fface18f7b783d463f4df57f97c610a45103ab
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321185"
---
# <a name="list-followed-items"></a><span data-ttu-id="39218-103">列出关注的项</span><span class="sxs-lookup"><span data-stu-id="39218-103">List followed items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39218-104">列出已登录用户的后续[项目](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="39218-104">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="39218-105">此集合包含用户驱动器中的项目，以及他们有从其他驱动器进行访问的权限的项目。</span><span class="sxs-lookup"><span data-stu-id="39218-105">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="39218-106">权限</span><span class="sxs-lookup"><span data-stu-id="39218-106">Permissions</span></span>

<span data-ttu-id="39218-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="39218-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39218-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="39218-109">Permission type</span></span>      | <span data-ttu-id="39218-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="39218-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39218-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39218-111">Delegated (work or school account)</span></span> | <span data-ttu-id="39218-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39218-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="39218-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39218-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39218-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="39218-114">Not supported.</span></span>    |
|<span data-ttu-id="39218-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="39218-115">Application</span></span> | <span data-ttu-id="39218-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39218-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="39218-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39218-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="39218-118">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="39218-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="39218-119">C#</span><span class="sxs-lookup"><span data-stu-id="39218-119">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-followed-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="39218-120">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39218-120">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-followed-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="39218-121">目标-C</span><span class="sxs-lookup"><span data-stu-id="39218-121">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-followed-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="39218-122">Java</span><span class="sxs-lookup"><span data-stu-id="39218-122">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-followed-items-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="39218-123">响应</span><span class="sxs-lookup"><span data-stu-id="39218-123">Response</span></span>

<span data-ttu-id="39218-124">此方法返回驱动器所有者正在关注的项目的[driveItem](../resources/driveitem.md)资源的集合。</span><span class="sxs-lookup"><span data-stu-id="39218-124">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="39218-125">如果未找到任何项目，则返回一个空集合。</span><span class="sxs-lookup"><span data-stu-id="39218-125">If no items were found, an empty collection is returned.</span></span>

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
