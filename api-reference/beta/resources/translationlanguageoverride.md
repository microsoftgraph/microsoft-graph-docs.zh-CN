---
title: translationLanguageOverride 资源类型
description: 表示翻译语言替代列表中的条目的资源。
localization_priority: Normal
author: jasonbro
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 791908546c64cbb0ea7ee7434bece3dca5c894cc
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518146"
---
# <a name="translationlanguageoverride-resource-type"></a><span data-ttu-id="194f6-103">translationLanguageOverride 资源类型</span><span class="sxs-lookup"><span data-stu-id="194f6-103">translationLanguageOverride resource type</span></span>

<span data-ttu-id="194f6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="194f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="194f6-105">表示语言的任何翻译替代。</span><span class="sxs-lookup"><span data-stu-id="194f6-105">Represents any translation override for a language.</span></span>

## <a name="properties"></a><span data-ttu-id="194f6-106">属性</span><span class="sxs-lookup"><span data-stu-id="194f6-106">Properties</span></span>

|<span data-ttu-id="194f6-107">属性</span><span class="sxs-lookup"><span data-stu-id="194f6-107">Property</span></span>             |<span data-ttu-id="194f6-108">类型</span><span class="sxs-lookup"><span data-stu-id="194f6-108">Type</span></span>                                         |<span data-ttu-id="194f6-109">说明</span><span class="sxs-lookup"><span data-stu-id="194f6-109">Description</span></span>                                                            |
|---------------------|-------------------------------------------------------------|-----------------------------------------------------------------------|
|<span data-ttu-id="194f6-110">languageTag</span><span class="sxs-lookup"><span data-stu-id="194f6-110">languageTag</span></span>          |<span data-ttu-id="194f6-111">String</span><span class="sxs-lookup"><span data-stu-id="194f6-111">String</span></span>                                       |<span data-ttu-id="194f6-112">要应用替代的语言。</span><span class="sxs-lookup"><span data-stu-id="194f6-112">The language to apply the override.</span></span><br><br><span data-ttu-id="194f6-113">默认返回。</span><span class="sxs-lookup"><span data-stu-id="194f6-113">Returned by default.</span></span> <span data-ttu-id="194f6-114">不可为空。</span><span class="sxs-lookup"><span data-stu-id="194f6-114">Not nullable.</span></span>       |                   
|<span data-ttu-id="194f6-115">translationBehavior</span><span class="sxs-lookup"><span data-stu-id="194f6-115">translationBehavior</span></span>  |[<span data-ttu-id="194f6-116">translationBehavior</span><span class="sxs-lookup"><span data-stu-id="194f6-116">translationBehavior</span></span>](translationPreferences.md#translationbehavior-values)        |<span data-ttu-id="194f6-117">语言（如果有）的翻译替代行为。</span><span class="sxs-lookup"><span data-stu-id="194f6-117">The translation override behavior for the language, if any.</span></span><br><br><span data-ttu-id="194f6-118">默认返回。</span><span class="sxs-lookup"><span data-stu-id="194f6-118">Returned by default.</span></span> <span data-ttu-id="194f6-119">不可为空。</span><span class="sxs-lookup"><span data-stu-id="194f6-119">Not nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="194f6-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="194f6-120">JSON representation</span></span>

<span data-ttu-id="194f6-121">下面是资源的 JSON 定义。</span><span class="sxs-lookup"><span data-stu-id="194f6-121">The following is a JSON definition of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.translationLanguageOverride"
}-->

```json
{
    "languageTag": "string",
    "translationBehavior": "string"
}
```
<!-- {
  "type": "#page.annotation",
  "description": translationLanguageOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


