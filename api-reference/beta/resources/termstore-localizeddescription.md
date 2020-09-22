---
title: localizedDescription 资源类型
description: 表示用于描述术语库中的术语的本地化说明。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 738555750c22f3ffdd5fbd43c8b1849888e0a40f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973615"
---
# <a name="localizeddescription-resource-type"></a><span data-ttu-id="7a0d0-103">localizedDescription 资源类型</span><span class="sxs-lookup"><span data-stu-id="7a0d0-103">localizedDescription resource type</span></span>

<span data-ttu-id="7a0d0-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="7a0d0-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a0d0-105">表示用于描述术语[库]中的[术语]的本地化说明。</span><span class="sxs-lookup"><span data-stu-id="7a0d0-105">Represents the localized description used to describe a [term] in the term [store].</span></span>


## <a name="properties"></a><span data-ttu-id="7a0d0-106">属性</span><span class="sxs-lookup"><span data-stu-id="7a0d0-106">Properties</span></span>
|<span data-ttu-id="7a0d0-107">属性</span><span class="sxs-lookup"><span data-stu-id="7a0d0-107">Property</span></span>|<span data-ttu-id="7a0d0-108">类型</span><span class="sxs-lookup"><span data-stu-id="7a0d0-108">Type</span></span>|<span data-ttu-id="7a0d0-109">说明</span><span class="sxs-lookup"><span data-stu-id="7a0d0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a0d0-110">说明</span><span class="sxs-lookup"><span data-stu-id="7a0d0-110">description</span></span>|<span data-ttu-id="7a0d0-111">String</span><span class="sxs-lookup"><span data-stu-id="7a0d0-111">String</span></span>|<span data-ttu-id="7a0d0-112">本地化语言中的说明。</span><span class="sxs-lookup"><span data-stu-id="7a0d0-112">The description in the localized language.</span></span>|
|<span data-ttu-id="7a0d0-113">languageTag</span><span class="sxs-lookup"><span data-stu-id="7a0d0-113">languageTag</span></span>|<span data-ttu-id="7a0d0-114">String</span><span class="sxs-lookup"><span data-stu-id="7a0d0-114">String</span></span>|<span data-ttu-id="7a0d0-115">标签的语言标记。</span><span class="sxs-lookup"><span data-stu-id="7a0d0-115">The language tag for the label.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a0d0-116">关系</span><span class="sxs-lookup"><span data-stu-id="7a0d0-116">Relationships</span></span>
<span data-ttu-id="7a0d0-117">无。</span><span class="sxs-lookup"><span data-stu-id="7a0d0-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a0d0-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a0d0-118">JSON representation</span></span>
<span data-ttu-id="7a0d0-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a0d0-119">The following is a JSON representation of the resource.</span></span>
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


