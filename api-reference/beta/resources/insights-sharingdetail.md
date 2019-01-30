---
title: sharingDetail 资源类型
description: '包含共享项目的属性的复杂类型。 '
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 3fff669b2b337e9566cd41a7cd5eb5ab73a84944
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643347"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="6a250-103">sharingDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a250-103">sharingDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a250-104">包含[共享](insights-shared.md)项目的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="6a250-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="6a250-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a250-105">JSON representation</span></span>
<span data-ttu-id="6a250-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a250-106">Here is a JSON representation of the resource</span></span>

```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a><span data-ttu-id="6a250-107">属性</span><span class="sxs-lookup"><span data-stu-id="6a250-107">Properties</span></span>

| <span data-ttu-id="6a250-108">属性</span><span class="sxs-lookup"><span data-stu-id="6a250-108">Property</span></span>              | <span data-ttu-id="6a250-109">类型</span><span class="sxs-lookup"><span data-stu-id="6a250-109">Type</span></span>          | <span data-ttu-id="6a250-110">说明</span><span class="sxs-lookup"><span data-stu-id="6a250-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="6a250-111">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a250-111">sharedDateTime</span></span>        | <span data-ttu-id="6a250-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a250-112">DateTimeOffset</span></span>| <span data-ttu-id="6a250-113">日期和时间上次共享文件。</span><span class="sxs-lookup"><span data-stu-id="6a250-113">The date and time the file was last shared.</span></span> <span data-ttu-id="6a250-114">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="6a250-114">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6a250-115">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="6a250-115">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="6a250-116">只读。</span><span class="sxs-lookup"><span data-stu-id="6a250-116">Read-only.</span></span>  |
| <span data-ttu-id="6a250-117">sharingSubject</span><span class="sxs-lookup"><span data-stu-id="6a250-117">sharingSubject</span></span>        | <span data-ttu-id="6a250-118">String</span><span class="sxs-lookup"><span data-stu-id="6a250-118">String</span></span>          | <span data-ttu-id="6a250-119">与共享文档主题。</span><span class="sxs-lookup"><span data-stu-id="6a250-119">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="6a250-120">sharingType</span><span class="sxs-lookup"><span data-stu-id="6a250-120">sharingType</span></span>             | <span data-ttu-id="6a250-121">String</span><span class="sxs-lookup"><span data-stu-id="6a250-121">String</span></span>        | <span data-ttu-id="6a250-122">确定文档的方式共享，则可以通过"链接"、"附件"、"组"、"Site"。</span><span class="sxs-lookup"><span data-stu-id="6a250-122">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="6a250-123">sharedBy</span><span class="sxs-lookup"><span data-stu-id="6a250-123">sharedBy</span></span>                | [<span data-ttu-id="6a250-124">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="6a250-124">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="6a250-125">共享文档的用户。</span><span class="sxs-lookup"><span data-stu-id="6a250-125">The user who shared the document.</span></span>  |
| <span data-ttu-id="6a250-126">sharingReference</span><span class="sxs-lookup"><span data-stu-id="6a250-126">sharingReference</span></span>        | [<span data-ttu-id="6a250-127">resourceReference</span><span class="sxs-lookup"><span data-stu-id="6a250-127">resourceReference</span></span>](insights-resourcereference.md)      |  |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-sharingdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
