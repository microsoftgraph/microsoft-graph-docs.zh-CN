---
title: classificationResult 资源类型
description: 表示分类请求的结果。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 719ce6fa70172a3ab323aec8c991147ef212bcb7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016826"
---
# <a name="classificationresult-resource-type"></a><span data-ttu-id="d4934-103">classificationResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4934-103">classificationResult resource type</span></span>

<span data-ttu-id="d4934-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4934-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4934-105">表示来自 Microsoft 分类引擎的分类操作的结果。</span><span class="sxs-lookup"><span data-stu-id="d4934-105">Represents the result of a classification operation from the Microsoft Classification Engine.</span></span> <span data-ttu-id="d4934-106">来自 Azure 信息保护、Office 和其他 Microsoft 服务的数据分类结果可能会返回一 [组定义完善的分类类型](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)。</span><span class="sxs-lookup"><span data-stu-id="d4934-106">Data classification results from Azure Information Protection, Office, and other Microsoft services may return a [well-defined set of classification types](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span> <span data-ttu-id="d4934-107">可以向 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) API 提供这些类型，以将敏感信息解析为 Microsoft 信息保护标签。</span><span class="sxs-lookup"><span data-stu-id="d4934-107">These types can be provided to the [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) API to resolve a sensitive information to a Microsoft Information Protection label.</span></span> 

## <a name="properties"></a><span data-ttu-id="d4934-108">属性</span><span class="sxs-lookup"><span data-stu-id="d4934-108">Properties</span></span>

| <span data-ttu-id="d4934-109">属性</span><span class="sxs-lookup"><span data-stu-id="d4934-109">Property</span></span>        | <span data-ttu-id="d4934-110">类型</span><span class="sxs-lookup"><span data-stu-id="d4934-110">Type</span></span>  | <span data-ttu-id="d4934-111">说明</span><span class="sxs-lookup"><span data-stu-id="d4934-111">Description</span></span>                                                            |
| :-------------- | :---- | :--------------------------------------------------------------------- |
| <span data-ttu-id="d4934-112">confidenceLevel</span><span class="sxs-lookup"><span data-stu-id="d4934-112">confidenceLevel</span></span> | <span data-ttu-id="d4934-113">Int32</span><span class="sxs-lookup"><span data-stu-id="d4934-113">Int32</span></span> | <span data-ttu-id="d4934-114">结果的置信度（0到100）。</span><span class="sxs-lookup"><span data-stu-id="d4934-114">The confidence level, 0 to 100, of the result.</span></span>                         |
| <span data-ttu-id="d4934-115">count</span><span class="sxs-lookup"><span data-stu-id="d4934-115">count</span></span>           | <span data-ttu-id="d4934-116">Int32</span><span class="sxs-lookup"><span data-stu-id="d4934-116">Int32</span></span> | <span data-ttu-id="d4934-117">输入中特定信息类型的实例数。</span><span class="sxs-lookup"><span data-stu-id="d4934-117">The number of instances of the specific information type in the input.</span></span> |
| <span data-ttu-id="d4934-118">sensitiveTypeId</span><span class="sxs-lookup"><span data-stu-id="d4934-118">sensitiveTypeId</span></span> | <span data-ttu-id="d4934-119">GUID</span><span class="sxs-lookup"><span data-stu-id="d4934-119">GUID</span></span>  | <span data-ttu-id="d4934-120">发现的敏感信息类型的 GUID。</span><span class="sxs-lookup"><span data-stu-id="d4934-120">The GUID of the discovered sensitive information type.</span></span>                 |

## <a name="json-representation"></a><span data-ttu-id="d4934-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4934-121">JSON representation</span></span>

<span data-ttu-id="d4934-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4934-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.classificationResult",
  "baseType": null
}-->

```json
{
  "confidenceLevel": 1024,
  "count": 1024,
  "sensitiveTypeId": "Guid"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "classificationResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


