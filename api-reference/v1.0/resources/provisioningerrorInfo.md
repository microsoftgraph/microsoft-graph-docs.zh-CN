---
title: provisioningErrorInfo 资源类型
description: 描述设置事件的状态和相关错误。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d22d68b7c040ea07e6aef2cc0f606bd378b3b47c
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241496"
---
# <a name="provisioningerrorinfo-resource-type"></a><span data-ttu-id="af862-103">provisioningErrorInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="af862-103">provisioningErrorInfo resource type</span></span>

<span data-ttu-id="af862-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af862-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="af862-105">描述设置事件的状态和相关错误。</span><span class="sxs-lookup"><span data-stu-id="af862-105">Describes the status of the provisioning event and the associated errors.</span></span> 

## <a name="properties"></a><span data-ttu-id="af862-106">属性</span><span class="sxs-lookup"><span data-stu-id="af862-106">Properties</span></span>

| <span data-ttu-id="af862-107">属性</span><span class="sxs-lookup"><span data-stu-id="af862-107">Property</span></span>     | <span data-ttu-id="af862-108">类型</span><span class="sxs-lookup"><span data-stu-id="af862-108">Type</span></span>        | <span data-ttu-id="af862-109">说明</span><span class="sxs-lookup"><span data-stu-id="af862-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="af862-110">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="af862-110">additionalDetails</span></span>|<span data-ttu-id="af862-111">String</span><span class="sxs-lookup"><span data-stu-id="af862-111">String</span></span>|<span data-ttu-id="af862-112">出现错误时的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="af862-112">Additional details in case of error.</span></span>|
|<span data-ttu-id="af862-113">errorCategory</span><span class="sxs-lookup"><span data-stu-id="af862-113">errorCategory</span></span>|<span data-ttu-id="af862-114">provisioningStatusErrorCategory</span><span class="sxs-lookup"><span data-stu-id="af862-114">provisioningStatusErrorCategory</span></span>|<span data-ttu-id="af862-115">对错误代码进行分类。</span><span class="sxs-lookup"><span data-stu-id="af862-115">Categorizes the error code.</span></span> <span data-ttu-id="af862-116">可能的值是 `failure` `nonServiceFailure` `success` 、、、、 `unknownFutureValue`</span><span class="sxs-lookup"><span data-stu-id="af862-116">Possible values are `failure`, `nonServiceFailure`, `success`, `unknownFutureValue`</span></span>|
|<span data-ttu-id="af862-117">errorCode</span><span class="sxs-lookup"><span data-stu-id="af862-117">errorCode</span></span>|<span data-ttu-id="af862-118">String</span><span class="sxs-lookup"><span data-stu-id="af862-118">String</span></span>|<span data-ttu-id="af862-119">发生任何错误时的唯一错误代码。</span><span class="sxs-lookup"><span data-stu-id="af862-119">Unique error code if any occurred.</span></span> [<span data-ttu-id="af862-120">了解更多</span><span class="sxs-lookup"><span data-stu-id="af862-120">Learn more</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|<span data-ttu-id="af862-121">reason</span><span class="sxs-lookup"><span data-stu-id="af862-121">reason</span></span>|<span data-ttu-id="af862-122">String</span><span class="sxs-lookup"><span data-stu-id="af862-122">String</span></span>|<span data-ttu-id="af862-123">总结状态并说明状态发生的原因。</span><span class="sxs-lookup"><span data-stu-id="af862-123">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="af862-124">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="af862-124">recommendedAction</span></span>|<span data-ttu-id="af862-125">String</span><span class="sxs-lookup"><span data-stu-id="af862-125">String</span></span>|<span data-ttu-id="af862-126">提供相应错误的解决方法。</span><span class="sxs-lookup"><span data-stu-id="af862-126">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="af862-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af862-127">JSON representation</span></span>

<span data-ttu-id="af862-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af862-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningErrorInfo",
  "baseType": null
}-->

```json
{
  "additionalDetails": "String",
  "errorCategory": "String",
  "errorCode": "String",
  "reason": "String",
  "recommendedAction": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningErrorInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


