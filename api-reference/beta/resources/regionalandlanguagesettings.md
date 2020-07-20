---
title: regionalAndLanguageSettings 资源类型
description: 表示用户区域和语言首选项的资源
localization_priority: Normal
author: jasonbro
ms.prod: settings
doc_type: resourcePageType
ms.openlocfilehash: ba8666b78023b7345d936516fc3aec2b116520ad
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845678"
---
# <a name="regionalandlanguagesettings-resource-type"></a><span data-ttu-id="0728b-103">regionalAndLanguageSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="0728b-103">regionalAndLanguageSettings resource type</span></span>

<span data-ttu-id="0728b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0728b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0728b-105">一种开放类型，表示用户对各种上下文中的语言的首选项，以及用于驱动默认日历的区域区域设置和格式以及日期和时间的格式设置。</span><span class="sxs-lookup"><span data-stu-id="0728b-105">An open type that represents a user's preferences for languages in various contexts, and for regional locale and formatting that drives the default calendar, and formatting for date and time.</span></span>

## <a name="methods"></a><span data-ttu-id="0728b-106">Methods</span><span class="sxs-lookup"><span data-stu-id="0728b-106">Methods</span></span>

| <span data-ttu-id="0728b-107">方法</span><span class="sxs-lookup"><span data-stu-id="0728b-107">Method</span></span>                                                 | <span data-ttu-id="0728b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="0728b-108">Return Type</span></span>                                                   | <span data-ttu-id="0728b-109">说明</span><span class="sxs-lookup"><span data-stu-id="0728b-109">Description</span></span>                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [<span data-ttu-id="0728b-110">获取</span><span class="sxs-lookup"><span data-stu-id="0728b-110">Get</span></span>](../api/regionalAndLanguageSettings-get.md)       | [<span data-ttu-id="0728b-111">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="0728b-111">regionalAndLanguageSettings</span></span>](regionalAndLanguageSettings.md) | <span data-ttu-id="0728b-112">读取**regionalAndLanguageSettings**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0728b-112">Read properties of a **regionalAndLanguageSettings** object.</span></span>                                       |
| [<span data-ttu-id="0728b-113">更新</span><span class="sxs-lookup"><span data-stu-id="0728b-113">Update</span></span>](../api/regionalandlanguagesettings-update.md) | [<span data-ttu-id="0728b-114">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="0728b-114">regionalAndLanguageSettings</span></span>](regionalAndLanguageSettings.md) | <span data-ttu-id="0728b-115">更新用户的**regionalAndLanguageSettings**对象的全部或属性子集。</span><span class="sxs-lookup"><span data-stu-id="0728b-115">Update all or a subset of the properties of the **regionalAndLanguageSettings** object for a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="0728b-116">属性</span><span class="sxs-lookup"><span data-stu-id="0728b-116">Properties</span></span>
| <span data-ttu-id="0728b-117">属性</span><span class="sxs-lookup"><span data-stu-id="0728b-117">Property</span></span>                   | <span data-ttu-id="0728b-118">类型</span><span class="sxs-lookup"><span data-stu-id="0728b-118">Type</span></span>                                                  | <span data-ttu-id="0728b-119">Description</span><span class="sxs-lookup"><span data-stu-id="0728b-119">Description</span></span>                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0728b-120">defaultDisplayLanguage</span><span class="sxs-lookup"><span data-stu-id="0728b-120">defaultDisplayLanguage</span></span>     | [<span data-ttu-id="0728b-121">localeInfo</span><span class="sxs-lookup"><span data-stu-id="0728b-121">localeInfo</span></span>](localeinfo.md)                           | <span data-ttu-id="0728b-122">适用于 Microsoft web 应用程序的用户首选用户界面语言（菜单、按钮、功能区、警告消息）。</span><span class="sxs-lookup"><span data-stu-id="0728b-122">The  user's preferred user interface language (menus, buttons, ribbons, warning messages) for Microsoft web applications.</span></span><br><br><span data-ttu-id="0728b-123">默认返回。</span><span class="sxs-lookup"><span data-stu-id="0728b-123">Returned by default.</span></span> <span data-ttu-id="0728b-124">不可为空。</span><span class="sxs-lookup"><span data-stu-id="0728b-124">Not nullable.</span></span> |
| <span data-ttu-id="0728b-125">authoringLanguages</span><span class="sxs-lookup"><span data-stu-id="0728b-125">authoringLanguages</span></span>         | <span data-ttu-id="0728b-126">localeInfo 集合</span><span class="sxs-lookup"><span data-stu-id="0728b-126">localeInfo collection</span></span>                                 | <span data-ttu-id="0728b-127">用户读取和作者的语言的优先顺序列表。</span><span class="sxs-lookup"><span data-stu-id="0728b-127">Prioritized list of languages the user reads and authors in.</span></span><br><br><span data-ttu-id="0728b-128">默认返回。</span><span class="sxs-lookup"><span data-stu-id="0728b-128">Returned by default.</span></span> <span data-ttu-id="0728b-129">不可为空。</span><span class="sxs-lookup"><span data-stu-id="0728b-129">Not nullable.</span></span>                                                              |
| <span data-ttu-id="0728b-130">defaultTranslationLanguage</span><span class="sxs-lookup"><span data-stu-id="0728b-130">defaultTranslationLanguage</span></span> | <span data-ttu-id="0728b-131">localeInfo</span><span class="sxs-lookup"><span data-stu-id="0728b-131">localeInfo</span></span>                                            | <span data-ttu-id="0728b-132">用户希望将文档、电子邮件和邮件翻译为的语言。</span><span class="sxs-lookup"><span data-stu-id="0728b-132">The language a user expects to have documents, emails, and messages translated into.</span></span><br><br><span data-ttu-id="0728b-133">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="0728b-133">Returned by default.</span></span>                                                    |
| <span data-ttu-id="0728b-134">defaultSpeechInputLanguage</span><span class="sxs-lookup"><span data-stu-id="0728b-134">defaultSpeechInputLanguage</span></span> | <span data-ttu-id="0728b-135">localeInfo</span><span class="sxs-lookup"><span data-stu-id="0728b-135">localeInfo</span></span>                                            | <span data-ttu-id="0728b-136">用户预期用作语音文本到语音方案的输入的语言。</span><span class="sxs-lookup"><span data-stu-id="0728b-136">The language a user expected to use as input for text to speech scenarios.</span></span><br><br><span data-ttu-id="0728b-137">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="0728b-137">Returned by default.</span></span>                                                              |
| <span data-ttu-id="0728b-138">defaultRegionalFormat</span><span class="sxs-lookup"><span data-stu-id="0728b-138">defaultRegionalFormat</span></span>      | <span data-ttu-id="0728b-139">localeInfo</span><span class="sxs-lookup"><span data-stu-id="0728b-139">localeInfo</span></span>                                            | <span data-ttu-id="0728b-140">驱动默认的日期、时间和日历格式的区域设置。</span><span class="sxs-lookup"><span data-stu-id="0728b-140">The locale that drives the default date, time, and calendar formatting.</span></span><br><br><span data-ttu-id="0728b-141">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="0728b-141">Returned by default.</span></span>                                                                 |
| <span data-ttu-id="0728b-142">regionalFormatOverrides</span><span class="sxs-lookup"><span data-stu-id="0728b-142">regionalFormatOverrides</span></span>    | [<span data-ttu-id="0728b-143">regionalFormatOverrides</span><span class="sxs-lookup"><span data-stu-id="0728b-143">regionalFormatOverrides</span></span>](regionalformatoverrides.md) | <span data-ttu-id="0728b-144">允许用户使用特定于字段的格式替代其 defaultRegionalFormat。</span><span class="sxs-lookup"><span data-stu-id="0728b-144">Allows a user to override their defaultRegionalFormat with field specific formats.</span></span><br><br><span data-ttu-id="0728b-145">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="0728b-145">Returned by default.</span></span>                                                      |

## <a name="json-representation"></a><span data-ttu-id="0728b-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0728b-146">JSON representation</span></span>

<span data-ttu-id="0728b-147">下面是资源的 JSON 定义。</span><span class="sxs-lookup"><span data-stu-id="0728b-147">The following is a JSON definition of the resource.</span></span>

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
