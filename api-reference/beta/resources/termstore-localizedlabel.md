---
title: localizedLabel 资源类型
description: 表示术语存储中术语的标签。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 4d7de3c9567c20659af4c863d2cf1ac248beff6b
ms.sourcegitcommit: a9a035e7cf7b500aebe5477c05361552e7c3a7ab
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696308"
---
# <a name="localizedlabel-resource-type"></a><span data-ttu-id="e7c1b-103">localizedLabel 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7c1b-103">localizedLabel resource type</span></span>

<span data-ttu-id="e7c1b-104">命名空间：microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="e7c1b-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7c1b-105">表示术语存储 [中] 术语 [的标签]。</span><span class="sxs-lookup"><span data-stu-id="e7c1b-105">Represents the label for a [term] in the term [store].</span></span>

<span data-ttu-id="e7c1b-106">标识与给定术语关联的标签。</span><span class="sxs-lookup"><span data-stu-id="e7c1b-106">Identifies the labels associated with a given term.</span></span>

## <a name="properties"></a><span data-ttu-id="e7c1b-107">属性</span><span class="sxs-lookup"><span data-stu-id="e7c1b-107">Properties</span></span>
|<span data-ttu-id="e7c1b-108">属性</span><span class="sxs-lookup"><span data-stu-id="e7c1b-108">Property</span></span>|<span data-ttu-id="e7c1b-109">类型</span><span class="sxs-lookup"><span data-stu-id="e7c1b-109">Type</span></span>|<span data-ttu-id="e7c1b-110">说明</span><span class="sxs-lookup"><span data-stu-id="e7c1b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7c1b-111">isDefault</span><span class="sxs-lookup"><span data-stu-id="e7c1b-111">isDefault</span></span>|<span data-ttu-id="e7c1b-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7c1b-112">Boolean</span></span>|<span data-ttu-id="e7c1b-113">指示标签是否是默认标签。</span><span class="sxs-lookup"><span data-stu-id="e7c1b-113">Indicates whether the label is the default label.</span></span>|
|<span data-ttu-id="e7c1b-114">languageTag</span><span class="sxs-lookup"><span data-stu-id="e7c1b-114">languageTag</span></span>|<span data-ttu-id="e7c1b-115">String</span><span class="sxs-lookup"><span data-stu-id="e7c1b-115">String</span></span>|<span data-ttu-id="e7c1b-116">标签的语言标记。</span><span class="sxs-lookup"><span data-stu-id="e7c1b-116">The language tag for the label.</span></span>|
|<span data-ttu-id="e7c1b-117">name</span><span class="sxs-lookup"><span data-stu-id="e7c1b-117">name</span></span>|<span data-ttu-id="e7c1b-118">String</span><span class="sxs-lookup"><span data-stu-id="e7c1b-118">String</span></span>|<span data-ttu-id="e7c1b-119">标签的名称。</span><span class="sxs-lookup"><span data-stu-id="e7c1b-119">The name of the label.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7c1b-120">关系</span><span class="sxs-lookup"><span data-stu-id="e7c1b-120">Relationships</span></span>
<span data-ttu-id="e7c1b-121">无。</span><span class="sxs-lookup"><span data-stu-id="e7c1b-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7c1b-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7c1b-122">JSON representation</span></span>
<span data-ttu-id="e7c1b-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7c1b-123">The following is a JSON representation of the resource.</span></span>
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
[term]: ../resources/termstore-term.md
[store]: ../resources/termstore-store.md


<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedLabelFacet is the facet for containing the label of a term",
  "keywords": "termLocalizedLabelFacet,facet,resource",
  "section": "documentation",
  "tocPath": "termstorelocalizedlabel",
  "tocBookmarks": {
    "Resources/termStore.termstorelocalizedlabel&quot;: &quot;#"
  },
  "suppressions": []
}
-->


