---
title: pendingContentUpdate
description: PendingContentUpdate 资源指示可能影响 driveItem 的二进制内容的操作处于 "正在等待" 已完成。
localization_priority: Normal
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5e7291ac4591ba63bec96108dd46bf9561358bb4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998083"
---
# <a name="pendingcontentupdate-resource-type"></a><span data-ttu-id="5eda4-103">pendingContentUpdate 资源类型</span><span class="sxs-lookup"><span data-stu-id="5eda4-103">pendingContentUpdate resource type</span></span>

<span data-ttu-id="5eda4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5eda4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5eda4-105">指示可能会影响 **driveItem** 的二进制内容的操作正在等待完成。</span><span class="sxs-lookup"><span data-stu-id="5eda4-105">Indicates that an operation that might affect the binary content of the **driveItem** is pending completion.</span></span>

## <a name="properties"></a><span data-ttu-id="5eda4-106">属性</span><span class="sxs-lookup"><span data-stu-id="5eda4-106">Properties</span></span>

| <span data-ttu-id="5eda4-107">属性</span><span class="sxs-lookup"><span data-stu-id="5eda4-107">Property</span></span>     | <span data-ttu-id="5eda4-108">类型</span><span class="sxs-lookup"><span data-stu-id="5eda4-108">Type</span></span>         | <span data-ttu-id="5eda4-109">说明</span><span class="sxs-lookup"><span data-stu-id="5eda4-109">Description</span></span> |
|:-------------|:-------------|:------------|
|<span data-ttu-id="5eda4-110">queuedDateTime</span><span class="sxs-lookup"><span data-stu-id="5eda4-110">queuedDateTime</span></span>|<span data-ttu-id="5eda4-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5eda4-111">DateTimeOffset</span></span>|<span data-ttu-id="5eda4-112">在 UTC 时间内排队待执行的二进制操作的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5eda4-112">Date and time the pending binary operation was queued in UTC time.</span></span> <span data-ttu-id="5eda4-113">只读。</span><span class="sxs-lookup"><span data-stu-id="5eda4-113">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5eda4-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5eda4-114">JSON representation</span></span>

<span data-ttu-id="5eda4-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5eda4-115">The following is a JSON representation of the resource.</span></span>

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


