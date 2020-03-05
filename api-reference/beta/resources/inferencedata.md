---
title: inferenceData 资源类型
description: inferenceData 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: profile
doc_type: resourcePageType
ms.openlocfilehash: 2097dc14de984f3d1517b4d17e8043f38411b89a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496171"
---
# <a name="inferencedata-resource-type"></a><span data-ttu-id="ba662-103">inferenceData 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba662-103">inferenceData resource type</span></span>

<span data-ttu-id="ba662-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ba662-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba662-105">[InferenceData](inferencedata.md)资源类型提供了有关通过推断用户信息创建的实体的附加详细信息。</span><span class="sxs-lookup"><span data-stu-id="ba662-105">The [inferenceData](inferencedata.md) resource type provides additional detail about an entity which has been created through inferring information about the user.</span></span> <span data-ttu-id="ba662-106">只要特定实体中的数据是由机器学习或其他系统进程对数据进行迭代时，就会出现此信息。</span><span class="sxs-lookup"><span data-stu-id="ba662-106">This information will be present whenever the data within a particular entity was derived from a machine learning or other system process iterating over data.</span></span>

## <a name="properties"></a><span data-ttu-id="ba662-107">属性</span><span class="sxs-lookup"><span data-stu-id="ba662-107">Properties</span></span>

| <span data-ttu-id="ba662-108">属性</span><span class="sxs-lookup"><span data-stu-id="ba662-108">Property</span></span>              | <span data-ttu-id="ba662-109">类型</span><span class="sxs-lookup"><span data-stu-id="ba662-109">Type</span></span>        | <span data-ttu-id="ba662-110">说明</span><span class="sxs-lookup"><span data-stu-id="ba662-110">Description</span></span>                                                                     |
|:----------------------|:------------|:--------------------------------------------------------------------------------|
|<span data-ttu-id="ba662-111">confidenceScore</span><span class="sxs-lookup"><span data-stu-id="ba662-111">confidenceScore</span></span>        |<span data-ttu-id="ba662-112">双精度</span><span class="sxs-lookup"><span data-stu-id="ba662-112">Double</span></span>       | <span data-ttu-id="ba662-113">反映有关用户推断的数据准确性的置信度分数。</span><span class="sxs-lookup"><span data-stu-id="ba662-113">Confidence score reflecting the accuracy of the data inferred about the user.</span></span>   |
|<span data-ttu-id="ba662-114">userHasVerifiedAccuracy</span><span class="sxs-lookup"><span data-stu-id="ba662-114">userHasVerifiedAccuracy</span></span>|<span data-ttu-id="ba662-115">布尔</span><span class="sxs-lookup"><span data-stu-id="ba662-115">Boolean</span></span>      | <span data-ttu-id="ba662-116">如果用户已确认此推理为 True 或 False，则为记录。</span><span class="sxs-lookup"><span data-stu-id="ba662-116">Records if the user has confirmed this inference as being True or False.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="ba662-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba662-117">JSON representation</span></span>

<span data-ttu-id="ba662-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba662-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceData",
  "baseType": null
}-->

```json
{
  "confidenceScore": 1024,
  "userHasVerifiedAccuracy": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->