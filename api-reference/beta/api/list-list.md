---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: 列出网站中的 SharePoint 列表
localization_priority: Normal
ms.openlocfilehash: fbba85c9bb1807955670d19398e2175c3805f64f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851699"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="59327-102">枚举网站中的列表</span><span class="sxs-lookup"><span data-stu-id="59327-102">Enumerate lists in a site</span></span>

> <span data-ttu-id="59327-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="59327-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59327-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="59327-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="59327-105">获取 [site][] 的 [lists][] 的集合。</span><span class="sxs-lookup"><span data-stu-id="59327-105">Get the collection of [lists][] for a [site][].</span></span>

[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="59327-108">权限</span><span class="sxs-lookup"><span data-stu-id="59327-108">Permissions</span></span>

<span data-ttu-id="59327-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59327-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59327-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="59327-111">Permission type</span></span>      | <span data-ttu-id="59327-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59327-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59327-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59327-113">Delegated (work or school account)</span></span> | <span data-ttu-id="59327-114">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59327-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="59327-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59327-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59327-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="59327-116">Not supported.</span></span>    |
|<span data-ttu-id="59327-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="59327-117">Application</span></span> | <span data-ttu-id="59327-118">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59327-118">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="59327-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59327-119">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="59327-120">示例</span><span class="sxs-lookup"><span data-stu-id="59327-120">Example</span></span>

#### <a name="request"></a><span data-ttu-id="59327-121">请求</span><span class="sxs-lookup"><span data-stu-id="59327-121">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="59327-122">响应</span><span class="sxs-lookup"><span data-stu-id="59327-122">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="59327-123">注解</span><span class="sxs-lookup"><span data-stu-id="59327-123">Remarks</span></span>

<span data-ttu-id="59327-124">默认情况下，将隐藏包含 [system][] Facet 的列表。</span><span class="sxs-lookup"><span data-stu-id="59327-124">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="59327-125">若要列出它们，请在 `$select` 语句中添加 `system`。</span><span class="sxs-lookup"><span data-stu-id="59327-125">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate"
} -->
