---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 获取 SharePoint 列表记录的以前版本
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b8a9078bb0e56f3c3068a92bab9835f2a4964f79
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540959"
---
# <a name="listing-versions-of-a-listitem-preview"></a><span data-ttu-id="e8821-102">列出 ListItem 的版本（预览）</span><span class="sxs-lookup"><span data-stu-id="e8821-102">Listing versions of a ListItem (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8821-103">SharePoint 可以配置为保留列表项的历史记录。</span><span class="sxs-lookup"><span data-stu-id="e8821-103">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="e8821-104">以前版本可能会保留有限的一段时间，具体取决于管理员设置，这对于每个用户或位置可能是唯一的。</span><span class="sxs-lookup"><span data-stu-id="e8821-104">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8821-105">权限</span><span class="sxs-lookup"><span data-stu-id="e8821-105">Permissions</span></span>

<span data-ttu-id="e8821-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8821-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="e8821-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8821-108">Permission type</span></span>             | <span data-ttu-id="e8821-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8821-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="e8821-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8821-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8821-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8821-111">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="e8821-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8821-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8821-113">无</span><span class="sxs-lookup"><span data-stu-id="e8821-113">n/a</span></span>                                         |
| <span data-ttu-id="e8821-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8821-114">Application</span></span>                            | <span data-ttu-id="e8821-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8821-115">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="e8821-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8821-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="e8821-117">响应</span><span class="sxs-lookup"><span data-stu-id="e8821-117">Response</span></span>

<span data-ttu-id="e8821-118">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ListItemVersion](../resources/listitemversion.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="e8821-118">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="e8821-119">示例</span><span class="sxs-lookup"><span data-stu-id="e8821-119">Example</span></span>

<span data-ttu-id="e8821-120">本示例检索 SharePoint 列表中的 listItem 的版本：</span><span class="sxs-lookup"><span data-stu-id="e8821-120">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="e8821-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8821-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="e8821-122">响应</span><span class="sxs-lookup"><span data-stu-id="e8821-122">Response</span></span>

<span data-ttu-id="e8821-123">这将返回版本的集合：</span><span class="sxs-lookup"><span data-stu-id="e8821-123">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z"
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z"
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z"
    }
  ]
}
```


<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-list-versions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
