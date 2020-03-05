---
title: contentInfo 资源类型
description: 表示要标记的某些信息的当前状态。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 04fcee1c95628782d4a959732afa88bf689e4ea7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507434"
---
# <a name="contentinfo-resource-type"></a><span data-ttu-id="0128a-103">contentInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="0128a-103">contentInfo resource type</span></span>

<span data-ttu-id="0128a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0128a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0128a-105">表示要标记的某些信息的当前状态。</span><span class="sxs-lookup"><span data-stu-id="0128a-105">Represents the current state of some information that is to be labeled.</span></span> <span data-ttu-id="0128a-106">**contentInfo**将传递到[evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md)、 [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md)和[evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) api，以向 API 描述信息的当前状态。</span><span class="sxs-lookup"><span data-stu-id="0128a-106">**contentInfo** is passed in to the [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), and [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) APIs to describe to the API the current state of the information.</span></span> <span data-ttu-id="0128a-107">此**contentInfo**详细说明了如何在应用、更新或删除标签时添加或删除要添加或删除的元数据、内容标记和保护的结果。</span><span class="sxs-lookup"><span data-stu-id="0128a-107">This **contentInfo** detail drives the results on what metadata, content marking, and protection should be added or removed when the label is applied, updated, or removed.</span></span> 

## <a name="properties"></a><span data-ttu-id="0128a-108">属性</span><span class="sxs-lookup"><span data-stu-id="0128a-108">Properties</span></span>

| <span data-ttu-id="0128a-109">属性</span><span class="sxs-lookup"><span data-stu-id="0128a-109">Property</span></span>   | <span data-ttu-id="0128a-110">类型</span><span class="sxs-lookup"><span data-stu-id="0128a-110">Type</span></span>                                       | <span data-ttu-id="0128a-111">说明</span><span class="sxs-lookup"><span data-stu-id="0128a-111">Description</span></span>                                                                                                                     |
| :--------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="0128a-112">format</span><span class="sxs-lookup"><span data-stu-id="0128a-112">format</span></span>     | <span data-ttu-id="0128a-113">String</span><span class="sxs-lookup"><span data-stu-id="0128a-113">String</span></span>                                     | <span data-ttu-id="0128a-114">可取值为：`default`、`email`。</span><span class="sxs-lookup"><span data-stu-id="0128a-114">Possible values are: `default`, `email`.</span></span>                                                                                        |
| <span data-ttu-id="0128a-115">标识符</span><span class="sxs-lookup"><span data-stu-id="0128a-115">identifier</span></span> | <span data-ttu-id="0128a-116">String</span><span class="sxs-lookup"><span data-stu-id="0128a-116">String</span></span>                                     | <span data-ttu-id="0128a-117">用于 Azure 信息保护分析的标识符。</span><span class="sxs-lookup"><span data-stu-id="0128a-117">Identifier used for Azure Information Protection Analytics.</span></span>                                                                     |
| <span data-ttu-id="0128a-118">metadata</span><span class="sxs-lookup"><span data-stu-id="0128a-118">metadata</span></span>   | <span data-ttu-id="0128a-119">[keyValuePair](keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0128a-119">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="0128a-120">现有的 Microsoft 信息保护元数据作为键/值对进行传递，其中的键是 MSIP_Label_GUID_PropName。</span><span class="sxs-lookup"><span data-stu-id="0128a-120">Existing Microsoft Information Protection metadata is passed as key/value pairs, where the key is the MSIP_Label_GUID_PropName.</span></span> |
| <span data-ttu-id="0128a-121">state</span><span class="sxs-lookup"><span data-stu-id="0128a-121">state</span></span>      | <span data-ttu-id="0128a-122">String</span><span class="sxs-lookup"><span data-stu-id="0128a-122">String</span></span>                                     | <span data-ttu-id="0128a-123">可取值为：`rest`、`motion`、`use`。</span><span class="sxs-lookup"><span data-stu-id="0128a-123">Possible values are: `rest`, `motion`, `use`.</span></span>                                                                                   |

## <a name="json-representation"></a><span data-ttu-id="0128a-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0128a-124">JSON representation</span></span>

<span data-ttu-id="0128a-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0128a-125">The following is a JSON representation of the resource.</span></span>

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