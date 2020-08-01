---
title: localizedLabel 资源类型
description: 表示术语库中术语的标签。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: dbd067dbd3447691fd7fbd8e51670cceb46d64da
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539209"
---
# <a name="localizedlabel-resource-type"></a><span data-ttu-id="6dacb-103">localizedLabel 资源类型</span><span class="sxs-lookup"><span data-stu-id="6dacb-103">localizedLabel resource type</span></span>

<span data-ttu-id="6dacb-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="6dacb-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dacb-105">表示术语[库]中[术语]的标签。</span><span class="sxs-lookup"><span data-stu-id="6dacb-105">Represents the label for a [term] in the term [store].</span></span>

<span data-ttu-id="6dacb-106">标识与给定术语相关联的标签。</span><span class="sxs-lookup"><span data-stu-id="6dacb-106">Identifies the labels associated with a given term.</span></span>

## <a name="properties"></a><span data-ttu-id="6dacb-107">属性</span><span class="sxs-lookup"><span data-stu-id="6dacb-107">Properties</span></span>
|<span data-ttu-id="6dacb-108">属性</span><span class="sxs-lookup"><span data-stu-id="6dacb-108">Property</span></span>|<span data-ttu-id="6dacb-109">类型</span><span class="sxs-lookup"><span data-stu-id="6dacb-109">Type</span></span>|<span data-ttu-id="6dacb-110">说明</span><span class="sxs-lookup"><span data-stu-id="6dacb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dacb-111">isDefault</span><span class="sxs-lookup"><span data-stu-id="6dacb-111">isDefault</span></span>|<span data-ttu-id="6dacb-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="6dacb-112">Boolean</span></span>|<span data-ttu-id="6dacb-113">指示标签是否为默认标签。</span><span class="sxs-lookup"><span data-stu-id="6dacb-113">Indicates whether the label is the default label.</span></span>|
|<span data-ttu-id="6dacb-114">languageTag</span><span class="sxs-lookup"><span data-stu-id="6dacb-114">languageTag</span></span>|<span data-ttu-id="6dacb-115">String</span><span class="sxs-lookup"><span data-stu-id="6dacb-115">String</span></span>|<span data-ttu-id="6dacb-116">标签的 anguage 标记。</span><span class="sxs-lookup"><span data-stu-id="6dacb-116">The anguage tag for the label.</span></span>|
|<span data-ttu-id="6dacb-117">name</span><span class="sxs-lookup"><span data-stu-id="6dacb-117">name</span></span>|<span data-ttu-id="6dacb-118">String</span><span class="sxs-lookup"><span data-stu-id="6dacb-118">String</span></span>|<span data-ttu-id="6dacb-119">标签的名称。</span><span class="sxs-lookup"><span data-stu-id="6dacb-119">The name of the label.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6dacb-120">关系</span><span class="sxs-lookup"><span data-stu-id="6dacb-120">Relationships</span></span>
<span data-ttu-id="6dacb-121">无。</span><span class="sxs-lookup"><span data-stu-id="6dacb-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6dacb-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6dacb-122">JSON representation</span></span>
<span data-ttu-id="6dacb-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6dacb-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.termStore.localizedLabel"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.localizedLabel",
  "name": "String",
  "isDefault": "Boolean",
  "languageTag": "String"
}
```


[microsoft.graph.termStore.term]: termstore-term.md
[microsoft.graph.termStore.localizedName]: termstore-localizedname.md
[microsoft.graph.termStore.store]: termstore-store.md
[术语]: ../resources/termstore-term.md
[term]: ../resources/termstore-term.md
[microsoft]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md


<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedLabelFacet is the facet for containing the label of a term",
  "keywords": "termLocalizedLabelFacet,facet,resource",
  "section": "documentation",
  "tocPath": "termstorelocalizedlabel",
  "tocBookmarks": {
    "Resources/termStore.termstorelocalizedlabel": "#"
  },
  "suppressions": []
}
-->
