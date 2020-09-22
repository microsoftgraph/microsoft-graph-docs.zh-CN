---
title: termsExpiration 资源类型
description: 在设置协议的计划到期时间时提供其他设置。
localization_priority: Normal
ms.prod: microsoft-identity-platform
author: raprakasMSFT
doc_type: resourcePageType
ms.openlocfilehash: b3b5de1d52c4a3abb1eee7d7199a539795ba1ac3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026101"
---
# <a name="termsexpiration-resource-type"></a><span data-ttu-id="5522f-103">termsExpiration 资源类型</span><span class="sxs-lookup"><span data-stu-id="5522f-103">termsExpiration resource type</span></span>

<span data-ttu-id="5522f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5522f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5522f-105">在设置协议的计划到期时间时提供其他设置。</span><span class="sxs-lookup"><span data-stu-id="5522f-105">Provides additional settings when setting the scheduled expiration of the agreement.</span></span>

## <a name="properties"></a><span data-ttu-id="5522f-106">属性</span><span class="sxs-lookup"><span data-stu-id="5522f-106">Properties</span></span>

| <span data-ttu-id="5522f-107">属性</span><span class="sxs-lookup"><span data-stu-id="5522f-107">Property</span></span>                     | <span data-ttu-id="5522f-108">类型</span><span class="sxs-lookup"><span data-stu-id="5522f-108">Type</span></span>                      | <span data-ttu-id="5522f-109">说明</span><span class="sxs-lookup"><span data-stu-id="5522f-109">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="5522f-110">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5522f-110">startDateTime</span></span>|<span data-ttu-id="5522f-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5522f-111">DateTimeOffset</span></span> | <span data-ttu-id="5522f-112">将协议设置为对所有用户过期的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5522f-112">The DateTime when the agreement is set to expire for all users.</span></span> <span data-ttu-id="5522f-113">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="5522f-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5522f-114">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="5522f-114">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|
| <span data-ttu-id="5522f-115">frequency</span><span class="sxs-lookup"><span data-stu-id="5522f-115">frequency</span></span>| <span data-ttu-id="5522f-116">持续时间</span><span class="sxs-lookup"><span data-stu-id="5522f-116">Duration</span></span> | <span data-ttu-id="5522f-117">这表示在 "startDateTime" 中设置的期限的第一次过期后的期限的到期频率。</span><span class="sxs-lookup"><span data-stu-id="5522f-117">This represents the frequency at which the terms will expire, after its first expiration as set in 'startDateTime'.</span></span> <span data-ttu-id="5522f-118">值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="5522f-118">The value is represented in ISO 8601 format for durations.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5522f-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5522f-119">JSON representation</span></span>

<span data-ttu-id="5522f-120">以下是此资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5522f-120">The following is a JSON representation of this resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.termsExpiration",
  "baseType": ""
}-->

```json
{
   "startDateTime": "2018-10-01T00:00:00.0000000Z",
   "frequency": ""
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


