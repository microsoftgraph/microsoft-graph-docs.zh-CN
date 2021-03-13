---
title: statusBase 资源类型
description: 描述预配摘要事件的状态。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 951ef56ecbe2ff8c2ab9692e4eaa9ddf7811d959
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761021"
---
# <a name="statusbase-resource-type"></a><span data-ttu-id="a2706-103">statusBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="a2706-103">statusBase resource type</span></span>

<span data-ttu-id="a2706-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2706-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2706-105">描述预配摘要事件的状态。</span><span class="sxs-lookup"><span data-stu-id="a2706-105">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="a2706-106">属性</span><span class="sxs-lookup"><span data-stu-id="a2706-106">Properties</span></span>

| <span data-ttu-id="a2706-107">属性</span><span class="sxs-lookup"><span data-stu-id="a2706-107">Property</span></span>     | <span data-ttu-id="a2706-108">类型</span><span class="sxs-lookup"><span data-stu-id="a2706-108">Type</span></span>        | <span data-ttu-id="a2706-109">说明</span><span class="sxs-lookup"><span data-stu-id="a2706-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a2706-110">状态</span><span class="sxs-lookup"><span data-stu-id="a2706-110">status</span></span>|<span data-ttu-id="a2706-111">String</span><span class="sxs-lookup"><span data-stu-id="a2706-111">String</span></span>| <span data-ttu-id="a2706-112">可取值为：`success`、`warning`、`failure`、`skipped`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="a2706-112">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2706-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a2706-113">JSON representation</span></span>

<span data-ttu-id="a2706-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2706-114">The following is a JSON representation of the resource.</span></span>

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


