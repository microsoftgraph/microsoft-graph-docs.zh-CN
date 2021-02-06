---
title: termsExpiration 资源类型
description: 在设置协议的计划到期时提供其他设置。
localization_priority: Normal
ms.prod: governance
author: raprakasMSFT
doc_type: resourcePageType
ms.openlocfilehash: 3f31489a80c87dd17a31500818c0c650c57c8a7c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128503"
---
# <a name="termsexpiration-resource-type"></a><span data-ttu-id="29e16-103">termsExpiration 资源类型</span><span class="sxs-lookup"><span data-stu-id="29e16-103">termsExpiration resource type</span></span>

<span data-ttu-id="29e16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29e16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29e16-105">在设置协议的计划到期时提供其他设置。</span><span class="sxs-lookup"><span data-stu-id="29e16-105">Provides additional settings when setting the scheduled expiration of the agreement.</span></span>

## <a name="properties"></a><span data-ttu-id="29e16-106">属性</span><span class="sxs-lookup"><span data-stu-id="29e16-106">Properties</span></span>

| <span data-ttu-id="29e16-107">属性</span><span class="sxs-lookup"><span data-stu-id="29e16-107">Property</span></span>                     | <span data-ttu-id="29e16-108">类型</span><span class="sxs-lookup"><span data-stu-id="29e16-108">Type</span></span>                      | <span data-ttu-id="29e16-109">说明</span><span class="sxs-lookup"><span data-stu-id="29e16-109">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="29e16-110">startDateTime</span><span class="sxs-lookup"><span data-stu-id="29e16-110">startDateTime</span></span>|<span data-ttu-id="29e16-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29e16-111">DateTimeOffset</span></span> | <span data-ttu-id="29e16-112">协议设置为对所有用户过期的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="29e16-112">The DateTime when the agreement is set to expire for all users.</span></span> <span data-ttu-id="29e16-113">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="29e16-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="29e16-114">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="29e16-114">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|
| <span data-ttu-id="29e16-115">frequency</span><span class="sxs-lookup"><span data-stu-id="29e16-115">frequency</span></span>| <span data-ttu-id="29e16-116">持续时间</span><span class="sxs-lookup"><span data-stu-id="29e16-116">Duration</span></span> | <span data-ttu-id="29e16-117">表示术语在 **startDateTime** 中设置的首次过期后过期的频率。</span><span class="sxs-lookup"><span data-stu-id="29e16-117">Represents the frequency at which the terms will expire, after its first expiration as set in **startDateTime**.</span></span> <span data-ttu-id="29e16-118">该值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="29e16-118">The value is represented in ISO 8601 format for durations.</span></span> <span data-ttu-id="29e16-119">例如， `PT1M` 表示 1 个月的时间段。</span><span class="sxs-lookup"><span data-stu-id="29e16-119">For example, `PT1M` represents a time period of 1 month.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29e16-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29e16-120">JSON representation</span></span>

<span data-ttu-id="29e16-121">下面是此资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29e16-121">The following is a JSON representation of this resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.termsExpiration",
}-->

```json
{
   "startDateTime": "2018-10-01T00:00:00.0000000Z",
   "frequency": "Duration"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "termsExpiration complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


