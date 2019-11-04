---
title: contentInfo 资源类型
description: 表示要标记的某些信息的当前状态。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5191be0533810f0a9da3b0ea83f209d69cc67297
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938875"
---
# <a name="contentinfo-resource-type"></a><span data-ttu-id="46a08-103">contentInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="46a08-103">contentInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46a08-104">表示要标记的某些信息的当前状态。</span><span class="sxs-lookup"><span data-stu-id="46a08-104">Represents the current state of some information that is to be labeled.</span></span> <span data-ttu-id="46a08-105">**contentInfo**将传递到[evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md)、 [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md)和[evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) api，以向 API 描述信息的当前状态。</span><span class="sxs-lookup"><span data-stu-id="46a08-105">**contentInfo** is passed in to the [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), and [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) APIs to describe to the API the current state of the information.</span></span> <span data-ttu-id="46a08-106">此**contentInfo**详细说明了如何在应用、更新或删除标签时添加或删除要添加或删除的元数据、内容标记和保护的结果。</span><span class="sxs-lookup"><span data-stu-id="46a08-106">This **contentInfo** detail drives the results on what metadata, content marking, and protection should be added or removed when the label is applied, updated, or removed.</span></span> 

## <a name="properties"></a><span data-ttu-id="46a08-107">属性</span><span class="sxs-lookup"><span data-stu-id="46a08-107">Properties</span></span>

| <span data-ttu-id="46a08-108">属性</span><span class="sxs-lookup"><span data-stu-id="46a08-108">Property</span></span>   | <span data-ttu-id="46a08-109">类型</span><span class="sxs-lookup"><span data-stu-id="46a08-109">Type</span></span>                                       | <span data-ttu-id="46a08-110">说明</span><span class="sxs-lookup"><span data-stu-id="46a08-110">Description</span></span>                                                                                                                     |
| :--------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="46a08-111">format</span><span class="sxs-lookup"><span data-stu-id="46a08-111">format</span></span>     | <span data-ttu-id="46a08-112">String</span><span class="sxs-lookup"><span data-stu-id="46a08-112">String</span></span>                                     | <span data-ttu-id="46a08-113">可取值为：`default`、`email`。</span><span class="sxs-lookup"><span data-stu-id="46a08-113">Possible values are: `default`, `email`.</span></span>                                                                                        |
| <span data-ttu-id="46a08-114">标识符</span><span class="sxs-lookup"><span data-stu-id="46a08-114">identifier</span></span> | <span data-ttu-id="46a08-115">字符串</span><span class="sxs-lookup"><span data-stu-id="46a08-115">String</span></span>                                     | <span data-ttu-id="46a08-116">用于 Azure 信息保护分析的标识符。</span><span class="sxs-lookup"><span data-stu-id="46a08-116">Identifier used for Azure Information Protection Analytics.</span></span>                                                                     |
| <span data-ttu-id="46a08-117">metadata</span><span class="sxs-lookup"><span data-stu-id="46a08-117">metadata</span></span>   | <span data-ttu-id="46a08-118">[keyValuePair](keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="46a08-118">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="46a08-119">现有的 Microsoft 信息保护元数据作为键/值对进行传递，其中的键是 MSIP_Label_GUID_PropName。</span><span class="sxs-lookup"><span data-stu-id="46a08-119">Existing Microsoft Information Protection metadata is passed as key/value pairs, where the key is the MSIP_Label_GUID_PropName.</span></span> |
| <span data-ttu-id="46a08-120">state</span><span class="sxs-lookup"><span data-stu-id="46a08-120">state</span></span>      | <span data-ttu-id="46a08-121">String</span><span class="sxs-lookup"><span data-stu-id="46a08-121">String</span></span>                                     | <span data-ttu-id="46a08-122">可取值为：`rest`、`motion`、`use`。</span><span class="sxs-lookup"><span data-stu-id="46a08-122">Possible values are: `rest`, `motion`, `use`.</span></span>                                                                                   |

## <a name="json-representation"></a><span data-ttu-id="46a08-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="46a08-123">JSON representation</span></span>

<span data-ttu-id="46a08-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="46a08-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.contentInfo",
  "baseType": null
}-->

```json
{
  "format": "String",
  "identifier": "String",
  "metadata": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "state": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contentInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->