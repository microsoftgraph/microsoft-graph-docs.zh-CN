---
title: statusBase 资源类型
description: 描述设置摘要事件的状态。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5d655649f7e1edca4e269576c9bcb6d1f3014e89
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523026"
---
# <a name="statusbase-resource-type"></a><span data-ttu-id="2e69a-103">statusBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="2e69a-103">statusBase resource type</span></span>

<span data-ttu-id="2e69a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e69a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e69a-105">描述设置摘要事件的状态。</span><span class="sxs-lookup"><span data-stu-id="2e69a-105">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="2e69a-106">属性</span><span class="sxs-lookup"><span data-stu-id="2e69a-106">Properties</span></span>

| <span data-ttu-id="2e69a-107">属性</span><span class="sxs-lookup"><span data-stu-id="2e69a-107">Property</span></span>     | <span data-ttu-id="2e69a-108">类型</span><span class="sxs-lookup"><span data-stu-id="2e69a-108">Type</span></span>        | <span data-ttu-id="2e69a-109">说明</span><span class="sxs-lookup"><span data-stu-id="2e69a-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2e69a-110">status</span><span class="sxs-lookup"><span data-stu-id="2e69a-110">status</span></span>|<span data-ttu-id="2e69a-111">String</span><span class="sxs-lookup"><span data-stu-id="2e69a-111">String</span></span>| <span data-ttu-id="2e69a-112">可取值为：`success`、`warning`、`failure`、`skipped`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2e69a-112">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e69a-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2e69a-113">JSON representation</span></span>

<span data-ttu-id="2e69a-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e69a-114">The following is a JSON representation of the resource.</span></span>

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


