---
title: provisioningErrorInfo 资源类型
description: 描述设置事件的状态和相关错误。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: dddddfa793cf9aac7436fc85e0ce911df7b4ec3e
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546964"
---
# <a name="provisioningerrorinfo-resource-type"></a><span data-ttu-id="982d6-103">provisioningErrorInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="982d6-103">provisioningErrorInfo resource type</span></span>

<span data-ttu-id="982d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="982d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="982d6-105">描述设置事件的状态和相关错误。</span><span class="sxs-lookup"><span data-stu-id="982d6-105">Describes the status of the provisioning event and the associated errors.</span></span> 

## <a name="properties"></a><span data-ttu-id="982d6-106">属性</span><span class="sxs-lookup"><span data-stu-id="982d6-106">Properties</span></span>

| <span data-ttu-id="982d6-107">属性</span><span class="sxs-lookup"><span data-stu-id="982d6-107">Property</span></span>     | <span data-ttu-id="982d6-108">类型</span><span class="sxs-lookup"><span data-stu-id="982d6-108">Type</span></span>        | <span data-ttu-id="982d6-109">说明</span><span class="sxs-lookup"><span data-stu-id="982d6-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="982d6-110">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="982d6-110">additionalDetails</span></span>|<span data-ttu-id="982d6-111">String</span><span class="sxs-lookup"><span data-stu-id="982d6-111">String</span></span>|<span data-ttu-id="982d6-112">出现错误时的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="982d6-112">Additional details in case of error.</span></span>|
|<span data-ttu-id="982d6-113">errorCategory</span><span class="sxs-lookup"><span data-stu-id="982d6-113">errorCategory</span></span>|<span data-ttu-id="982d6-114">String</span><span class="sxs-lookup"><span data-stu-id="982d6-114">String</span></span>|<span data-ttu-id="982d6-115">对错误代码进行分类。</span><span class="sxs-lookup"><span data-stu-id="982d6-115">Categorizes the error code.</span></span> <span data-ttu-id="982d6-116">可能的值是 `failure` `nonServiceFailure` `success` 、、、、 `unknownFutureValue`</span><span class="sxs-lookup"><span data-stu-id="982d6-116">Possible values are `failure`, `nonServiceFailure`, `success`, `unknownFutureValue`</span></span>|
|<span data-ttu-id="982d6-117">errorCode</span><span class="sxs-lookup"><span data-stu-id="982d6-117">errorCode</span></span>|<span data-ttu-id="982d6-118">String</span><span class="sxs-lookup"><span data-stu-id="982d6-118">String</span></span>|<span data-ttu-id="982d6-119">发生任何错误时的唯一错误代码。</span><span class="sxs-lookup"><span data-stu-id="982d6-119">Unique error code if any occurred.</span></span> [<span data-ttu-id="982d6-120">了解详细信息</span><span class="sxs-lookup"><span data-stu-id="982d6-120">Learn more</span></span>](/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|<span data-ttu-id="982d6-121">reason</span><span class="sxs-lookup"><span data-stu-id="982d6-121">reason</span></span>|<span data-ttu-id="982d6-122">String</span><span class="sxs-lookup"><span data-stu-id="982d6-122">String</span></span>|<span data-ttu-id="982d6-123">总结状态并说明状态发生的原因。</span><span class="sxs-lookup"><span data-stu-id="982d6-123">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="982d6-124">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="982d6-124">recommendedAction</span></span>|<span data-ttu-id="982d6-125">String</span><span class="sxs-lookup"><span data-stu-id="982d6-125">String</span></span>|<span data-ttu-id="982d6-126">提供相应错误的解决方法。</span><span class="sxs-lookup"><span data-stu-id="982d6-126">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="982d6-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="982d6-127">JSON representation</span></span>

<span data-ttu-id="982d6-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="982d6-128">The following is a JSON representation of the resource.</span></span>

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


