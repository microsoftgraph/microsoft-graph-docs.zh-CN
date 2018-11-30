---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: 列出网站中的 SharePoint 列表
ms.openlocfilehash: bae0bc23c6a50200c0c380470bb5c70943c6ab0e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049061"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="bb78c-102">枚举网站中的列表</span><span class="sxs-lookup"><span data-stu-id="bb78c-102">Enumerate lists in a site</span></span>

> <span data-ttu-id="bb78c-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bb78c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb78c-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bb78c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bb78c-105">获取 [site][] 的 [lists][] 的集合。</span><span class="sxs-lookup"><span data-stu-id="bb78c-105">Get the collection of [lists][] for a [site][].</span></span>

[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="bb78c-108">权限</span><span class="sxs-lookup"><span data-stu-id="bb78c-108">Permissions</span></span>

<span data-ttu-id="bb78c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb78c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb78c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb78c-111">Permission type</span></span>      | <span data-ttu-id="bb78c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb78c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb78c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb78c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bb78c-114">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb78c-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="bb78c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb78c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb78c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb78c-116">Not supported.</span></span>    |
|<span data-ttu-id="bb78c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb78c-117">Application</span></span> | <span data-ttu-id="bb78c-118">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb78c-118">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb78c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb78c-119">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="bb78c-120">示例</span><span class="sxs-lookup"><span data-stu-id="bb78c-120">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bb78c-121">请求</span><span class="sxs-lookup"><span data-stu-id="bb78c-121">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="bb78c-122">响应</span><span class="sxs-lookup"><span data-stu-id="bb78c-122">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="bb78c-123">注解</span><span class="sxs-lookup"><span data-stu-id="bb78c-123">Remarks</span></span>

<span data-ttu-id="bb78c-124">默认情况下，将隐藏包含 [system][] Facet 的列表。</span><span class="sxs-lookup"><span data-stu-id="bb78c-124">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="bb78c-125">若要列出它们，请在 `$select` 语句中添加 `system`。</span><span class="sxs-lookup"><span data-stu-id="bb78c-125">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate"
} -->
