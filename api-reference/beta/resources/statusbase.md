---
title: statusBase 资源类型
description: 描述设置摘要事件的状态。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ee205db24cf8591725ca7d9fc3c4a0fe8c72489e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067102"
---
# <a name="statusbase-resource-type"></a><span data-ttu-id="21a19-103">statusBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="21a19-103">statusBase resource type</span></span>

<span data-ttu-id="21a19-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21a19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21a19-105">描述设置摘要事件的状态。</span><span class="sxs-lookup"><span data-stu-id="21a19-105">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="21a19-106">属性</span><span class="sxs-lookup"><span data-stu-id="21a19-106">Properties</span></span>

| <span data-ttu-id="21a19-107">属性</span><span class="sxs-lookup"><span data-stu-id="21a19-107">Property</span></span>     | <span data-ttu-id="21a19-108">类型</span><span class="sxs-lookup"><span data-stu-id="21a19-108">Type</span></span>        | <span data-ttu-id="21a19-109">说明</span><span class="sxs-lookup"><span data-stu-id="21a19-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="21a19-110">状态</span><span class="sxs-lookup"><span data-stu-id="21a19-110">status</span></span>|<span data-ttu-id="21a19-111">String</span><span class="sxs-lookup"><span data-stu-id="21a19-111">String</span></span>| <span data-ttu-id="21a19-112">可能的值是：`success`、`failure`、`skipped`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="21a19-112">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21a19-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="21a19-113">JSON representation</span></span>

<span data-ttu-id="21a19-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21a19-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.statusBase",
  "baseType": null
}-->

```json
{
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "statusBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


