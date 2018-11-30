---
title: 获取 ListItemVersion 资源
description: 检索 ListItem 的某个特定版本的元数据。
ms.openlocfilehash: 2796449496d14dd3c4a1faeeb52871a07fcb9599
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008653"
---
# <a name="get-a-listitemversion-resource"></a><span data-ttu-id="c2420-103">获取 ListItemVersion 资源</span><span class="sxs-lookup"><span data-stu-id="c2420-103">Get a ListItemVersion resource</span></span>

<span data-ttu-id="c2420-104">检索 [ListItem](../resources/listitem.md) 的某个特定版本的元数据。</span><span class="sxs-lookup"><span data-stu-id="c2420-104">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c2420-105">权限</span><span class="sxs-lookup"><span data-stu-id="c2420-105">Permissions</span></span>

<span data-ttu-id="c2420-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2420-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="c2420-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2420-108">Permission type</span></span>             | <span data-ttu-id="c2420-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c2420-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c2420-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2420-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2420-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2420-111">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="c2420-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2420-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2420-113">无</span><span class="sxs-lookup"><span data-stu-id="c2420-113">n/a</span></span>                                         |
| <span data-ttu-id="c2420-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c2420-114">Application</span></span>                            | <span data-ttu-id="c2420-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2420-115">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="c2420-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2420-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="c2420-117">响应</span><span class="sxs-lookup"><span data-stu-id="c2420-117">Response</span></span>

<span data-ttu-id="c2420-118">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ListItemVersion](../resources/listitemversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c2420-118">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="c2420-119">示例</span><span class="sxs-lookup"><span data-stu-id="c2420-119">Example</span></span>

<span data-ttu-id="c2420-120">本示例检索 listItem 的版本，并扩展字段集合以请求 listItem 中的字段值。</span><span class="sxs-lookup"><span data-stu-id="c2420-120">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="c2420-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2420-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read sites.read.all", "tags": "service.graph service.sharepoint" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="c2420-122">响应</span><span class="sxs-lookup"><span data-stu-id="c2420-122">Response</span></span>

<span data-ttu-id="c2420-123">这将返回版本的集合：</span><span class="sxs-lookup"><span data-stu-id="c2420-123">This returns a collection of versions:</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
