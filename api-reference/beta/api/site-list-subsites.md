---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 列出 SharePoint 网站的子网站
localization_priority: Normal
ms.openlocfilehash: b773dc217836fe2474c244917773d9496d158a6a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835425"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="9ea53-102">枚举子网站</span><span class="sxs-lookup"><span data-stu-id="9ea53-102">Enumerate subsites</span></span>

> <span data-ttu-id="9ea53-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9ea53-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ea53-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9ea53-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9ea53-105">获取为 [网站][] 定义的子网站集合。</span><span class="sxs-lookup"><span data-stu-id="9ea53-105">Get a collection of subsites defined for a [site][].</span></span>

[网站]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="9ea53-107">权限</span><span class="sxs-lookup"><span data-stu-id="9ea53-107">Permissions</span></span>

<span data-ttu-id="9ea53-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ea53-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ea53-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ea53-110">Permission type</span></span>      | <span data-ttu-id="9ea53-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9ea53-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ea53-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ea53-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9ea53-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ea53-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9ea53-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ea53-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ea53-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ea53-115">Not supported.</span></span>    |
|<span data-ttu-id="9ea53-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ea53-116">Application</span></span> | <span data-ttu-id="9ea53-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ea53-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ea53-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ea53-118">HTTP request</span></span>

<!-- { "blockType": "request", "name": "list-subsites", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/sites
```

## <a name="response"></a><span data-ttu-id="9ea53-119">响应</span><span class="sxs-lookup"><span data-stu-id="9ea53-119">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Team A Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteA"
    },
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Team B Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteB"
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/List subsites"
} -->
