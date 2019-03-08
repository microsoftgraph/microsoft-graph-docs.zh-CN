---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 获取列表项的以前版本 - SharePoint API
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 88f442178d3e703c4861e3a6fe5746a7f0c5e8b8
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482103"
---
# <a name="get-a-listitemversion-resource-preview"></a><span data-ttu-id="086e0-102">获取 ListItemVersion 资源（预览）</span><span class="sxs-lookup"><span data-stu-id="086e0-102">Get a ListItemVersion resource (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="086e0-103">检索 [ListItem](../resources/listitem.md) 的某个特定版本的元数据。</span><span class="sxs-lookup"><span data-stu-id="086e0-103">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="086e0-104">权限</span><span class="sxs-lookup"><span data-stu-id="086e0-104">Permissions</span></span>

<span data-ttu-id="086e0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="086e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="086e0-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="086e0-107">Permission type</span></span>             | <span data-ttu-id="086e0-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="086e0-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="086e0-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="086e0-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="086e0-110">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="086e0-110">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="086e0-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="086e0-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="086e0-112">无</span><span class="sxs-lookup"><span data-stu-id="086e0-112">n/a</span></span>                                         |
| <span data-ttu-id="086e0-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="086e0-113">Application</span></span>                            | <span data-ttu-id="086e0-114">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="086e0-114">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="086e0-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="086e0-115">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="086e0-116">响应</span><span class="sxs-lookup"><span data-stu-id="086e0-116">Response</span></span>

<span data-ttu-id="086e0-117">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ListItemVersion](../resources/listitemversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="086e0-117">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="086e0-118">示例</span><span class="sxs-lookup"><span data-stu-id="086e0-118">Example</span></span>

<span data-ttu-id="086e0-119">本示例检索 listItem 的版本，并扩展字段集合以请求 listItem 中的字段值。</span><span class="sxs-lookup"><span data-stu-id="086e0-119">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="086e0-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="086e0-120">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="086e0-121">响应</span><span class="sxs-lookup"><span data-stu-id="086e0-121">Response</span></span>

<span data-ttu-id="086e0-122">这将返回版本的集合：</span><span class="sxs-lookup"><span data-stu-id="086e0-122">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "1.0",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "fields": {  }
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
    "Error: /api-reference/beta/api/listitemversion-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
