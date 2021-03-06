---
title: regionalAndLanguageSettings 资源类型
description: 表示用户区域和语言首选项的资源
localization_priority: Normal
author: jasonbro
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: d5fd77038735ed1faa175d77ed2bd10b3b2ef784
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516484"
---
# <a name="regionalandlanguagesettings-resource-type"></a><span data-ttu-id="3f9ab-103">regionalAndLanguageSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f9ab-103">regionalAndLanguageSettings resource type</span></span>

<span data-ttu-id="3f9ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f9ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f9ab-105">一种开放类型，表示用户在各种上下文中的语言首选项，以及驱动默认日历的区域设置和格式设置以及日期和时间的格式设置。</span><span class="sxs-lookup"><span data-stu-id="3f9ab-105">An open type that represents a user's preferences for languages in various contexts, and for regional locale and formatting that drives the default calendar, and formatting for date and time.</span></span>

## <a name="methods"></a><span data-ttu-id="3f9ab-106">方法</span><span class="sxs-lookup"><span data-stu-id="3f9ab-106">Methods</span></span>

| <span data-ttu-id="3f9ab-107">方法</span><span class="sxs-lookup"><span data-stu-id="3f9ab-107">Method</span></span>                                                 | <span data-ttu-id="3f9ab-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3f9ab-108">Return Type</span></span>                                                   | <span data-ttu-id="3f9ab-109">说明</span><span class="sxs-lookup"><span data-stu-id="3f9ab-109">Description</span></span>                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [<span data-ttu-id="3f9ab-110">获取</span><span class="sxs-lookup"><span data-stu-id="3f9ab-110">Get</span></span>](../api/regionalAndLanguageSettings-get.md)       | [<span data-ttu-id="3f9ab-111">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="3f9ab-111">regionalAndLanguageSettings</span></span>](regionalAndLanguageSettings.md) | <span data-ttu-id="3f9ab-112">读取 **regionalAndLanguageSettings 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="3f9ab-112">Read properties of a **regionalAndLanguageSettings** object.</span></span>                                       |
| [<span data-ttu-id="3f9ab-113">更新</span><span class="sxs-lookup"><span data-stu-id="3f9ab-113">Update</span></span>](../api/regionalandlanguagesettings-update.md) | [<span data-ttu-id="3f9ab-114">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="3f9ab-114">regionalAndLanguageSettings</span></span>](regionalAndLanguageSettings.md) | <span data-ttu-id="3f9ab-115">为用户更新 **regionalAndLanguageSettings** 对象的所有属性或部分属性。</span><span class="sxs-lookup"><span data-stu-id="3f9ab-115">Update all or a subset of the properties of the **regionalAndLanguageSettings** object for a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="3f9ab-116">属性</span><span class="sxs-lookup"><span data-stu-id="3f9ab-116">Properties</span></span>
| <span data-ttu-id="3f9ab-117">属性</span><span class="sxs-lookup"><span data-stu-id="3f9ab-117">Property</span></span>                   | <span data-ttu-id="3f9ab-118">类型</span><span class="sxs-lookup"><span data-stu-id="3f9ab-118">Type</span></span>                                                  | <span data-ttu-id="3f9ab-119">说明</span><span class="sxs-lookup"><span data-stu-id="3f9ab-119">Description</span></span>                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="3f9ab-120">defaultDisplayLanguage</span><span class="sxs-lookup"><span data-stu-id="3f9ab-120">defaultDisplayLanguage</span></span>     | [<span data-ttu-id="3f9ab-121">localeInfo</span><span class="sxs-lookup"><span data-stu-id="3f9ab-121">localeInfo</span></span>](localeinfo.md)                           | <span data-ttu-id="3f9ab-122">用户的首选用户界面语言 (菜单、按钮、功能区、警告消息) Microsoft Web 应用程序。</span><span class="sxs-lookup"><span data-stu-id="3f9ab-122">The  user's preferred user interface language (menus, buttons, ribbons, warning messages) for Microsoft web applications.</span></span><br><br><span data-ttu-id="3f9ab-123">默认返回。</span><span class="sxs-lookup"><span data-stu-id="3f9ab-123">Returned by default.</span></span> <span data-ttu-id="3f9ab-124">不可为空。</span><span class="sxs-lookup"><span data-stu-id="3f9ab-124">Not nullable.</span></span> |
| <span data-ttu-id="3f9ab-125">authoringLanguages</span><span class="sxs-lookup"><span data-stu-id="3f9ab-125">authoringLanguages</span></span>         | <span data-ttu-id="3f9ab-126">localeInfo 集合</span><span class="sxs-lookup"><span data-stu-id="3f9ab-126">localeInfo collection</span></span>                                 | <span data-ttu-id="3f9ab-127">用户读取和作者使用的语言的优先级列表。</span><span class="sxs-lookup"><span data-stu-id="3f9ab-127">Prioritized list of languages the user reads and authors in.</span></span><br><br><span data-ttu-id="3f9ab-128">默认返回。</span><span class="sxs-lookup"><span data-stu-id="3f9ab-128">Returned by default.</span></span> <span data-ttu-id="3f9ab-129">不可为空。</span><span class="sxs-lookup"><span data-stu-id="3f9ab-129">Not nullable.</span></span>                                                              |
| <span data-ttu-id="3f9ab-130">defaultTranslationLanguage</span><span class="sxs-lookup"><span data-stu-id="3f9ab-130">defaultTranslationLanguage</span></span> | <span data-ttu-id="3f9ab-131">localeInfo</span><span class="sxs-lookup"><span data-stu-id="3f9ab-131">localeInfo</span></span>                                            | <span data-ttu-id="3f9ab-132">用户期望将文档、电子邮件和邮件翻译为的语言。</span><span class="sxs-lookup"><span data-stu-id="3f9ab-132">The language a user expects to have documents, emails, and messages translated into.</span></span><br><br><span data-ttu-id="3f9ab-133">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="3f9ab-133">Returned by default.</span></span>                                                    |
| <span data-ttu-id="3f9ab-134">defaultSpeechInputLanguage</span><span class="sxs-lookup"><span data-stu-id="3f9ab-134">defaultSpeechInputLanguage</span></span> | <span data-ttu-id="3f9ab-135">localeInfo</span><span class="sxs-lookup"><span data-stu-id="3f9ab-135">localeInfo</span></span>                                            | <span data-ttu-id="3f9ab-136">用户预期用作文本到语音方案输入的语言。</span><span class="sxs-lookup"><span data-stu-id="3f9ab-136">The language a user expected to use as input for text to speech scenarios.</span></span><br><br><span data-ttu-id="3f9ab-137">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="3f9ab-137">Returned by default.</span></span>                                                              |
| <span data-ttu-id="3f9ab-138">defaultRegionalFormat</span><span class="sxs-lookup"><span data-stu-id="3f9ab-138">defaultRegionalFormat</span></span>      | <span data-ttu-id="3f9ab-139">localeInfo</span><span class="sxs-lookup"><span data-stu-id="3f9ab-139">localeInfo</span></span>                                            | <span data-ttu-id="3f9ab-140">驱动默认日期、时间和日历格式设置区域设置。</span><span class="sxs-lookup"><span data-stu-id="3f9ab-140">The locale that drives the default date, time, and calendar formatting.</span></span><br><br><span data-ttu-id="3f9ab-141">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="3f9ab-141">Returned by default.</span></span>                                                                 |
| <span data-ttu-id="3f9ab-142">regionalFormatOverrides</span><span class="sxs-lookup"><span data-stu-id="3f9ab-142">regionalFormatOverrides</span></span>    | [<span data-ttu-id="3f9ab-143">regionalFormatOverrides</span><span class="sxs-lookup"><span data-stu-id="3f9ab-143">regionalFormatOverrides</span></span>](regionalformatoverrides.md) | <span data-ttu-id="3f9ab-144">允许用户使用特定于字段的格式替代其默认RegionalFormat。</span><span class="sxs-lookup"><span data-stu-id="3f9ab-144">Allows a user to override their defaultRegionalFormat with field specific formats.</span></span><br><br><span data-ttu-id="3f9ab-145">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="3f9ab-145">Returned by default.</span></span>                                                      |
| <span data-ttu-id="3f9ab-146">translationPreferences</span><span class="sxs-lookup"><span data-stu-id="3f9ab-146">translationPreferences</span></span>     | [<span data-ttu-id="3f9ab-147">translationPreferences</span><span class="sxs-lookup"><span data-stu-id="3f9ab-147">translationPreferences</span></span>](translationPreferences.md)   | <span data-ttu-id="3f9ab-148">使用翻译的文档、电子邮件、邮件和网站时用户的首选设置。</span><span class="sxs-lookup"><span data-stu-id="3f9ab-148">The user's preferred settings when consuming translated documents, emails, messages, and websites.</span></span><br><br><span data-ttu-id="3f9ab-149">默认返回。</span><span class="sxs-lookup"><span data-stu-id="3f9ab-149">Returned by default.</span></span> <span data-ttu-id="3f9ab-150">不可为空。</span><span class="sxs-lookup"><span data-stu-id="3f9ab-150">Not nullable.</span></span>                                       |

## <a name="json-representation"></a><span data-ttu-id="3f9ab-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f9ab-151">JSON representation</span></span>

<span data-ttu-id="3f9ab-152">下面是资源的 JSON 定义。</span><span class="sxs-lookup"><span data-stu-id="3f9ab-152">The following is a JSON definition of the resource.</span></span>

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings"
} -->

```json
{
    "defaultDisplayLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "authoringLanguages": [{"@odata.type":"microsoft.graph.localeInfo"}],
    "defaultTranslationLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "defaultSpeechInputLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "defaultRegionalFormat": {"@odata.type":"microsoft.graph.localeInfo"},
    "regionalFormatOverrides": {"@odata.type":"microsoft.graph.regionalFormatOverrides"},
    "translationPreferences":{"@odata.type":"microsoft.graph.translationPreferences"}
}
```
<!-- {
  "type": "#page.annotation",
  "description": "regionalAndLanguageSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


