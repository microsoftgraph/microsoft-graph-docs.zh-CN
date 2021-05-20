---
title: statusDetails 资源类型
description: 描述设置事件的状态和相关错误。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: e3333ac030ec08722ad6bcaa58a153fc961469cf
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546903"
---
# <a name="statusdetails-resource-type-deprecated"></a><span data-ttu-id="79fb4-103">statusDetails 资源类型 (已弃) </span><span class="sxs-lookup"><span data-stu-id="79fb4-103">statusDetails resource type (deprecated)</span></span>

<span data-ttu-id="79fb4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79fb4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
>[!CAUTION] 
> <span data-ttu-id="79fb4-105">statusDetails API 已弃用，并将于 2021 年 12 月 31 日停止返回数据。</span><span class="sxs-lookup"><span data-stu-id="79fb4-105">The statusDetails API is deprecated and will stop returning data om December 31, 2021.</span></span> <span data-ttu-id="79fb4-106">请使用新的 [provisioningStatusInfo](provisioningstatusinfo.md) 类型。</span><span class="sxs-lookup"><span data-stu-id="79fb4-106">Please use the new [provisioningStatusInfo](provisioningstatusinfo.md) type.</span></span>

<span data-ttu-id="79fb4-107">描述设置事件的状态和相关错误。</span><span class="sxs-lookup"><span data-stu-id="79fb4-107">Describes the status of the provisioning event and the associated errors.</span></span> <span data-ttu-id="79fb4-108">它继承自 [statusBase，](/graph/api/resources/statusbase) 并且仅在 status 设置为 时使用 `failure` 。</span><span class="sxs-lookup"><span data-stu-id="79fb4-108">It is inherited from [statusBase](/graph/api/resources/statusbase) and only used when status is set to `failure`.</span></span>  

## <a name="properties"></a><span data-ttu-id="79fb4-109">属性</span><span class="sxs-lookup"><span data-stu-id="79fb4-109">Properties</span></span>

| <span data-ttu-id="79fb4-110">属性</span><span class="sxs-lookup"><span data-stu-id="79fb4-110">Property</span></span>     | <span data-ttu-id="79fb4-111">类型</span><span class="sxs-lookup"><span data-stu-id="79fb4-111">Type</span></span>        | <span data-ttu-id="79fb4-112">说明</span><span class="sxs-lookup"><span data-stu-id="79fb4-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="79fb4-113">状态</span><span class="sxs-lookup"><span data-stu-id="79fb4-113">status</span></span>|<span data-ttu-id="79fb4-114">statusBase</span><span class="sxs-lookup"><span data-stu-id="79fb4-114">statusBase</span></span>|<span data-ttu-id="79fb4-115">可取值为：`success`、`warning`、`failure`、`skipped`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="79fb4-115">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span> <span data-ttu-id="79fb4-116">继承自 statusBase。</span><span class="sxs-lookup"><span data-stu-id="79fb4-116">Inherited from statusBase.</span></span>|
|<span data-ttu-id="79fb4-117">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="79fb4-117">additionalDetails</span></span>|<span data-ttu-id="79fb4-118">String</span><span class="sxs-lookup"><span data-stu-id="79fb4-118">String</span></span>|<span data-ttu-id="79fb4-119">出现错误时的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="79fb4-119">Additional details in case of error.</span></span>|
|<span data-ttu-id="79fb4-120">errorCategory</span><span class="sxs-lookup"><span data-stu-id="79fb4-120">errorCategory</span></span>|<span data-ttu-id="79fb4-121">String</span><span class="sxs-lookup"><span data-stu-id="79fb4-121">String</span></span>|<span data-ttu-id="79fb4-122">对错误代码进行分类。</span><span class="sxs-lookup"><span data-stu-id="79fb4-122">Categorizes the error code.</span></span> <span data-ttu-id="79fb4-123">可取值为 `Failure`、`NonServiceFailure`、`Success`。</span><span class="sxs-lookup"><span data-stu-id="79fb4-123">Possible values are `Failure`, `NonServiceFailure`, `Success`.</span></span>|
|<span data-ttu-id="79fb4-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="79fb4-124">errorCode</span></span>|<span data-ttu-id="79fb4-125">String</span><span class="sxs-lookup"><span data-stu-id="79fb4-125">String</span></span>|<span data-ttu-id="79fb4-126">发生任何错误时的唯一错误代码。</span><span class="sxs-lookup"><span data-stu-id="79fb4-126">Unique error code if any occurred.</span></span> [<span data-ttu-id="79fb4-127">了解详细信息</span><span class="sxs-lookup"><span data-stu-id="79fb4-127">Learn more</span></span>](/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|<span data-ttu-id="79fb4-128">reason</span><span class="sxs-lookup"><span data-stu-id="79fb4-128">reason</span></span>|<span data-ttu-id="79fb4-129">String</span><span class="sxs-lookup"><span data-stu-id="79fb4-129">String</span></span>|<span data-ttu-id="79fb4-130">总结状态并说明状态发生的原因。</span><span class="sxs-lookup"><span data-stu-id="79fb4-130">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="79fb4-131">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="79fb4-131">recommendedAction</span></span>|<span data-ttu-id="79fb4-132">String</span><span class="sxs-lookup"><span data-stu-id="79fb4-132">String</span></span>|<span data-ttu-id="79fb4-133">提供相应错误的解决方法。</span><span class="sxs-lookup"><span data-stu-id="79fb4-133">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="79fb4-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="79fb4-134">JSON representation</span></span>

<span data-ttu-id="79fb4-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79fb4-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.statusDetails",
  "baseType": "microsoft.graph.statusBase"
}-->

```json
{
  "status": "failure",
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
  "description": "statusDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


