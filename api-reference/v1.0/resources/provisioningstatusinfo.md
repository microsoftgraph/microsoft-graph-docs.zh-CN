---
title: provisioningStatusInfo 资源类型
description: 描述预配摘要事件的状态。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 7b6ab84ab1139d2ec5d60e7d5c668d0444e472d3
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680967"
---
# <a name="provisioningstatusinfo-resource-type"></a><span data-ttu-id="c6aa4-103">provisioningStatusInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6aa4-103">provisioningStatusInfo resource type</span></span>

<span data-ttu-id="c6aa4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6aa4-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="c6aa4-105">描述预配摘要事件的状态。</span><span class="sxs-lookup"><span data-stu-id="c6aa4-105">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="c6aa4-106">属性</span><span class="sxs-lookup"><span data-stu-id="c6aa4-106">Properties</span></span>

| <span data-ttu-id="c6aa4-107">属性</span><span class="sxs-lookup"><span data-stu-id="c6aa4-107">Property</span></span>     | <span data-ttu-id="c6aa4-108">类型</span><span class="sxs-lookup"><span data-stu-id="c6aa4-108">Type</span></span>        | <span data-ttu-id="c6aa4-109">说明</span><span class="sxs-lookup"><span data-stu-id="c6aa4-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c6aa4-110">状态</span><span class="sxs-lookup"><span data-stu-id="c6aa4-110">status</span></span>|<span data-ttu-id="c6aa4-111">provisioningResult</span><span class="sxs-lookup"><span data-stu-id="c6aa4-111">provisioningResult</span></span>| <span data-ttu-id="c6aa4-112">可取值为：`success`、`warning`、`failure`、`skipped`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c6aa4-112">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c6aa4-113">errorInfo</span><span class="sxs-lookup"><span data-stu-id="c6aa4-113">errorInfo</span></span>|[<span data-ttu-id="c6aa4-114">provisioningErrorInfo</span><span class="sxs-lookup"><span data-stu-id="c6aa4-114">provisioningErrorInfo</span></span>](provisioningErrorInfo.md)| <span data-ttu-id="c6aa4-115">如果状态未成功/跳过错误的详细信息将包含在其中。</span><span class="sxs-lookup"><span data-stu-id="c6aa4-115">If status is not success/ skipped details for the error are contained in this.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c6aa4-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6aa4-116">JSON representation</span></span>

<span data-ttu-id="c6aa4-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6aa4-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningStatusInfo",
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
  "description": "provisioningStatusInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


