---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 列出最近的文件
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: be4f6632f86c62a8672bb94728dee9771aafc540
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482124"
---
# <a name="list-recent-files"></a><span data-ttu-id="d0ef2-102">列出最近使用的文件</span><span class="sxs-lookup"><span data-stu-id="d0ef2-102">List recent files</span></span>

<span data-ttu-id="d0ef2-p101">列出已登录用户最近使用的一组项目。此集合包含用户驱动器中的项目，以及他们有从其他驱动器进行访问的权限的项目。</span><span class="sxs-lookup"><span data-stu-id="d0ef2-p101">List a set of items that have been recently used by the signed in user. This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0ef2-105">权限</span><span class="sxs-lookup"><span data-stu-id="d0ef2-105">Permissions</span></span>

<span data-ttu-id="d0ef2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0ef2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0ef2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0ef2-108">Permission type</span></span>      | <span data-ttu-id="d0ef2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0ef2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0ef2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0ef2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d0ef2-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0ef2-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d0ef2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0ef2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0ef2-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0ef2-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d0ef2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0ef2-114">Application</span></span> | <span data-ttu-id="d0ef2-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0ef2-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0ef2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0ef2-116">HTTP request</span></span>

<!-- { "blockType": "request",
       "name": "view-recent-files", 
       "scopes": "files.read",
       "tags": "service.graph",
       "target": "action" } -->

```http
GET /me/drive/recent
```

## <a name="response"></a><span data-ttu-id="d0ef2-117">响应</span><span class="sxs-lookup"><span data-stu-id="d0ef2-117">Response</span></span>

<span data-ttu-id="d0ef2-118">此方法返回驱动器所有者最近访问的项的 [DriveItem](../resources/driveitem.md) 资源集合。</span><span class="sxs-lookup"><span data-stu-id="d0ef2-118">This method returns a collection of [DriveItem](../resources/driveitem.md) resources for items which the owner of the drive has recently accessed.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="d0ef2-119">注解</span><span class="sxs-lookup"><span data-stu-id="d0ef2-119">Remarks</span></span>

<span data-ttu-id="d0ef2-p103">从**最近**操作返回的部分 driveItem 将包括 **remoteItem** 方面，这表明它们是其他驱动器中的项目。若要访问原始的 driveItem 对象，你将需要使用 **remoteItem** 中提供的信息发出请求，信息格式如下：</span><span class="sxs-lookup"><span data-stu-id="d0ef2-p103">Some driveItems returned from the **recent** action will include the **remoteItem** facet which indicates they are items from another drive. To access the original driveItem object, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of recently used files for the owner of the drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Drives/Recent files"
} -->
