---
title: provisioningStatusInfo 资源类型
description: 描述预配摘要事件的状态。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 669201b5527160da6b903614523d633a8c11cb1d
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232916"
---
# <a name="provisioningstatusinfo-resource-type"></a><span data-ttu-id="44dac-103">provisioningStatusInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="44dac-103">provisioningStatusInfo resource type</span></span>

<span data-ttu-id="44dac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44dac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44dac-105">描述预配摘要事件的状态。</span><span class="sxs-lookup"><span data-stu-id="44dac-105">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="44dac-106">属性</span><span class="sxs-lookup"><span data-stu-id="44dac-106">Properties</span></span>

| <span data-ttu-id="44dac-107">属性</span><span class="sxs-lookup"><span data-stu-id="44dac-107">Property</span></span>     | <span data-ttu-id="44dac-108">类型</span><span class="sxs-lookup"><span data-stu-id="44dac-108">Type</span></span>        | <span data-ttu-id="44dac-109">说明</span><span class="sxs-lookup"><span data-stu-id="44dac-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="44dac-110">状态</span><span class="sxs-lookup"><span data-stu-id="44dac-110">status</span></span>|<span data-ttu-id="44dac-111">String</span><span class="sxs-lookup"><span data-stu-id="44dac-111">String</span></span>| <span data-ttu-id="44dac-112">可取值为：`success`、`warning`、`failure`、`skipped`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="44dac-112">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="44dac-113">errorInfo</span><span class="sxs-lookup"><span data-stu-id="44dac-113">errorInfo</span></span>|[<span data-ttu-id="44dac-114">provisioningErrorInfo</span><span class="sxs-lookup"><span data-stu-id="44dac-114">provisioningErrorInfo</span></span>](provisioningerrorinfo.md)| <span data-ttu-id="44dac-115">如果状态未成功/跳过错误的详细信息将包含在其中。</span><span class="sxs-lookup"><span data-stu-id="44dac-115">If status is not success/ skipped details for the error are contained in this.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44dac-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44dac-116">JSON representation</span></span>

<span data-ttu-id="44dac-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44dac-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningStatusInfo",
  "baseType": null
}-->

```json
{
  "status": "String",
  "errorinfo": {"@odata.type": "microsoft.graph.provisioningErrorInfo"},}
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


