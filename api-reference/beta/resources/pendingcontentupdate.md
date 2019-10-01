---
title: pendingContentUpdate
description: PendingContentUpdate 资源指示可能影响 driveItem 的二进制内容的操作处于 "正在等待" 已完成。
localization_priority: Normal
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1637ac3faa1d42cd47f49735a1b24fb60868a23d
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333393"
---
# <a name="pendingcontentupdate-resource-type"></a><span data-ttu-id="d3d65-103">pendingContentUpdate 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3d65-103">pendingContentUpdate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3d65-104">指示可能会影响**driveItem**的二进制内容的操作正在等待完成。</span><span class="sxs-lookup"><span data-stu-id="d3d65-104">Indicates that an operation that might affect the binary content of the **driveItem** is pending completion.</span></span>

## <a name="properties"></a><span data-ttu-id="d3d65-105">属性</span><span class="sxs-lookup"><span data-stu-id="d3d65-105">Properties</span></span>

| <span data-ttu-id="d3d65-106">属性</span><span class="sxs-lookup"><span data-stu-id="d3d65-106">Property</span></span>     | <span data-ttu-id="d3d65-107">类型</span><span class="sxs-lookup"><span data-stu-id="d3d65-107">Type</span></span>         | <span data-ttu-id="d3d65-108">说明</span><span class="sxs-lookup"><span data-stu-id="d3d65-108">Description</span></span> |
|:-------------|:-------------|:------------|
|<span data-ttu-id="d3d65-109">queuedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3d65-109">queuedDateTime</span></span>|<span data-ttu-id="d3d65-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3d65-110">DateTimeOffset</span></span>|<span data-ttu-id="d3d65-111">在 UTC 时间内排队待执行的二进制操作的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d3d65-111">Date and time the pending binary operation was queued in UTC time.</span></span> <span data-ttu-id="d3d65-112">只读。</span><span class="sxs-lookup"><span data-stu-id="d3d65-112">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3d65-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3d65-113">JSON representation</span></span>

<span data-ttu-id="d3d65-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3d65-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pendingContentUpdate",
  "baseType": null
}-->

```json
{
  "queuedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The pendingContentUpdate resource indicates that an operation that may affect the binary content of the DriveItem is pending completion.",
  "keywords": "pendingoperation,operation,pendingcontentupdate",
  "section": "documentation",
  "tocPath": ""
}-->
