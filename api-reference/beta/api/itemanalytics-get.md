---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: 获取分析
ms.openlocfilehash: 57f009e0d2a07a5bf8c9a0f3b3617083bc279545
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045731"
---
# <a name="get-analytics"></a><span data-ttu-id="9fe78-102">获取分析</span><span class="sxs-lookup"><span data-stu-id="9fe78-102">Get analytics</span></span>

> <span data-ttu-id="9fe78-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9fe78-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9fe78-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9fe78-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9fe78-105">获取[itemAnalytics][]有关发生下此资源的视图。</span><span class="sxs-lookup"><span data-stu-id="9fe78-105">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="9fe78-106">**ItemAnalytics**资源，可方便要获取的活动 stats`allTime`和`lastSevenDays`。</span><span class="sxs-lookup"><span data-stu-id="9fe78-106">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="9fe78-107">自定义的时间范围或时间间隔，使用[getActivitiesByInterval][] API。</span><span class="sxs-lookup"><span data-stu-id="9fe78-107">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="9fe78-108">**注意：\*\*\*\*ItemAnalytics**资源尚不可用所有[国家/地区的部署](/graph/deployments)中。</span><span class="sxs-lookup"><span data-stu-id="9fe78-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="9fe78-111">权限</span><span class="sxs-lookup"><span data-stu-id="9fe78-111">Permissions</span></span>

<span data-ttu-id="9fe78-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9fe78-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fe78-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="9fe78-114">Permission type</span></span>                        | <span data-ttu-id="9fe78-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9fe78-115">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="9fe78-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9fe78-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="9fe78-117">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fe78-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="9fe78-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9fe78-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fe78-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="9fe78-119">Not supported.</span></span>
|<span data-ttu-id="9fe78-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="9fe78-120">Application</span></span>                            | <span data-ttu-id="9fe78-121">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fe78-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="9fe78-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9fe78-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="9fe78-123">示例</span><span class="sxs-lookup"><span data-stu-id="9fe78-123">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9fe78-124">请求</span><span class="sxs-lookup"><span data-stu-id="9fe78-124">Request</span></span>

<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```

#### <a name="response"></a><span data-ttu-id="9fe78-125">响应</span><span class="sxs-lookup"><span data-stu-id="9fe78-125">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.itemAnalytics", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "allTime": {
        "access": {
            "actionCount": 123,
            "actorCount": 89
        }
    },
    "lastSevenDays": {
        "access": {
            "actionCount": 52,
            "actorCount": 41
        }
    }
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics"
} -->
