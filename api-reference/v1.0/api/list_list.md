---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: 列出网站中的 SharePoint 列表
ms.openlocfilehash: 5d88720ecf3d183f806526364130dd2812874f3c
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2018
ms.locfileid: "23267645"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="897e5-102">枚举网站中的列表</span><span class="sxs-lookup"><span data-stu-id="897e5-102">Enumerate lists in a site</span></span>

<span data-ttu-id="897e5-103">获取 [site][] 的 [lists][] 的集合。</span><span class="sxs-lookup"><span data-stu-id="897e5-103">Get the collection of [lists][] for a [site][].</span></span>

[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="897e5-106">权限</span><span class="sxs-lookup"><span data-stu-id="897e5-106">Permissions</span></span>

<span data-ttu-id="897e5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="897e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="897e5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="897e5-109">Permission type</span></span>      | <span data-ttu-id="897e5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="897e5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="897e5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="897e5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="897e5-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="897e5-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="897e5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="897e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="897e5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="897e5-114">Not supported.</span></span>    |
|<span data-ttu-id="897e5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="897e5-115">Application</span></span> | <span data-ttu-id="897e5-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="897e5-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="897e5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="897e5-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="897e5-118">示例</span><span class="sxs-lookup"><span data-stu-id="897e5-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="897e5-119">请求</span><span class="sxs-lookup"><span data-stu-id="897e5-119">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="897e5-120">响应</span><span class="sxs-lookup"><span data-stu-id="897e5-120">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "b57af081-936c-4803-a120-d94887b03864",
      "name": "Documents",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "documentLibrary"
       }
    },
    {
      "id": "1234-112-112-4",
      "name": "MicroFeed",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "genericList"
       }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="897e5-121">注解</span><span class="sxs-lookup"><span data-stu-id="897e5-121">Remarks</span></span>

<span data-ttu-id="897e5-122">默认情况下，将隐藏包含 [system][] Facet 的列表。</span><span class="sxs-lookup"><span data-stu-id="897e5-122">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="897e5-123">若要列出它们，请在 `$select` 语句中添加 `system`。</span><span class="sxs-lookup"><span data-stu-id="897e5-123">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemFacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate"
} -->
