---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 列出最近的文件
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d50954f06001b53aa02b9fb49d3daab1a686f42a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589335"
---
# <a name="list-recent-files"></a><span data-ttu-id="cf4a1-102">列出最近使用的文件</span><span class="sxs-lookup"><span data-stu-id="cf4a1-102">List recent files</span></span>

<span data-ttu-id="cf4a1-p101">列出已登录用户最近使用的一组项目。此集合包含用户驱动器中的项目，以及他们有从其他驱动器进行访问的权限的项目。</span><span class="sxs-lookup"><span data-stu-id="cf4a1-p101">List a set of items that have been recently used by the signed in user. This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf4a1-105">权限</span><span class="sxs-lookup"><span data-stu-id="cf4a1-105">Permissions</span></span>

<span data-ttu-id="cf4a1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf4a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf4a1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf4a1-108">Permission type</span></span>      | <span data-ttu-id="cf4a1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf4a1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf4a1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf4a1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cf4a1-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf4a1-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="cf4a1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf4a1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf4a1-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf4a1-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="cf4a1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf4a1-114">Application</span></span> | <span data-ttu-id="cf4a1-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf4a1-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf4a1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf4a1-116">HTTP request</span></span>

<!-- { "blockType": "request",
       "name": "view-recent-files", 
       "scopes": "files.read",
       "tags": "service.graph",
       "target": "action" } -->

```http
GET /me/drive/recent
```

## <a name="response"></a><span data-ttu-id="cf4a1-117">响应</span><span class="sxs-lookup"><span data-stu-id="cf4a1-117">Response</span></span>

<span data-ttu-id="cf4a1-118">此方法返回驱动器所有者最近访问的项的 [DriveItem](../resources/driveitem.md) 资源集合。</span><span class="sxs-lookup"><span data-stu-id="cf4a1-118">This method returns a collection of [DriveItem](../resources/driveitem.md) resources for items which the owner of the drive has recently accessed.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="cf4a1-119">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="cf4a1-119">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cf4a1-120">语言</span><span class="sxs-lookup"><span data-stu-id="cf4a1-120">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/view-recent-files-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cf4a1-121">Javascript</span><span class="sxs-lookup"><span data-stu-id="cf4a1-121">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/view-recent-files-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="cf4a1-122">注解</span><span class="sxs-lookup"><span data-stu-id="cf4a1-122">Remarks</span></span>

<span data-ttu-id="cf4a1-p103">从**最近**操作返回的部分 driveItem 将包括 **remoteItem** 方面，这表明它们是其他驱动器中的项目。若要访问原始的 driveItem 对象，你将需要使用 **remoteItem** 中提供的信息发出请求，信息格式如下：</span><span class="sxs-lookup"><span data-stu-id="cf4a1-p103">Some driveItems returned from the **recent** action will include the **remoteItem** facet which indicates they are items from another drive. To access the original driveItem object, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of recently used files for the owner of the drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Drives/Recent files",
  "suppressions": [
    "Error: /api-reference/v1.0/api/drive-recent.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-recent.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
