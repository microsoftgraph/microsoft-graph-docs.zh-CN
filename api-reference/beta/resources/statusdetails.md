---
title: statusDetails 资源类型
description: 描述设置事件的状态和相关错误。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: d817c0aa46dde6b49debd849d8fd2ae61e06a672
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956818"
---
# <a name="statusdetails-resource-type"></a><span data-ttu-id="17789-103">statusDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="17789-103">statusDetails resource type</span></span>

<span data-ttu-id="17789-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17789-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17789-105">描述设置事件的状态和相关错误。</span><span class="sxs-lookup"><span data-stu-id="17789-105">Describes the status of the provisioning event and the associated errors.</span></span> <span data-ttu-id="17789-106">它继承自 [statusBase，](/graph/api/resources/statusbase) 并且仅在 status 设置为 时使用 `failure` 。</span><span class="sxs-lookup"><span data-stu-id="17789-106">It is inherited from [statusBase](/graph/api/resources/statusbase) and only used when status is set to `failure`.</span></span>  

## <a name="properties"></a><span data-ttu-id="17789-107">属性</span><span class="sxs-lookup"><span data-stu-id="17789-107">Properties</span></span>

| <span data-ttu-id="17789-108">属性</span><span class="sxs-lookup"><span data-stu-id="17789-108">Property</span></span>     | <span data-ttu-id="17789-109">类型</span><span class="sxs-lookup"><span data-stu-id="17789-109">Type</span></span>        | <span data-ttu-id="17789-110">说明</span><span class="sxs-lookup"><span data-stu-id="17789-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="17789-111">状态</span><span class="sxs-lookup"><span data-stu-id="17789-111">status</span></span>|<span data-ttu-id="17789-112">statusBase</span><span class="sxs-lookup"><span data-stu-id="17789-112">statusBase</span></span>|<span data-ttu-id="17789-113">可取值为：`success`、`warning`、`failure`、`skipped`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="17789-113">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span> <span data-ttu-id="17789-114">继承自 statusBase。</span><span class="sxs-lookup"><span data-stu-id="17789-114">Inherited from statusBase.</span></span>|
|<span data-ttu-id="17789-115">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="17789-115">additionalDetails</span></span>|<span data-ttu-id="17789-116">String</span><span class="sxs-lookup"><span data-stu-id="17789-116">String</span></span>|<span data-ttu-id="17789-117">出现错误时的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="17789-117">Additional details in case of error.</span></span>|
|<span data-ttu-id="17789-118">errorCategory</span><span class="sxs-lookup"><span data-stu-id="17789-118">errorCategory</span></span>|<span data-ttu-id="17789-119">String</span><span class="sxs-lookup"><span data-stu-id="17789-119">String</span></span>|<span data-ttu-id="17789-120">对错误代码进行分类。</span><span class="sxs-lookup"><span data-stu-id="17789-120">Categorizes the error code.</span></span> <span data-ttu-id="17789-121">可取值为 `Failure`、`NonServiceFailure`、`Success`。</span><span class="sxs-lookup"><span data-stu-id="17789-121">Possible values are `Failure`, `NonServiceFailure`, `Success`.</span></span>|
|<span data-ttu-id="17789-122">errorCode</span><span class="sxs-lookup"><span data-stu-id="17789-122">errorCode</span></span>|<span data-ttu-id="17789-123">String</span><span class="sxs-lookup"><span data-stu-id="17789-123">String</span></span>|<span data-ttu-id="17789-124">发生任何错误时的唯一错误代码。</span><span class="sxs-lookup"><span data-stu-id="17789-124">Unique error code if any occurred.</span></span> [<span data-ttu-id="17789-125">了解更多</span><span class="sxs-lookup"><span data-stu-id="17789-125">Learn more</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|<span data-ttu-id="17789-126">reason</span><span class="sxs-lookup"><span data-stu-id="17789-126">reason</span></span>|<span data-ttu-id="17789-127">String</span><span class="sxs-lookup"><span data-stu-id="17789-127">String</span></span>|<span data-ttu-id="17789-128">总结状态并说明状态发生的原因。</span><span class="sxs-lookup"><span data-stu-id="17789-128">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="17789-129">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="17789-129">recommendedAction</span></span>|<span data-ttu-id="17789-130">String</span><span class="sxs-lookup"><span data-stu-id="17789-130">String</span></span>|<span data-ttu-id="17789-131">提供相应错误的解决方法。</span><span class="sxs-lookup"><span data-stu-id="17789-131">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="17789-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17789-132">JSON representation</span></span>

<span data-ttu-id="17789-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17789-133">The following is a JSON representation of the resource.</span></span>

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


