---
title: localizedName 资源类型
description: 表示术语库中使用的本地化名称，用于标识本地化语言中的名称。
author: mohitpcad
ms.author: mopathak
localization_priority: Normal
ms.prod: sharepoint-taxonomy
doc_type: resourcePageType
ms.openlocfilehash: 5c9e6d4cd614c242e8f915fde71eadd07aa5de15
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973601"
---
# <a name="localizedname-resource-type"></a><span data-ttu-id="67b25-103">localizedName 资源类型</span><span class="sxs-lookup"><span data-stu-id="67b25-103">localizedName resource type</span></span>

<span data-ttu-id="67b25-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="67b25-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67b25-105">表示术语 [库]中使用的本地化名称，用于标识本地化语言中的名称。</span><span class="sxs-lookup"><span data-stu-id="67b25-105">Represents the localized name used in the term [store], which identifies the name in the localized language.</span></span> <span data-ttu-id="67b25-106">有关详细信息，请参阅 [localizedLabel]。</span><span class="sxs-lookup"><span data-stu-id="67b25-106">For more information, see [localizedLabel].</span></span>

## <a name="properties"></a><span data-ttu-id="67b25-107">属性</span><span class="sxs-lookup"><span data-stu-id="67b25-107">Properties</span></span>
|<span data-ttu-id="67b25-108">属性</span><span class="sxs-lookup"><span data-stu-id="67b25-108">Property</span></span>|<span data-ttu-id="67b25-109">类型</span><span class="sxs-lookup"><span data-stu-id="67b25-109">Type</span></span>|<span data-ttu-id="67b25-110">说明</span><span class="sxs-lookup"><span data-stu-id="67b25-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67b25-111">languageTag</span><span class="sxs-lookup"><span data-stu-id="67b25-111">languageTag</span></span>|<span data-ttu-id="67b25-112">String</span><span class="sxs-lookup"><span data-stu-id="67b25-112">String</span></span>|<span data-ttu-id="67b25-113">标签的语言标记。</span><span class="sxs-lookup"><span data-stu-id="67b25-113">The language tag for the label.</span></span>|
|<span data-ttu-id="67b25-114">name</span><span class="sxs-lookup"><span data-stu-id="67b25-114">name</span></span>|<span data-ttu-id="67b25-115">String</span><span class="sxs-lookup"><span data-stu-id="67b25-115">String</span></span>|<span data-ttu-id="67b25-116">本地化语言中的名称。</span><span class="sxs-lookup"><span data-stu-id="67b25-116">The name in the localized language.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67b25-117">关系</span><span class="sxs-lookup"><span data-stu-id="67b25-117">Relationships</span></span>
<span data-ttu-id="67b25-118">无。</span><span class="sxs-lookup"><span data-stu-id="67b25-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="67b25-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="67b25-119">JSON representation</span></span>
<span data-ttu-id="67b25-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67b25-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.termStore.localizedName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.localizedName",
  "name": "String",
  "languageTag": "String"
}
```

[microsoft.graph.termStore.localizedLabel]: termstore-localizedlabel.md
[microsoft.graph.termstore.store]: termstore-store.md
[商店]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md
[localizedLabel]: ../resources/termstore-localizedlabel.md

<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedName is the facet for containing the name of termGroup",
  "keywords": "termLocalizedLNameFacet,facet,resource",
  "section": "documentation",
  "tocPath": "TermLocalizedNameFacet",
  "tocBookmarks": {
    "Resources/termStore.termLocalizedName": "#"
  },
  "suppressions": []
}
-->


