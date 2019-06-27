---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 列出与我共享的文件
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c9c5681443ba6c4621f3be9836433cd87a9a4ca5
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260296"
---
# <a name="list-items-shared-with-the-signed-in-user"></a><span data-ttu-id="8da74-102">列出与已登录用户共享的项目</span><span class="sxs-lookup"><span data-stu-id="8da74-102">List items shared with the signed-in user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8da74-103">检索已与[驱动器](../resources/drive.md)所有者共享的 [DriveItem](../resources/driveitem.md) 资源的集合。</span><span class="sxs-lookup"><span data-stu-id="8da74-103">Retrieve a collection of [DriveItem](../resources/driveitem.md) resources that have been shared with the owner of the [Drive](../resources/drive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8da74-104">权限</span><span class="sxs-lookup"><span data-stu-id="8da74-104">Permissions</span></span>

<span data-ttu-id="8da74-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8da74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8da74-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="8da74-107">Permission type</span></span>      | <span data-ttu-id="8da74-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8da74-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8da74-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8da74-109">Delegated (work or school account)</span></span> | <span data-ttu-id="8da74-110">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8da74-110">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8da74-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8da74-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8da74-112">Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8da74-112">Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8da74-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="8da74-113">Application</span></span> | <span data-ttu-id="8da74-114">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8da74-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

<span data-ttu-id="8da74-115">**注意：** 虽然 /sharedWithMe 请求可通过 Files.Read 或 Files.ReadWrite 权限成功发出，但一些属性可能会丢失。</span><span class="sxs-lookup"><span data-stu-id="8da74-115">**Note:** while the /sharedWithMe request will succeed with Files.Read or Files.ReadWrite permissions, some properties may be missing.</span></span>
<span data-ttu-id="8da74-116">此外，如果没有 **All** 权限之一，则无法访问从此 API 返回的共享项。</span><span class="sxs-lookup"><span data-stu-id="8da74-116">Additionally, without one of the  **All** permissions, shared items returned from this API will not be accessible.</span></span>

## <a name="http-request"></a><span data-ttu-id="8da74-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8da74-117">HTTP request</span></span>

<!-- { "blockType": "request", "name": "shared-with-me", "scopes": "files.read", "target": "action" } -->

```http
GET /me/drive/sharedWithMe
```

## <a name="response"></a><span data-ttu-id="8da74-118">响应</span><span class="sxs-lookup"><span data-stu-id="8da74-118">Response</span></span>

<span data-ttu-id="8da74-p103">此方法返回 [DriveItem](../resources/driveitem.md) 资源的集合，这些资源包含已与驱动器所有者共享的 DriveItem 资源。在此示例中，由于此驱动器是用户的默认驱动器，此方法将返回与已登录用户共享的项目。</span><span class="sxs-lookup"><span data-stu-id="8da74-p103">This returns a collection of [DriveItem](../resources/driveitem.md) resources which contain the DriveItem resources shared with the owner of the drive. In this example, since the drive is the user's default drive, this returns items shared with the signed in user.</span></span>

<!-- {"blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc",
      "remoteItem": {
        "id": "1991210caf!192",
        "name": "March Proposal.docx",
        "file": { },
        "size": 19121,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    },
    {
      "id": "1312def",
      "remoteItem": {
        "id": "1991210caf!1991",
        "name": "Team Roster.xlsx",
        "file": { },
        "size": 37619,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8da74-121">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="8da74-121">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8da74-122">C#</span><span class="sxs-lookup"><span data-stu-id="8da74-122">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/shared-with-me-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8da74-123">Javascript</span><span class="sxs-lookup"><span data-stu-id="8da74-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/shared-with-me-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8da74-124">目标-C</span><span class="sxs-lookup"><span data-stu-id="8da74-124">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/shared-with-me-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="8da74-125">注解</span><span class="sxs-lookup"><span data-stu-id="8da74-125">Remarks</span></span>

<span data-ttu-id="8da74-p104">从 **sharedWithMe** 操作返回的 driveItem 始终都将包括 [**remoteItem**](../resources/remoteitem.md) 方面，这表明它们是其他驱动器中的项目。若要访问共享的 DriveItem 资源，你将需要使用 **remoteItem** 中提供的信息发出请求，信息格式如下：</span><span class="sxs-lookup"><span data-stu-id="8da74-p104">DriveItems returned from the **sharedWithMe** action will always include the [**remoteItem**](../resources/remoteitem.md) facet which indicates they are items from a different drive. To access the shared DriveItem resource, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

<!--
{
  "type": "#page.annotation",
  "description": "List the items shared with the owner of a drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Sharing/Shared with me",
  "suppressions": [
    "Error: /api-reference/beta/api/drive-sharedwithme.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/drive-sharedwithme.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-sharedwithme.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
