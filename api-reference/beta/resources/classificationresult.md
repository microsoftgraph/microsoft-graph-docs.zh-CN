---
title: classificationResult 资源类型
description: 表示分类请求的结果。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 51b03cf4a579ccab642fe9bdce2e71becebba4be
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938763"
---
# <a name="classificationresult-resource-type"></a><span data-ttu-id="815f3-103">classificationResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="815f3-103">classificationResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="815f3-104">表示来自 Microsoft 分类引擎的分类操作的结果。</span><span class="sxs-lookup"><span data-stu-id="815f3-104">Represents the result of a classification operation from the Microsoft Classification Engine.</span></span> <span data-ttu-id="815f3-105">来自 Azure 信息保护、Office 和其他 Microsoft 服务的数据分类结果可能会返回一[组定义完善的分类类型](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)。</span><span class="sxs-lookup"><span data-stu-id="815f3-105">Data classification results from Azure Information Protection, Office, and other Microsoft services may return a [well-defined set of classification types](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span> <span data-ttu-id="815f3-106">可以向[evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) API 提供这些类型，以将敏感信息解析为 Microsoft 信息保护标签。</span><span class="sxs-lookup"><span data-stu-id="815f3-106">These types can be provided to the [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) API to resolve a sensitive information to a Microsoft Information Protection label.</span></span> 

## <a name="properties"></a><span data-ttu-id="815f3-107">属性</span><span class="sxs-lookup"><span data-stu-id="815f3-107">Properties</span></span>

| <span data-ttu-id="815f3-108">属性</span><span class="sxs-lookup"><span data-stu-id="815f3-108">Property</span></span>        | <span data-ttu-id="815f3-109">类型</span><span class="sxs-lookup"><span data-stu-id="815f3-109">Type</span></span>  | <span data-ttu-id="815f3-110">描述</span><span class="sxs-lookup"><span data-stu-id="815f3-110">Description</span></span>                                                            |
| :-------------- | :---- | :--------------------------------------------------------------------- |
| <span data-ttu-id="815f3-111">confidenceLevel</span><span class="sxs-lookup"><span data-stu-id="815f3-111">confidenceLevel</span></span> | <span data-ttu-id="815f3-112">Int32</span><span class="sxs-lookup"><span data-stu-id="815f3-112">Int32</span></span> | <span data-ttu-id="815f3-113">结果的置信度（0到100）。</span><span class="sxs-lookup"><span data-stu-id="815f3-113">The confidence level, 0 to 100, of the result.</span></span>                         |
| <span data-ttu-id="815f3-114">count</span><span class="sxs-lookup"><span data-stu-id="815f3-114">count</span></span>           | <span data-ttu-id="815f3-115">Int32</span><span class="sxs-lookup"><span data-stu-id="815f3-115">Int32</span></span> | <span data-ttu-id="815f3-116">输入中特定信息类型的实例数。</span><span class="sxs-lookup"><span data-stu-id="815f3-116">The number of instances of the specific information type in the input.</span></span> |
| <span data-ttu-id="815f3-117">sensitiveTypeId</span><span class="sxs-lookup"><span data-stu-id="815f3-117">sensitiveTypeId</span></span> | <span data-ttu-id="815f3-118">GUID</span><span class="sxs-lookup"><span data-stu-id="815f3-118">GUID</span></span>  | <span data-ttu-id="815f3-119">发现的敏感信息类型的 GUID。</span><span class="sxs-lookup"><span data-stu-id="815f3-119">The GUID of the discovered sensitive information type.</span></span>                 |

## <a name="json-representation"></a><span data-ttu-id="815f3-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="815f3-120">JSON representation</span></span>

<span data-ttu-id="815f3-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="815f3-121">The following is a JSON representation of the resource.</span></span>

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
