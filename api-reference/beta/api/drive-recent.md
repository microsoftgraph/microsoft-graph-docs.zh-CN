---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 列出最近的文件
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c0462d98a26ab053ba47f1dda8b739dbd5f4806a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260310"
---
# <a name="list-recent-files"></a><span data-ttu-id="b0615-102">列出最近使用的文件</span><span class="sxs-lookup"><span data-stu-id="b0615-102">List recent files</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0615-p101">列出已登录用户最近使用的一组项目。此集合包含用户驱动器中的项目，以及他们有从其他驱动器进行访问的权限的项目。</span><span class="sxs-lookup"><span data-stu-id="b0615-p101">List a set of items that have been recently used by the signed in user. This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0615-105">权限</span><span class="sxs-lookup"><span data-stu-id="b0615-105">Permissions</span></span>

<span data-ttu-id="b0615-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0615-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0615-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0615-108">Permission type</span></span>      | <span data-ttu-id="b0615-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b0615-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0615-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0615-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b0615-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0615-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b0615-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0615-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0615-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0615-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b0615-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0615-114">Application</span></span> | <span data-ttu-id="b0615-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0615-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0615-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0615-116">HTTP request</span></span>

<!-- { "blockType": "request",
       "name": "view-recent-files", 
       "scopes": "files.read",
       "target": "action" } -->

```http
GET /me/drive/recent
```

## <a name="response"></a><span data-ttu-id="b0615-117">响应</span><span class="sxs-lookup"><span data-stu-id="b0615-117">Response</span></span>

<span data-ttu-id="b0615-118">此方法返回驱动器所有者最近访问的项的 [DriveItem](../resources/driveitem.md) 资源集合。</span><span class="sxs-lookup"><span data-stu-id="b0615-118">This method returns a collection of [DriveItem](../resources/driveitem.md) resources for items which the owner of the drive has recently accessed.</span></span>

<!-- { "blockType": "response",
       "@odata.type": "Collection(microsoft.graph.driveItem)",
       "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "remoteItem":
      {
        "id": "1991210caf!192",
        "name": "March Proposal.docx",
        "file": { },
        "size": 19121,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      },
      "fileSystemInfo": {
        "lastAccessedDateTime": "2017-02-20T19:13:00Z"
      }
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "file": { },
      "size": 37810,
      "parentReference": {
        "driveId": "1312def",
        "id": "1312def!123"
      },
      "fileSystemInfo": {
        "lastAccessedDateTime": "2017-02-20T16:43:21Z"
      }
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b0615-119">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="b0615-119">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b0615-120">C#</span><span class="sxs-lookup"><span data-stu-id="b0615-120">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/view-recent-files-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0615-121">Javascript</span><span class="sxs-lookup"><span data-stu-id="b0615-121">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/view-recent-files-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b0615-122">目标-C</span><span class="sxs-lookup"><span data-stu-id="b0615-122">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/view-recent-files-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="b0615-123">注解</span><span class="sxs-lookup"><span data-stu-id="b0615-123">Remarks</span></span>

<span data-ttu-id="b0615-p103">从**最近**操作返回的部分 driveItem 将包括 **remoteItem** 方面，这表明它们是其他驱动器中的项目。若要访问原始的 driveItem 对象，你将需要使用 **remoteItem** 中提供的信息发出请求，信息格式如下：</span><span class="sxs-lookup"><span data-stu-id="b0615-p103">Some driveItems returned from the **recent** action will include the **remoteItem** facet which indicates they are items from another drive. To access the original driveItem object, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

<!--
{
  "type": "#page.annotation",
  "description": "Retrieve a list of recently used files for the owner of the drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Drives/Recent files",
  "suppressions": [
    "Error: /api-reference/beta/api/drive-recent.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/drive-recent.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-recent.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
