---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 列出与我共享的文件
localization_priority: Priority
ms.prod: sharepoint
description: 检索已与驱动器所有者共享的 DriveItem 资源的集合。
doc_type: apiPageType
ms.openlocfilehash: 9bf79fefdd9b0536830aec4780bfef4f43928724
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517802"
---
# <a name="list-items-shared-with-the-signed-in-user"></a><span data-ttu-id="8c059-103">列出与已登录用户共享的项目</span><span class="sxs-lookup"><span data-stu-id="8c059-103">List items shared with the signed-in user</span></span>

<span data-ttu-id="8c059-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c059-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8c059-105">检索已与[驱动器](../resources/drive.md)所有者共享的 [DriveItem](../resources/driveitem.md) 资源的集合。</span><span class="sxs-lookup"><span data-stu-id="8c059-105">Retrieve a collection of [DriveItem](../resources/driveitem.md) resources that have been shared with the owner of the [Drive](../resources/drive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8c059-106">权限</span><span class="sxs-lookup"><span data-stu-id="8c059-106">Permissions</span></span>

<span data-ttu-id="8c059-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c059-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c059-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c059-109">Permission type</span></span>      | <span data-ttu-id="8c059-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8c059-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c059-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c059-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8c059-112">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c059-112">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8c059-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c059-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c059-114">Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c059-114">Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8c059-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c059-115">Application</span></span> | <span data-ttu-id="8c059-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c059-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

<span data-ttu-id="8c059-117">**注意：** 虽然 /sharedWithMe 请求可通过 Files.Read 或 Files.ReadWrite 权限成功发出，但一些属性可能会丢失。</span><span class="sxs-lookup"><span data-stu-id="8c059-117">**Note:** while the /sharedWithMe request will succeed with Files.Read or Files.ReadWrite permissions, some properties may be missing.</span></span>
<span data-ttu-id="8c059-118">此外，如果没有 **All** 权限之一，则无法访问从此 API 返回的共享项。</span><span class="sxs-lookup"><span data-stu-id="8c059-118">Additionally, without one of the  **All** permissions, shared items returned from this API will not be accessible.</span></span>

## <a name="http-request"></a><span data-ttu-id="8c059-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c059-119">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="8c059-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c059-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "shared-with-me", "scopes": "files.read", "tags": "service.graph", "target": "action" } -->

```msgraph-interactive
GET /me/drive/sharedWithMe
```
# <a name="c"></a>[<span data-ttu-id="8c059-121">C#</span><span class="sxs-lookup"><span data-stu-id="8c059-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shared-with-me-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c059-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c059-122">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shared-with-me-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c059-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c059-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shared-with-me-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c059-124">Java</span><span class="sxs-lookup"><span data-stu-id="8c059-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shared-with-me-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="8c059-125">响应</span><span class="sxs-lookup"><span data-stu-id="8c059-125">Response</span></span>

<span data-ttu-id="8c059-p103">此方法返回 [DriveItem](../resources/driveitem.md) 资源的集合，这些资源包含已与驱动器所有者共享的 DriveItem 资源。在此示例中，由于此驱动器是用户的默认驱动器，此方法将返回与已登录用户共享的项目。</span><span class="sxs-lookup"><span data-stu-id="8c059-p103">This returns a collection of [DriveItem](../resources/driveitem.md) resources which contain the DriveItem resources shared with the owner of the drive. In this example, since the drive is the user's default drive, this returns items shared with the signed in user.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="8c059-128">注解</span><span class="sxs-lookup"><span data-stu-id="8c059-128">Remarks</span></span>

<span data-ttu-id="8c059-p104">从 **sharedWithMe** 操作返回的 driveItem 始终都将包括 [**remoteItem**](../resources/remoteitem.md) 方面，这表明它们是其他驱动器中的项目。若要访问共享的 DriveItem 资源，你将需要使用 **remoteItem** 中提供的信息发出请求，信息格式如下：</span><span class="sxs-lookup"><span data-stu-id="8c059-p104">DriveItems returned from the **sharedWithMe** action will always include the [**remoteItem**](../resources/remoteitem.md) facet which indicates they are items from a different drive. To access the shared DriveItem resource, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

<!-- {
  "type": "#page.annotation",
  "description": "List the items shared with the owner of a drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Sharing/Shared with me",
  "suppressions": [
  ]
} -->
