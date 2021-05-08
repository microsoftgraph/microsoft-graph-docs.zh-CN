---
title: provisioningErrorInfo 资源类型
description: 描述设置事件的状态和相关错误。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 839370e0dc15ee247997b6d934107e27f62cc87a
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232949"
---
# <a name="provisioningerrorinfo-resource-type"></a><span data-ttu-id="486a3-103">provisioningErrorInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="486a3-103">provisioningErrorInfo resource type</span></span>

<span data-ttu-id="486a3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="486a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="486a3-105">描述设置事件的状态和相关错误。</span><span class="sxs-lookup"><span data-stu-id="486a3-105">Describes the status of the provisioning event and the associated errors.</span></span> 

## <a name="properties"></a><span data-ttu-id="486a3-106">属性</span><span class="sxs-lookup"><span data-stu-id="486a3-106">Properties</span></span>

| <span data-ttu-id="486a3-107">属性</span><span class="sxs-lookup"><span data-stu-id="486a3-107">Property</span></span>     | <span data-ttu-id="486a3-108">类型</span><span class="sxs-lookup"><span data-stu-id="486a3-108">Type</span></span>        | <span data-ttu-id="486a3-109">说明</span><span class="sxs-lookup"><span data-stu-id="486a3-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="486a3-110">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="486a3-110">additionalDetails</span></span>|<span data-ttu-id="486a3-111">String</span><span class="sxs-lookup"><span data-stu-id="486a3-111">String</span></span>|<span data-ttu-id="486a3-112">出现错误时的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="486a3-112">Additional details in case of error.</span></span>|
|<span data-ttu-id="486a3-113">errorCategory</span><span class="sxs-lookup"><span data-stu-id="486a3-113">errorCategory</span></span>|<span data-ttu-id="486a3-114">String</span><span class="sxs-lookup"><span data-stu-id="486a3-114">String</span></span>|<span data-ttu-id="486a3-115">对错误代码进行分类。</span><span class="sxs-lookup"><span data-stu-id="486a3-115">Categorizes the error code.</span></span> <span data-ttu-id="486a3-116">可能的值是 `failure` `nonServiceFailure` `success` 、、、、 `unknownFutureValue`</span><span class="sxs-lookup"><span data-stu-id="486a3-116">Possible values are `failure`, `nonServiceFailure`, `success`, `unknownFutureValue`</span></span>|
|<span data-ttu-id="486a3-117">errorCode</span><span class="sxs-lookup"><span data-stu-id="486a3-117">errorCode</span></span>|<span data-ttu-id="486a3-118">String</span><span class="sxs-lookup"><span data-stu-id="486a3-118">String</span></span>|<span data-ttu-id="486a3-119">发生任何错误时的唯一错误代码。</span><span class="sxs-lookup"><span data-stu-id="486a3-119">Unique error code if any occurred.</span></span> [<span data-ttu-id="486a3-120">了解更多</span><span class="sxs-lookup"><span data-stu-id="486a3-120">Learn more</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|<span data-ttu-id="486a3-121">reason</span><span class="sxs-lookup"><span data-stu-id="486a3-121">reason</span></span>|<span data-ttu-id="486a3-122">String</span><span class="sxs-lookup"><span data-stu-id="486a3-122">String</span></span>|<span data-ttu-id="486a3-123">总结状态并说明状态发生的原因。</span><span class="sxs-lookup"><span data-stu-id="486a3-123">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="486a3-124">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="486a3-124">recommendedAction</span></span>|<span data-ttu-id="486a3-125">String</span><span class="sxs-lookup"><span data-stu-id="486a3-125">String</span></span>|<span data-ttu-id="486a3-126">提供相应错误的解决方法。</span><span class="sxs-lookup"><span data-stu-id="486a3-126">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="486a3-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="486a3-127">JSON representation</span></span>

<span data-ttu-id="486a3-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="486a3-128">The following is a JSON representation of the resource.</span></span>

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


