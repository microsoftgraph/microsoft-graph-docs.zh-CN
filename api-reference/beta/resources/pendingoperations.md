---
title: pendingOperations
description: PendingOperations 资源指示可能影响 driveItem 状态的一个或多个操作正在等待完成。
localization_priority: Normal
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d83a68bf555fa5cc239fb38b147d12754f223e13
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333392"
---
# <a name="pendingoperations-resource-type"></a><span data-ttu-id="24d58-103">pendingOperations 资源类型</span><span class="sxs-lookup"><span data-stu-id="24d58-103">pendingOperations resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24d58-104">指示可能影响**driveItem**状态的一个或多个操作正在等待完成。</span><span class="sxs-lookup"><span data-stu-id="24d58-104">Indicates that one or more operations that might affect the state of the **driveItem** are pending completion.</span></span>

## <a name="properties"></a><span data-ttu-id="24d58-105">属性</span><span class="sxs-lookup"><span data-stu-id="24d58-105">Properties</span></span>

| <span data-ttu-id="24d58-106">属性</span><span class="sxs-lookup"><span data-stu-id="24d58-106">Property</span></span>     | <span data-ttu-id="24d58-107">类型</span><span class="sxs-lookup"><span data-stu-id="24d58-107">Type</span></span>        | <span data-ttu-id="24d58-108">说明</span><span class="sxs-lookup"><span data-stu-id="24d58-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="24d58-109">pendingContentUpdate</span><span class="sxs-lookup"><span data-stu-id="24d58-109">pendingContentUpdate</span></span>|[<span data-ttu-id="24d58-110">pendingContentUpdate</span><span class="sxs-lookup"><span data-stu-id="24d58-110">pendingContentUpdate</span></span>](pendingcontentupdate.md)|<span data-ttu-id="24d58-111">一个属性，指示可能更新文件二进制内容的操作正在等待完成。</span><span class="sxs-lookup"><span data-stu-id="24d58-111">A property that indicates that an operation that might update the binary content of a file is pending completion.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="24d58-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24d58-112">JSON representation</span></span>

<span data-ttu-id="24d58-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24d58-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pendingOperations",
  "baseType": null
}-->

```json
{
  "pendingContentUpdate": {"@odata.type": "microsoft.graph.pendingContentUpdate"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The pendingOperations resource indicates that an operation that may affect the state of the DriveItem is pending completion.",
  "keywords": "pendingoperations,pendingoperations,operation,pendingcontentupdate",
  "section": "documentation",
  "tocPath": ""
}-->
