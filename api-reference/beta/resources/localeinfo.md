---
title: localeInfo 资源类型
description: 有关已登录用户的区域设置信息，包括首选语言和国家/地区。
localization_priority: Normal
ms.openlocfilehash: cfd5b0e318a2f78d382dccd10b23da167d8b5c8a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888198"
---
# <a name="localeinfo-resource-type"></a><span data-ttu-id="366d1-103">localeInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="366d1-103">localeInfo resource type</span></span>

> <span data-ttu-id="366d1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="366d1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="366d1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="366d1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="366d1-106">有关已登录用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="366d1-106">Information about the locale, including the preferred language and country/region, of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="366d1-107">属性</span><span class="sxs-lookup"><span data-stu-id="366d1-107">Properties</span></span>
| <span data-ttu-id="366d1-108">属性</span><span class="sxs-lookup"><span data-stu-id="366d1-108">Property</span></span>     | <span data-ttu-id="366d1-109">类型</span><span class="sxs-lookup"><span data-stu-id="366d1-109">Type</span></span>   |<span data-ttu-id="366d1-110">说明</span><span class="sxs-lookup"><span data-stu-id="366d1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="366d1-111">区域设置</span><span class="sxs-lookup"><span data-stu-id="366d1-111">locale</span></span>|<span data-ttu-id="366d1-112">string</span><span class="sxs-lookup"><span data-stu-id="366d1-112">string</span></span>|<span data-ttu-id="366d1-p102">用户的区域设置表示形式，其中包括用户的首选语言和国家/地区。例如，“en-us”。根据 [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm) 中的定义，语言组件前面是 2 个字母的代码；根据 [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm) 中的定义，国家/地区组件前面是 2 个字母的代码。</span><span class="sxs-lookup"><span data-stu-id="366d1-p102">A locale representation for the user, which includes the user's preferred language and country/region. For example, "en-us". The language component follows 2-letter codes as defined in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), and the country component follows 2-letter codes as defined in [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span></span>|
|<span data-ttu-id="366d1-116">displayName</span><span class="sxs-lookup"><span data-stu-id="366d1-116">displayName</span></span>|<span data-ttu-id="366d1-117">string</span><span class="sxs-lookup"><span data-stu-id="366d1-117">string</span></span>|<span data-ttu-id="366d1-118">用自然语言表示用户区域设置的名称，例如“English (United States)”。</span><span class="sxs-lookup"><span data-stu-id="366d1-118">A name representing the user's locale in natural language, for example, "English (United States)".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="366d1-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="366d1-119">JSON representation</span></span>

<span data-ttu-id="366d1-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="366d1-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.localeInfo"
}-->

```json
{
  "locale": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "localeInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
