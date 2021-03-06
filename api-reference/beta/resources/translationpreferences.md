---
title: translationPreferences 资源类型
description: 表示用户的翻译设置首选项的资源。
localization_priority: Normal
author: jasonbro
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: b2e45f797709067e52f142c3de3f2be566b55201
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518145"
---
# <a name="translationpreferences-resource-type"></a><span data-ttu-id="2aa72-103">translationPreferences 资源类型</span><span class="sxs-lookup"><span data-stu-id="2aa72-103">translationPreferences resource type</span></span>

<span data-ttu-id="2aa72-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2aa72-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2aa72-105">表示用户的翻译语言替代列表中的条目。</span><span class="sxs-lookup"><span data-stu-id="2aa72-105">Represents an entry in a user's translation language override list.</span></span>

## <a name="properties"></a><span data-ttu-id="2aa72-106">属性</span><span class="sxs-lookup"><span data-stu-id="2aa72-106">Properties</span></span>

|<span data-ttu-id="2aa72-107">属性</span><span class="sxs-lookup"><span data-stu-id="2aa72-107">Property</span></span>             |<span data-ttu-id="2aa72-108">类型</span><span class="sxs-lookup"><span data-stu-id="2aa72-108">Type</span></span>                                         |<span data-ttu-id="2aa72-109">说明</span><span class="sxs-lookup"><span data-stu-id="2aa72-109">Description</span></span>                                                            |
|---------------------|-------------------------------------------------------------|-----------------------------------------------------------------------|
|<span data-ttu-id="2aa72-110">translationBehavior</span><span class="sxs-lookup"><span data-stu-id="2aa72-110">translationBehavior</span></span>  |[<span data-ttu-id="2aa72-111">translationBehavior</span><span class="sxs-lookup"><span data-stu-id="2aa72-111">translationBehavior</span></span>](#translationbehavior-values)       |<span data-ttu-id="2aa72-112">用户的首选翻译行为。</span><span class="sxs-lookup"><span data-stu-id="2aa72-112">The user's preferred translation behavior.</span></span><br><br><span data-ttu-id="2aa72-113">默认返回。</span><span class="sxs-lookup"><span data-stu-id="2aa72-113">Returned by default.</span></span> <span data-ttu-id="2aa72-114">不可为空。</span><span class="sxs-lookup"><span data-stu-id="2aa72-114">Not nullable.</span></span> |                   
|<span data-ttu-id="2aa72-115">languageOverrides</span><span class="sxs-lookup"><span data-stu-id="2aa72-115">languageOverrides</span></span>    |<span data-ttu-id="2aa72-116">[translationLanguageOverride](translationLanguageOverride.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2aa72-116">[translationLanguageOverride](translationLanguageOverride.md) collection</span></span>                | <span data-ttu-id="2aa72-117">语言（如果有）的翻译替代行为。</span><span class="sxs-lookup"><span data-stu-id="2aa72-117">Translation override behavior for languages, if any.</span></span><br><br><span data-ttu-id="2aa72-118">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="2aa72-118">Returned by default.</span></span>|
|<span data-ttu-id="2aa72-119">untranslatedLanguages</span><span class="sxs-lookup"><span data-stu-id="2aa72-119">untranslatedLanguages</span></span>|<span data-ttu-id="2aa72-120">字符串集合</span><span class="sxs-lookup"><span data-stu-id="2aa72-120">String collection</span></span>| <span data-ttu-id="2aa72-121">用户不需要翻译的语言列表。</span><span class="sxs-lookup"><span data-stu-id="2aa72-121">The list of languages the user does not need translated.</span></span> <span data-ttu-id="2aa72-122">这从 [regionalAndLanguageSettings](regionalandlanguagesettings.md)中的 **authoringLanguages** 集合和 **translationPreferences** 中的 **languageOverrides** 集合计算。</span><span class="sxs-lookup"><span data-stu-id="2aa72-122">This is computed from the **authoringLanguages** collection in [regionalAndLanguageSettings](regionalandlanguagesettings.md), and the **languageOverrides** collection in **translationPreferences**.</span></span> <span data-ttu-id="2aa72-123">该列表指定中性区域性值，其中包括没有任何国家/地区关联的语言代码。</span><span class="sxs-lookup"><span data-stu-id="2aa72-123">The list specifies neutral culture values that include the language code without any country or region association.</span></span> <span data-ttu-id="2aa72-124">例如，它会为中性法语区域性指定"fr"，而不是为法国法语指定"fr-FR"。</span><span class="sxs-lookup"><span data-stu-id="2aa72-124">For example, it would specify "fr" for the neutral French culture, but not "fr-FR" for the French culture in France.</span></span> <br><br><span data-ttu-id="2aa72-125">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="2aa72-125">Returned by default.</span></span> <span data-ttu-id="2aa72-126">只读。</span><span class="sxs-lookup"><span data-stu-id="2aa72-126">Read only.</span></span>| 

### <a name="translationbehavior-values"></a><span data-ttu-id="2aa72-127">translationBehavior 值</span><span class="sxs-lookup"><span data-stu-id="2aa72-127">translationBehavior values</span></span>

|<span data-ttu-id="2aa72-128">成员</span><span class="sxs-lookup"><span data-stu-id="2aa72-128">Member</span></span> |<span data-ttu-id="2aa72-129">说明</span><span class="sxs-lookup"><span data-stu-id="2aa72-129">Description</span></span>                                                                  |
|-------|-----------------------------------------------------------------------------|
|<span data-ttu-id="2aa72-130">Ask</span><span class="sxs-lookup"><span data-stu-id="2aa72-130">Ask</span></span>    |<span data-ttu-id="2aa72-131">在翻译用户的消息/聊天/网页之前提示用户。</span><span class="sxs-lookup"><span data-stu-id="2aa72-131">Prompt the user before translating the messages/chats/web pages for the user.</span></span>|
|<span data-ttu-id="2aa72-132">是</span><span class="sxs-lookup"><span data-stu-id="2aa72-132">Yes</span></span>    |<span data-ttu-id="2aa72-133">自动翻译用户的消息/聊天/网页。</span><span class="sxs-lookup"><span data-stu-id="2aa72-133">Automatically translate the messages/chats/web pages for the user.</span></span>           |
|<span data-ttu-id="2aa72-134">否</span><span class="sxs-lookup"><span data-stu-id="2aa72-134">No</span></span>     |<span data-ttu-id="2aa72-135">不要为用户提供提示或自动翻译。</span><span class="sxs-lookup"><span data-stu-id="2aa72-135">Do not offer prompted or automatic translation for the user.</span></span>                 |



## <a name="json-representation"></a><span data-ttu-id="2aa72-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2aa72-136">JSON representation</span></span>

<span data-ttu-id="2aa72-137">下面是资源的 JSON 定义。</span><span class="sxs-lookup"><span data-stu-id="2aa72-137">The following is a JSON definition of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.translationPreferences"
}-->

```json
{
    "translationBehavior": "string",
    "languageOverrides": [{"@odata.type":"microsoft.graph.translationLanguageOverride"}],
    "untranslatedLanguages": ["string"]
}
```
<!-- {
  "type": "#page.annotation",
  "description": translationPreferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


