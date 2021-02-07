---
title: localeInfo 资源类型
description: 有关已登录用户的区域设置信息，包括首选语言和国家/地区。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 893d0985d72eb74b6850652ae375f336df1abe1a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131668"
---
# <a name="localeinfo-resource-type"></a><span data-ttu-id="12784-103">localeInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="12784-103">localeInfo resource type</span></span>

<span data-ttu-id="12784-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12784-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="12784-105">有关已登录用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="12784-105">Information about the locale, including the preferred language and country/region, of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="12784-106">属性</span><span class="sxs-lookup"><span data-stu-id="12784-106">Properties</span></span>
| <span data-ttu-id="12784-107">属性</span><span class="sxs-lookup"><span data-stu-id="12784-107">Property</span></span>     | <span data-ttu-id="12784-108">类型</span><span class="sxs-lookup"><span data-stu-id="12784-108">Type</span></span>   |<span data-ttu-id="12784-109">说明</span><span class="sxs-lookup"><span data-stu-id="12784-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12784-110">区域设置</span><span class="sxs-lookup"><span data-stu-id="12784-110">locale</span></span>|<span data-ttu-id="12784-111">string</span><span class="sxs-lookup"><span data-stu-id="12784-111">string</span></span>|<span data-ttu-id="12784-p101">用户的区域设置表示形式，其中包括用户的首选语言和国家/地区。例如，“en-us”。根据 [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm) 中的定义，语言组件前面是 2 个字母的代码；根据 [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm) 中的定义，国家/地区组件前面是 2 个字母的代码。</span><span class="sxs-lookup"><span data-stu-id="12784-p101">A locale representation for the user, which includes the user's preferred language and country/region. For example, "en-us". The language component follows 2-letter codes as defined in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), and the country component follows 2-letter codes as defined in [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span></span>|
|<span data-ttu-id="12784-115">displayName</span><span class="sxs-lookup"><span data-stu-id="12784-115">displayName</span></span>|<span data-ttu-id="12784-116">string</span><span class="sxs-lookup"><span data-stu-id="12784-116">string</span></span>|<span data-ttu-id="12784-117">用自然语言表示用户区域设置的名称，例如“English (United States)”。</span><span class="sxs-lookup"><span data-stu-id="12784-117">A name representing the user's locale in natural language, for example, "English (United States)".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12784-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12784-118">JSON representation</span></span>

<span data-ttu-id="12784-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12784-119">Here is a JSON representation of the resource.</span></span>

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

