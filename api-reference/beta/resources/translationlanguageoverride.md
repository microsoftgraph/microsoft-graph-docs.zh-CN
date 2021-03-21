---
title: translationLanguageOverride 资源类型
description: 表示翻译语言替代列表中的条目的资源。
localization_priority: Normal
author: jasonbro
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: c9fa8d600ee3fb503446965d78491563c4ceae2e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954949"
---
# <a name="translationlanguageoverride-resource-type"></a><span data-ttu-id="e4f63-103">translationLanguageOverride 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4f63-103">translationLanguageOverride resource type</span></span>

<span data-ttu-id="e4f63-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4f63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4f63-105">表示语言的任何翻译替代。</span><span class="sxs-lookup"><span data-stu-id="e4f63-105">Represents any translation override for a language.</span></span>

## <a name="properties"></a><span data-ttu-id="e4f63-106">属性</span><span class="sxs-lookup"><span data-stu-id="e4f63-106">Properties</span></span>

|<span data-ttu-id="e4f63-107">属性</span><span class="sxs-lookup"><span data-stu-id="e4f63-107">Property</span></span>             |<span data-ttu-id="e4f63-108">类型</span><span class="sxs-lookup"><span data-stu-id="e4f63-108">Type</span></span>                                         |<span data-ttu-id="e4f63-109">说明</span><span class="sxs-lookup"><span data-stu-id="e4f63-109">Description</span></span>                                                            |
|---------------------|-------------------------------------------------------------|-----------------------------------------------------------------------|
|<span data-ttu-id="e4f63-110">languageTag</span><span class="sxs-lookup"><span data-stu-id="e4f63-110">languageTag</span></span>          |<span data-ttu-id="e4f63-111">String</span><span class="sxs-lookup"><span data-stu-id="e4f63-111">String</span></span>                                       |<span data-ttu-id="e4f63-112">要应用替代的语言。</span><span class="sxs-lookup"><span data-stu-id="e4f63-112">The language to apply the override.</span></span><br><br><span data-ttu-id="e4f63-113">默认返回。</span><span class="sxs-lookup"><span data-stu-id="e4f63-113">Returned by default.</span></span> <span data-ttu-id="e4f63-114">不可为空。</span><span class="sxs-lookup"><span data-stu-id="e4f63-114">Not nullable.</span></span>       |                   
|<span data-ttu-id="e4f63-115">translationBehavior</span><span class="sxs-lookup"><span data-stu-id="e4f63-115">translationBehavior</span></span>  |[<span data-ttu-id="e4f63-116">translationBehavior</span><span class="sxs-lookup"><span data-stu-id="e4f63-116">translationBehavior</span></span>](translationPreferences.md#translationbehavior-values)        |<span data-ttu-id="e4f63-117">语言（如果有）的翻译替代行为。</span><span class="sxs-lookup"><span data-stu-id="e4f63-117">The translation override behavior for the language, if any.</span></span><br><br><span data-ttu-id="e4f63-118">默认返回。</span><span class="sxs-lookup"><span data-stu-id="e4f63-118">Returned by default.</span></span> <span data-ttu-id="e4f63-119">不可为空。</span><span class="sxs-lookup"><span data-stu-id="e4f63-119">Not nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4f63-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4f63-120">JSON representation</span></span>

<span data-ttu-id="e4f63-121">下面是资源的 JSON 定义。</span><span class="sxs-lookup"><span data-stu-id="e4f63-121">The following is a JSON definition of the resource.</span></span>

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


