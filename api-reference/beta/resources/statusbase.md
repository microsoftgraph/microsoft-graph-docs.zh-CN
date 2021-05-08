---
title: statusBase 资源类型
description: 描述预配摘要事件的状态。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3e100c1b86c8d299a7d74431715a6e9ef1464393
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231974"
---
# <a name="statusbase-resource-type-deprecated"></a><span data-ttu-id="7a146-103">statusBase 资源类型 (已弃) </span><span class="sxs-lookup"><span data-stu-id="7a146-103">statusBase resource type (deprecated)</span></span>

<span data-ttu-id="7a146-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a146-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
>[!CAUTION] 
> <span data-ttu-id="7a146-105">statusBase API 已弃用，并将于 2021 年 12 月 31 日停止返回数据。</span><span class="sxs-lookup"><span data-stu-id="7a146-105">The statusBase API is deprecated and will stop returning data om December 31, 2021.</span></span> <span data-ttu-id="7a146-106">请使用新的 [provisioningStatusInfo](provisioningstatusinfo.md) 类型。</span><span class="sxs-lookup"><span data-stu-id="7a146-106">Please use the new [provisioningStatusInfo](provisioningstatusinfo.md) type.</span></span>

<span data-ttu-id="7a146-107">描述预配摘要事件的状态。</span><span class="sxs-lookup"><span data-stu-id="7a146-107">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="7a146-108">属性</span><span class="sxs-lookup"><span data-stu-id="7a146-108">Properties</span></span>

| <span data-ttu-id="7a146-109">属性</span><span class="sxs-lookup"><span data-stu-id="7a146-109">Property</span></span>     | <span data-ttu-id="7a146-110">类型</span><span class="sxs-lookup"><span data-stu-id="7a146-110">Type</span></span>        | <span data-ttu-id="7a146-111">说明</span><span class="sxs-lookup"><span data-stu-id="7a146-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7a146-112">状态</span><span class="sxs-lookup"><span data-stu-id="7a146-112">status</span></span>|<span data-ttu-id="7a146-113">provisioningResult</span><span class="sxs-lookup"><span data-stu-id="7a146-113">provisioningResult</span></span>| <span data-ttu-id="7a146-114">可取值为：`success`、`warning`、`failure`、`skipped`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="7a146-114">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a146-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a146-115">JSON representation</span></span>

<span data-ttu-id="7a146-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a146-116">The following is a JSON representation of the resource.</span></span>

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


