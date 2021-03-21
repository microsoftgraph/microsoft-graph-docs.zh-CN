---
title: contentInfo 资源类型
description: 表示要标记的一些信息的当前状态。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 939d7730c0de2ffb13d4dbdcade6f7c2fbce5de4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962649"
---
# <a name="contentinfo-resource-type"></a><span data-ttu-id="f35d9-103">contentInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="f35d9-103">contentInfo resource type</span></span>

<span data-ttu-id="f35d9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f35d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f35d9-105">表示要标记的一些信息的当前状态。</span><span class="sxs-lookup"><span data-stu-id="f35d9-105">Represents the current state of some information that is to be labeled.</span></span> <span data-ttu-id="f35d9-106">**contentInfo** 传递到 [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) [、evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md)和 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) API，以向 API 描述信息的当前状态。</span><span class="sxs-lookup"><span data-stu-id="f35d9-106">**contentInfo** is passed in to the [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), and [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) APIs to describe to the API the current state of the information.</span></span> <span data-ttu-id="f35d9-107">此 **contentInfo** 详细信息将推动在应用、更新或删除标签时应添加或删除哪些元数据、内容标记和保护的结果。</span><span class="sxs-lookup"><span data-stu-id="f35d9-107">This **contentInfo** detail drives the results on what metadata, content marking, and protection should be added or removed when the label is applied, updated, or removed.</span></span> 

## <a name="properties"></a><span data-ttu-id="f35d9-108">属性</span><span class="sxs-lookup"><span data-stu-id="f35d9-108">Properties</span></span>

| <span data-ttu-id="f35d9-109">属性</span><span class="sxs-lookup"><span data-stu-id="f35d9-109">Property</span></span>   | <span data-ttu-id="f35d9-110">类型</span><span class="sxs-lookup"><span data-stu-id="f35d9-110">Type</span></span>                                       | <span data-ttu-id="f35d9-111">说明</span><span class="sxs-lookup"><span data-stu-id="f35d9-111">Description</span></span>                                                                                                                     |
| :--------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="f35d9-112">format</span><span class="sxs-lookup"><span data-stu-id="f35d9-112">format</span></span>     | <span data-ttu-id="f35d9-113">String</span><span class="sxs-lookup"><span data-stu-id="f35d9-113">String</span></span>                                     | <span data-ttu-id="f35d9-114">可取值为：`default`、`email`。</span><span class="sxs-lookup"><span data-stu-id="f35d9-114">Possible values are: `default`, `email`.</span></span>                                                                                        |
| <span data-ttu-id="f35d9-115">标识符</span><span class="sxs-lookup"><span data-stu-id="f35d9-115">identifier</span></span> | <span data-ttu-id="f35d9-116">String</span><span class="sxs-lookup"><span data-stu-id="f35d9-116">String</span></span>                                     | <span data-ttu-id="f35d9-117">用于 Azure 信息保护分析的标识符。</span><span class="sxs-lookup"><span data-stu-id="f35d9-117">Identifier used for Azure Information Protection Analytics.</span></span>                                                                     |
| <span data-ttu-id="f35d9-118">metadata</span><span class="sxs-lookup"><span data-stu-id="f35d9-118">metadata</span></span>   | <span data-ttu-id="f35d9-119">[keyValuePair](keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f35d9-119">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="f35d9-120">现有的 Microsoft 信息保护元数据作为键/值对传递，其中键是MSIP_Label_GUID_PropName。</span><span class="sxs-lookup"><span data-stu-id="f35d9-120">Existing Microsoft Information Protection metadata is passed as key/value pairs, where the key is the MSIP_Label_GUID_PropName.</span></span> |
| <span data-ttu-id="f35d9-121">state</span><span class="sxs-lookup"><span data-stu-id="f35d9-121">state</span></span>      | <span data-ttu-id="f35d9-122">String</span><span class="sxs-lookup"><span data-stu-id="f35d9-122">String</span></span>                                     | <span data-ttu-id="f35d9-123">可取值为：`rest`、`motion`、`use`。</span><span class="sxs-lookup"><span data-stu-id="f35d9-123">Possible values are: `rest`, `motion`, `use`.</span></span>                                                                                   |

## <a name="json-representation"></a><span data-ttu-id="f35d9-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f35d9-124">JSON representation</span></span>

<span data-ttu-id="f35d9-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f35d9-125">The following is a JSON representation of the resource.</span></span>

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

