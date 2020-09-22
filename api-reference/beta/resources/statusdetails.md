---
title: statusDetails 资源类型
description: 描述设置事件的状态和关联的错误。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 16f014ebc3a188644784434a69e13917f05beaae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029020"
---
# <a name="statusdetails-resource-type"></a><span data-ttu-id="14822-103">statusDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="14822-103">statusDetails resource type</span></span>

<span data-ttu-id="14822-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14822-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14822-105">描述设置事件的状态和关联的错误。</span><span class="sxs-lookup"><span data-stu-id="14822-105">Describes the status of the provisioning event and the associated errors.</span></span> <span data-ttu-id="14822-106">它是从 [statusBase](/graph/api/resources/statusbase?view=graph-rest-beta) 继承的，仅在将状态设置为 "失败" 时使用。</span><span class="sxs-lookup"><span data-stu-id="14822-106">It is inherited from [statusBase](/graph/api/resources/statusbase?view=graph-rest-beta) and only used when status is set to 'failure'.</span></span>  

## <a name="properties"></a><span data-ttu-id="14822-107">属性</span><span class="sxs-lookup"><span data-stu-id="14822-107">Properties</span></span>

| <span data-ttu-id="14822-108">属性</span><span class="sxs-lookup"><span data-stu-id="14822-108">Property</span></span>     | <span data-ttu-id="14822-109">类型</span><span class="sxs-lookup"><span data-stu-id="14822-109">Type</span></span>        | <span data-ttu-id="14822-110">说明</span><span class="sxs-lookup"><span data-stu-id="14822-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="14822-111">状态</span><span class="sxs-lookup"><span data-stu-id="14822-111">status</span></span>|<span data-ttu-id="14822-112">String</span><span class="sxs-lookup"><span data-stu-id="14822-112">String</span></span>|<span data-ttu-id="14822-113">可能的值是：`success`、`failure`、`skipped`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="14822-113">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span> <span data-ttu-id="14822-114">继承自 statusBase。</span><span class="sxs-lookup"><span data-stu-id="14822-114">Inherited from statusBase.</span></span>|
|<span data-ttu-id="14822-115">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="14822-115">additionalDetails</span></span>|<span data-ttu-id="14822-116">String</span><span class="sxs-lookup"><span data-stu-id="14822-116">String</span></span>|<span data-ttu-id="14822-117">发生错误时的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="14822-117">Additional details in case of error.</span></span>|
|<span data-ttu-id="14822-118">errorCategory</span><span class="sxs-lookup"><span data-stu-id="14822-118">errorCategory</span></span>|<span data-ttu-id="14822-119">String</span><span class="sxs-lookup"><span data-stu-id="14822-119">String</span></span>|<span data-ttu-id="14822-120">对错误代码进行分类。</span><span class="sxs-lookup"><span data-stu-id="14822-120">Categorizes the error code.</span></span>|
|<span data-ttu-id="14822-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="14822-121">errorCode</span></span>|<span data-ttu-id="14822-122">String</span><span class="sxs-lookup"><span data-stu-id="14822-122">String</span></span>|<span data-ttu-id="14822-123">出现的唯一错误代码。</span><span class="sxs-lookup"><span data-stu-id="14822-123">Unique error code if any occurred.</span></span>|
|<span data-ttu-id="14822-124">reason</span><span class="sxs-lookup"><span data-stu-id="14822-124">reason</span></span>|<span data-ttu-id="14822-125">String</span><span class="sxs-lookup"><span data-stu-id="14822-125">String</span></span>|<span data-ttu-id="14822-126">概述状态并介绍状态发生的原因。</span><span class="sxs-lookup"><span data-stu-id="14822-126">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="14822-127">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="14822-127">recommendedAction</span></span>|<span data-ttu-id="14822-128">String</span><span class="sxs-lookup"><span data-stu-id="14822-128">String</span></span>|<span data-ttu-id="14822-129">提供对应错误的解决方案。</span><span class="sxs-lookup"><span data-stu-id="14822-129">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14822-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14822-130">JSON representation</span></span>

<span data-ttu-id="14822-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14822-131">The following is a JSON representation of the resource.</span></span>

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


