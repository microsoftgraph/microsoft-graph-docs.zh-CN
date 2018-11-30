---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 获取列表项的以前版本 - SharePoint API
ms.openlocfilehash: 05d2545ee6ce67c558e16144b324bb7722a7d884
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045395"
---
# <a name="get-a-listitemversion-resource-preview"></a><span data-ttu-id="4a971-102">获取 ListItemVersion 资源（预览）</span><span class="sxs-lookup"><span data-stu-id="4a971-102">Get a ListItemVersion resource (preview)</span></span>

> <span data-ttu-id="4a971-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4a971-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a971-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4a971-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4a971-105">检索 [ListItem](../resources/listitem.md) 的某个特定版本的元数据。</span><span class="sxs-lookup"><span data-stu-id="4a971-105">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a971-106">权限</span><span class="sxs-lookup"><span data-stu-id="4a971-106">Permissions</span></span>

<span data-ttu-id="4a971-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a971-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="4a971-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a971-109">Permission type</span></span>             | <span data-ttu-id="4a971-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4a971-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="4a971-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a971-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a971-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a971-112">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="4a971-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a971-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a971-114">无</span><span class="sxs-lookup"><span data-stu-id="4a971-114">n/a</span></span>                                         |
| <span data-ttu-id="4a971-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a971-115">Application</span></span>                            | <span data-ttu-id="4a971-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a971-116">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="4a971-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a971-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="4a971-118">响应</span><span class="sxs-lookup"><span data-stu-id="4a971-118">Response</span></span>

<span data-ttu-id="4a971-119">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ListItemVersion](../resources/listitemversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4a971-119">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="4a971-120">示例</span><span class="sxs-lookup"><span data-stu-id="4a971-120">Example</span></span>

<span data-ttu-id="4a971-121">本示例检索 listItem 的版本，并扩展字段集合以请求 listItem 中的字段值。</span><span class="sxs-lookup"><span data-stu-id="4a971-121">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="4a971-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a971-122">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="4a971-123">响应</span><span class="sxs-lookup"><span data-stu-id="4a971-123">Response</span></span>

<span data-ttu-id="4a971-124">这将返回版本的集合：</span><span class="sxs-lookup"><span data-stu-id="4a971-124">This returns a collection of versions:</span></span>

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