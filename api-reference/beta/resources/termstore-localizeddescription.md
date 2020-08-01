---
title: localizedDescription 资源类型
description: 表示用于描述术语库中的术语的本地化说明。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0bded2c1ad4804fb952ecfd9c75c87f3a8624c7e
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539158"
---
# <a name="localizeddescription-resource-type"></a><span data-ttu-id="94747-103">localizedDescription 资源类型</span><span class="sxs-lookup"><span data-stu-id="94747-103">localizedDescription resource type</span></span>

<span data-ttu-id="94747-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="94747-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94747-105">表示用于描述术语[库]中的[术语]的本地化说明。</span><span class="sxs-lookup"><span data-stu-id="94747-105">Represents the localized description used to describe a [term] in the term [store].</span></span>


## <a name="properties"></a><span data-ttu-id="94747-106">属性</span><span class="sxs-lookup"><span data-stu-id="94747-106">Properties</span></span>
|<span data-ttu-id="94747-107">属性</span><span class="sxs-lookup"><span data-stu-id="94747-107">Property</span></span>|<span data-ttu-id="94747-108">类型</span><span class="sxs-lookup"><span data-stu-id="94747-108">Type</span></span>|<span data-ttu-id="94747-109">说明</span><span class="sxs-lookup"><span data-stu-id="94747-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94747-110">说明</span><span class="sxs-lookup"><span data-stu-id="94747-110">description</span></span>|<span data-ttu-id="94747-111">String</span><span class="sxs-lookup"><span data-stu-id="94747-111">String</span></span>|<span data-ttu-id="94747-112">本地化语言中的说明。</span><span class="sxs-lookup"><span data-stu-id="94747-112">The description in the localized language.</span></span>|
|<span data-ttu-id="94747-113">languageTag</span><span class="sxs-lookup"><span data-stu-id="94747-113">languageTag</span></span>|<span data-ttu-id="94747-114">String</span><span class="sxs-lookup"><span data-stu-id="94747-114">String</span></span>|<span data-ttu-id="94747-115">标签的语言标记。</span><span class="sxs-lookup"><span data-stu-id="94747-115">The language tag for the label.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94747-116">关系</span><span class="sxs-lookup"><span data-stu-id="94747-116">Relationships</span></span>
<span data-ttu-id="94747-117">无。</span><span class="sxs-lookup"><span data-stu-id="94747-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="94747-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94747-118">JSON representation</span></span>
<span data-ttu-id="94747-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94747-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.termStore.localizedDescription"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.localizedDescription",
  "description": "String",
  "languageTag": "String"
}
```

[microsoft.graph.termStore.term]: termStore-term.md
[microsoft.graph.termStore.store]: termStore-store.md
[术语]: ../resources/termstore-term.md
[term]: ../resources/termstore-term.md
[microsoft]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md

<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedDescriptionFacet is the facet for containing the description of a set",
  "keywords": "termLocalizedDescriptionFacet,facet,resource",
  "section": "documentation",
  "tocPath": "TermLocalizedDescriptionFacet",
  "tocBookmarks": {
    "Resources/termStore.termLocalizedDescription": "#"
  },
  "suppressions": []
}
-->
