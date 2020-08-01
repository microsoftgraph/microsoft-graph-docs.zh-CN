---
title: localizedName 资源类型
description: 表示术语库中使用的本地化名称，用于标识本地化语言中的名称。
author: mohitpcad
ms.author: mopathak
localization_priority: Normal
ms.prod: sharepoint-taxonomy
doc_type: resourcePageType
ms.openlocfilehash: cc29deb6e6db5f5664e6fb6bed69195b7183e026
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539157"
---
# <a name="localizedname-resource-type"></a><span data-ttu-id="b0cb0-103">localizedName 资源类型</span><span class="sxs-lookup"><span data-stu-id="b0cb0-103">localizedName resource type</span></span>

<span data-ttu-id="b0cb0-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="b0cb0-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0cb0-105">表示术语[库]中使用的本地化名称，用于标识本地化语言中的名称。</span><span class="sxs-lookup"><span data-stu-id="b0cb0-105">Represents the localized name used in the term [store], which identifies the name in the localized language.</span></span> <span data-ttu-id="b0cb0-106">有关详细信息，请参阅[localizedLabel]。</span><span class="sxs-lookup"><span data-stu-id="b0cb0-106">For more information, see [localizedLabel].</span></span>

## <a name="properties"></a><span data-ttu-id="b0cb0-107">属性</span><span class="sxs-lookup"><span data-stu-id="b0cb0-107">Properties</span></span>
|<span data-ttu-id="b0cb0-108">属性</span><span class="sxs-lookup"><span data-stu-id="b0cb0-108">Property</span></span>|<span data-ttu-id="b0cb0-109">类型</span><span class="sxs-lookup"><span data-stu-id="b0cb0-109">Type</span></span>|<span data-ttu-id="b0cb0-110">说明</span><span class="sxs-lookup"><span data-stu-id="b0cb0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0cb0-111">languageTag</span><span class="sxs-lookup"><span data-stu-id="b0cb0-111">languageTag</span></span>|<span data-ttu-id="b0cb0-112">String</span><span class="sxs-lookup"><span data-stu-id="b0cb0-112">String</span></span>|<span data-ttu-id="b0cb0-113">标签的语言标记。</span><span class="sxs-lookup"><span data-stu-id="b0cb0-113">The language tag for the label.</span></span>|
|<span data-ttu-id="b0cb0-114">name</span><span class="sxs-lookup"><span data-stu-id="b0cb0-114">name</span></span>|<span data-ttu-id="b0cb0-115">String</span><span class="sxs-lookup"><span data-stu-id="b0cb0-115">String</span></span>|<span data-ttu-id="b0cb0-116">本地化语言中的名称。</span><span class="sxs-lookup"><span data-stu-id="b0cb0-116">The name in the localized language.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0cb0-117">关系</span><span class="sxs-lookup"><span data-stu-id="b0cb0-117">Relationships</span></span>
<span data-ttu-id="b0cb0-118">无。</span><span class="sxs-lookup"><span data-stu-id="b0cb0-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0cb0-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0cb0-119">JSON representation</span></span>
<span data-ttu-id="b0cb0-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0cb0-120">The following is a JSON representation of the resource.</span></span>
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
[microsoft]: ../resources/termstore-store.md
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
