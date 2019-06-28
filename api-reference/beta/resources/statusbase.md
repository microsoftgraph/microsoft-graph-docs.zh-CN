---
title: statusBase 资源类型
description: 描述设置摘要事件的状态。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: de35e89b674130bb1f2896b299ba5f4efe3af099
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349357"
---
# <a name="statusbase-resource-type"></a><span data-ttu-id="24b6e-103">statusBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="24b6e-103">statusBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24b6e-104">描述设置摘要事件的状态。</span><span class="sxs-lookup"><span data-stu-id="24b6e-104">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="24b6e-105">属性</span><span class="sxs-lookup"><span data-stu-id="24b6e-105">Properties</span></span>

| <span data-ttu-id="24b6e-106">属性</span><span class="sxs-lookup"><span data-stu-id="24b6e-106">Property</span></span>     | <span data-ttu-id="24b6e-107">类型</span><span class="sxs-lookup"><span data-stu-id="24b6e-107">Type</span></span>        | <span data-ttu-id="24b6e-108">说明</span><span class="sxs-lookup"><span data-stu-id="24b6e-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="24b6e-109">status</span><span class="sxs-lookup"><span data-stu-id="24b6e-109">status</span></span>|<span data-ttu-id="24b6e-110">String</span><span class="sxs-lookup"><span data-stu-id="24b6e-110">String</span></span>| <span data-ttu-id="24b6e-111">可能的值是：`success`、`failure`、`skipped`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="24b6e-111">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="24b6e-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24b6e-112">JSON representation</span></span>

<span data-ttu-id="24b6e-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24b6e-113">The following is a JSON representation of the resource.</span></span>

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
