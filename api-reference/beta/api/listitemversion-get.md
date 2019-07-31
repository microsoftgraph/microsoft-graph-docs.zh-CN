---
author: JeremyKelley
description: 检索 ListItem 的某个特定版本的元数据。
ms.date: 09/10/2017
title: 获取列表项的以前版本 - SharePoint API
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 752287ac5e004688e1dd1747f3689c5f460dc946
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984090"
---
# <a name="get-a-listitemversion-resource-preview"></a><span data-ttu-id="1c021-103">获取 ListItemVersion 资源（预览）</span><span class="sxs-lookup"><span data-stu-id="1c021-103">Get a ListItemVersion resource (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c021-104">检索 [ListItem](../resources/listitem.md) 的某个特定版本的元数据。</span><span class="sxs-lookup"><span data-stu-id="1c021-104">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1c021-105">权限</span><span class="sxs-lookup"><span data-stu-id="1c021-105">Permissions</span></span>

<span data-ttu-id="1c021-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1c021-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="1c021-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c021-108">Permission type</span></span>             | <span data-ttu-id="1c021-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1c021-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="1c021-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c021-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c021-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c021-111">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="1c021-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c021-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c021-113">无</span><span class="sxs-lookup"><span data-stu-id="1c021-113">n/a</span></span>                                         |
| <span data-ttu-id="1c021-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c021-114">Application</span></span>                            | <span data-ttu-id="1c021-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c021-115">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="1c021-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c021-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="1c021-117">响应</span><span class="sxs-lookup"><span data-stu-id="1c021-117">Response</span></span>

<span data-ttu-id="1c021-118">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ListItemVersion](../resources/listitemversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1c021-118">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="1c021-119">示例</span><span class="sxs-lookup"><span data-stu-id="1c021-119">Example</span></span>

<span data-ttu-id="1c021-120">本示例检索 listItem 的版本，并扩展字段集合以请求 listItem 中的字段值。</span><span class="sxs-lookup"><span data-stu-id="1c021-120">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="1c021-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c021-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="1c021-122">响应</span><span class="sxs-lookup"><span data-stu-id="1c021-122">Response</span></span>

<span data-ttu-id="1c021-123">这将返回版本的集合：</span><span class="sxs-lookup"><span data-stu-id="1c021-123">This returns a collection of versions:</span></span>

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
  "suppressions": []
}
-->
