---
title: regionalAndLanguageSettings 资源类型
description: 表示用户区域和语言首选项的资源
localization_priority: Normal
author: jasonbro
ms.prod: settings
doc_type: resourcePageType
ms.openlocfilehash: 0e6178b7d2a461365c759432d62efcffc44cfe6a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073511"
---
# <a name="regionalandlanguagesettings-resource-type"></a><span data-ttu-id="ff336-103">regionalAndLanguageSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff336-103">regionalAndLanguageSettings resource type</span></span>

<span data-ttu-id="ff336-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff336-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff336-105">一种开放类型，表示用户对各种上下文中的语言的首选项，以及用于驱动默认日历的区域区域设置和格式以及日期和时间的格式设置。</span><span class="sxs-lookup"><span data-stu-id="ff336-105">An open type that represents a user's preferences for languages in various contexts, and for regional locale and formatting that drives the default calendar, and formatting for date and time.</span></span>

## <a name="methods"></a><span data-ttu-id="ff336-106">方法</span><span class="sxs-lookup"><span data-stu-id="ff336-106">Methods</span></span>

| <span data-ttu-id="ff336-107">方法</span><span class="sxs-lookup"><span data-stu-id="ff336-107">Method</span></span>                                                 | <span data-ttu-id="ff336-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="ff336-108">Return Type</span></span>                                                   | <span data-ttu-id="ff336-109">说明</span><span class="sxs-lookup"><span data-stu-id="ff336-109">Description</span></span>                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [<span data-ttu-id="ff336-110">Get</span><span class="sxs-lookup"><span data-stu-id="ff336-110">Get</span></span>](../api/regionalAndLanguageSettings-get.md)       | [<span data-ttu-id="ff336-111">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="ff336-111">regionalAndLanguageSettings</span></span>](regionalAndLanguageSettings.md) | <span data-ttu-id="ff336-112">读取 **regionalAndLanguageSettings** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ff336-112">Read properties of a **regionalAndLanguageSettings** object.</span></span>                                       |
| [<span data-ttu-id="ff336-113">更新</span><span class="sxs-lookup"><span data-stu-id="ff336-113">Update</span></span>](../api/regionalandlanguagesettings-update.md) | [<span data-ttu-id="ff336-114">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="ff336-114">regionalAndLanguageSettings</span></span>](regionalAndLanguageSettings.md) | <span data-ttu-id="ff336-115">更新用户的 **regionalAndLanguageSettings** 对象的全部或属性子集。</span><span class="sxs-lookup"><span data-stu-id="ff336-115">Update all or a subset of the properties of the **regionalAndLanguageSettings** object for a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="ff336-116">属性</span><span class="sxs-lookup"><span data-stu-id="ff336-116">Properties</span></span>
| <span data-ttu-id="ff336-117">属性</span><span class="sxs-lookup"><span data-stu-id="ff336-117">Property</span></span>                   | <span data-ttu-id="ff336-118">类型</span><span class="sxs-lookup"><span data-stu-id="ff336-118">Type</span></span>                                                  | <span data-ttu-id="ff336-119">说明</span><span class="sxs-lookup"><span data-stu-id="ff336-119">Description</span></span>                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ff336-120">defaultDisplayLanguage</span><span class="sxs-lookup"><span data-stu-id="ff336-120">defaultDisplayLanguage</span></span>     | [<span data-ttu-id="ff336-121">localeInfo</span><span class="sxs-lookup"><span data-stu-id="ff336-121">localeInfo</span></span>](localeinfo.md)                           | <span data-ttu-id="ff336-122">用户的首选用户界面语言 (适用于 Microsoft web 应用程序的菜单、按钮、功能区、警告消息) 。</span><span class="sxs-lookup"><span data-stu-id="ff336-122">The  user's preferred user interface language (menus, buttons, ribbons, warning messages) for Microsoft web applications.</span></span><br><br><span data-ttu-id="ff336-123">默认返回。</span><span class="sxs-lookup"><span data-stu-id="ff336-123">Returned by default.</span></span> <span data-ttu-id="ff336-124">不可为空。</span><span class="sxs-lookup"><span data-stu-id="ff336-124">Not nullable.</span></span> |
| <span data-ttu-id="ff336-125">authoringLanguages</span><span class="sxs-lookup"><span data-stu-id="ff336-125">authoringLanguages</span></span>         | <span data-ttu-id="ff336-126">localeInfo 集合</span><span class="sxs-lookup"><span data-stu-id="ff336-126">localeInfo collection</span></span>                                 | <span data-ttu-id="ff336-127">用户读取和作者的语言的优先顺序列表。</span><span class="sxs-lookup"><span data-stu-id="ff336-127">Prioritized list of languages the user reads and authors in.</span></span><br><br><span data-ttu-id="ff336-128">默认返回。</span><span class="sxs-lookup"><span data-stu-id="ff336-128">Returned by default.</span></span> <span data-ttu-id="ff336-129">不可为空。</span><span class="sxs-lookup"><span data-stu-id="ff336-129">Not nullable.</span></span>                                                              |
| <span data-ttu-id="ff336-130">defaultTranslationLanguage</span><span class="sxs-lookup"><span data-stu-id="ff336-130">defaultTranslationLanguage</span></span> | <span data-ttu-id="ff336-131">localeInfo</span><span class="sxs-lookup"><span data-stu-id="ff336-131">localeInfo</span></span>                                            | <span data-ttu-id="ff336-132">用户希望将文档、电子邮件和邮件翻译为的语言。</span><span class="sxs-lookup"><span data-stu-id="ff336-132">The language a user expects to have documents, emails, and messages translated into.</span></span><br><br><span data-ttu-id="ff336-133">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="ff336-133">Returned by default.</span></span>                                                    |
| <span data-ttu-id="ff336-134">defaultSpeechInputLanguage</span><span class="sxs-lookup"><span data-stu-id="ff336-134">defaultSpeechInputLanguage</span></span> | <span data-ttu-id="ff336-135">localeInfo</span><span class="sxs-lookup"><span data-stu-id="ff336-135">localeInfo</span></span>                                            | <span data-ttu-id="ff336-136">用户预期用作语音文本到语音方案的输入的语言。</span><span class="sxs-lookup"><span data-stu-id="ff336-136">The language a user expected to use as input for text to speech scenarios.</span></span><br><br><span data-ttu-id="ff336-137">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="ff336-137">Returned by default.</span></span>                                                              |
| <span data-ttu-id="ff336-138">defaultRegionalFormat</span><span class="sxs-lookup"><span data-stu-id="ff336-138">defaultRegionalFormat</span></span>      | <span data-ttu-id="ff336-139">localeInfo</span><span class="sxs-lookup"><span data-stu-id="ff336-139">localeInfo</span></span>                                            | <span data-ttu-id="ff336-140">驱动默认的日期、时间和日历格式的区域设置。</span><span class="sxs-lookup"><span data-stu-id="ff336-140">The locale that drives the default date, time, and calendar formatting.</span></span><br><br><span data-ttu-id="ff336-141">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="ff336-141">Returned by default.</span></span>                                                                 |
| <span data-ttu-id="ff336-142">regionalFormatOverrides</span><span class="sxs-lookup"><span data-stu-id="ff336-142">regionalFormatOverrides</span></span>    | [<span data-ttu-id="ff336-143">regionalFormatOverrides</span><span class="sxs-lookup"><span data-stu-id="ff336-143">regionalFormatOverrides</span></span>](regionalformatoverrides.md) | <span data-ttu-id="ff336-144">允许用户使用特定于字段的格式替代其 defaultRegionalFormat。</span><span class="sxs-lookup"><span data-stu-id="ff336-144">Allows a user to override their defaultRegionalFormat with field specific formats.</span></span><br><br><span data-ttu-id="ff336-145">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="ff336-145">Returned by default.</span></span>                                                      |

## <a name="json-representation"></a><span data-ttu-id="ff336-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff336-146">JSON representation</span></span>

<span data-ttu-id="ff336-147">下面是资源的 JSON 定义。</span><span class="sxs-lookup"><span data-stu-id="ff336-147">The following is a JSON definition of the resource.</span></span>

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings"
} -->

```json
{
    "defaultDisplayLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "authoringLanguages":[{"@odata.type":"microsoft.graph.localeInfo"}] ,
    "defaultTranslationLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "defaultSpeechInputLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "defaultRegionalFormat":{"@odata.type":"microsoft.graph.localeInfo"} ,
    "regionalFormatOverrides":{"@odata.type":"microsoft.graph.regionalFormatOverrides"}
}
```
<!-- {
  "type": "#page.annotation",
  "description": "regionalAndLanguageSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


