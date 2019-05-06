---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: 获取分析结果
localization_priority: Normal
ms.openlocfilehash: b0112041d6b8a8fead91ff76501d9e9b5f1c3102
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33598314"
---
# <a name="get-analytics"></a><span data-ttu-id="38e98-102">获取分析结果</span><span class="sxs-lookup"><span data-stu-id="38e98-102">Get analytics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38e98-103">获取有关在此资源下发生的视图的[itemAnalytics][] 。</span><span class="sxs-lookup"><span data-stu-id="38e98-103">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="38e98-104">**ItemAnalytics**资源是获取`allTime`和的`lastSevenDays`活动统计信息的便捷方式。</span><span class="sxs-lookup"><span data-stu-id="38e98-104">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="38e98-105">对于自定义时间范围或时间间隔, 请使用[getActivitiesByInterval][] API。</span><span class="sxs-lookup"><span data-stu-id="38e98-105">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="38e98-106">**注意:\*\*\*\*ItemAnalytics**资源在所有[国家/地区部署](/graph/deployments)中尚不可用。</span><span class="sxs-lookup"><span data-stu-id="38e98-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="38e98-109">权限</span><span class="sxs-lookup"><span data-stu-id="38e98-109">Permissions</span></span>

<span data-ttu-id="38e98-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38e98-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38e98-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="38e98-112">Permission type</span></span>                        | <span data-ttu-id="38e98-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="38e98-113">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="38e98-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38e98-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="38e98-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38e98-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="38e98-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38e98-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38e98-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="38e98-117">Not supported.</span></span>
|<span data-ttu-id="38e98-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="38e98-118">Application</span></span>                            | <span data-ttu-id="38e98-119">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38e98-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="38e98-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38e98-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="38e98-121">示例</span><span class="sxs-lookup"><span data-stu-id="38e98-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="38e98-122">请求</span><span class="sxs-lookup"><span data-stu-id="38e98-122">Request</span></span>

<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```

#### <a name="response"></a><span data-ttu-id="38e98-123">响应</span><span class="sxs-lookup"><span data-stu-id="38e98-123">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="38e98-124">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="38e98-124">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="38e98-125">语言</span><span class="sxs-lookup"><span data-stu-id="38e98-125">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-analytics-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="38e98-126">Javascript</span><span class="sxs-lookup"><span data-stu-id="38e98-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-analytics-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics",
  "suppressions": [
    "Error: /api-reference/beta/api/itemanalytics-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/itemanalytics-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
