---
title: statusDetails 资源类型
description: 描述设置事件的状态和关联的错误。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d3c22e67af690a28bb974a0334af7891f0c25cfb
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349349"
---
# <a name="statusdetails-resource-type"></a><span data-ttu-id="a83b2-103">statusDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="a83b2-103">statusDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a83b2-104">描述设置事件的状态和关联的错误。</span><span class="sxs-lookup"><span data-stu-id="a83b2-104">Describes the status of the provisioning event and the associated errors.</span></span> <span data-ttu-id="a83b2-105">它是从[statusBase](/graph/api/resources/statusBase?view=graph-rest-beta)继承的, 仅在将状态设置为 "失败" 时使用。</span><span class="sxs-lookup"><span data-stu-id="a83b2-105">It is inherited from [statusBase](/graph/api/resources/statusBase?view=graph-rest-beta) and only used when status is set to 'failure'.</span></span>  

## <a name="properties"></a><span data-ttu-id="a83b2-106">属性</span><span class="sxs-lookup"><span data-stu-id="a83b2-106">Properties</span></span>

| <span data-ttu-id="a83b2-107">属性</span><span class="sxs-lookup"><span data-stu-id="a83b2-107">Property</span></span>     | <span data-ttu-id="a83b2-108">类型</span><span class="sxs-lookup"><span data-stu-id="a83b2-108">Type</span></span>        | <span data-ttu-id="a83b2-109">说明</span><span class="sxs-lookup"><span data-stu-id="a83b2-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a83b2-110">status</span><span class="sxs-lookup"><span data-stu-id="a83b2-110">status</span></span>|<span data-ttu-id="a83b2-111">String</span><span class="sxs-lookup"><span data-stu-id="a83b2-111">String</span></span>|<span data-ttu-id="a83b2-112">可能的值是：`success`、`failure`、`skipped`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="a83b2-112">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span> <span data-ttu-id="a83b2-113">继承自 statusBase。</span><span class="sxs-lookup"><span data-stu-id="a83b2-113">Inherited from statusBase.</span></span>|
|<span data-ttu-id="a83b2-114">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="a83b2-114">additionalDetails</span></span>|<span data-ttu-id="a83b2-115">String</span><span class="sxs-lookup"><span data-stu-id="a83b2-115">String</span></span>|<span data-ttu-id="a83b2-116">发生错误时的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="a83b2-116">Additional details in case of error.</span></span>|
|<span data-ttu-id="a83b2-117">errorCategory</span><span class="sxs-lookup"><span data-stu-id="a83b2-117">errorCategory</span></span>|<span data-ttu-id="a83b2-118">String</span><span class="sxs-lookup"><span data-stu-id="a83b2-118">String</span></span>|<span data-ttu-id="a83b2-119">对错误代码进行分类。</span><span class="sxs-lookup"><span data-stu-id="a83b2-119">Categorizes the error code.</span></span>|
|<span data-ttu-id="a83b2-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="a83b2-120">errorCode</span></span>|<span data-ttu-id="a83b2-121">String</span><span class="sxs-lookup"><span data-stu-id="a83b2-121">String</span></span>|<span data-ttu-id="a83b2-122">出现的唯一错误代码。</span><span class="sxs-lookup"><span data-stu-id="a83b2-122">Unique error code if any occurred.</span></span>|
|<span data-ttu-id="a83b2-123">在于</span><span class="sxs-lookup"><span data-stu-id="a83b2-123">reason</span></span>|<span data-ttu-id="a83b2-124">String</span><span class="sxs-lookup"><span data-stu-id="a83b2-124">String</span></span>|<span data-ttu-id="a83b2-125">概述状态并介绍状态发生的原因。</span><span class="sxs-lookup"><span data-stu-id="a83b2-125">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="a83b2-126">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="a83b2-126">recommendedAction</span></span>|<span data-ttu-id="a83b2-127">String</span><span class="sxs-lookup"><span data-stu-id="a83b2-127">String</span></span>|<span data-ttu-id="a83b2-128">提供对应错误的解决方案。</span><span class="sxs-lookup"><span data-stu-id="a83b2-128">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a83b2-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a83b2-129">JSON representation</span></span>

<span data-ttu-id="a83b2-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a83b2-130">The following is a JSON representation of the resource.</span></span>

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
