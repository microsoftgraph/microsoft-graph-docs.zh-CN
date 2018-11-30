---
title: localeInfo 资源类型
description: 有关已登录用户的区域设置信息，包括首选语言和国家/地区。
ms.openlocfilehash: f61f1af1d4ad49b1083403576ac4069d97d694cb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011605"
---
# <a name="localeinfo-resource-type"></a><span data-ttu-id="e43a7-103">localeInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="e43a7-103">localeInfo resource type</span></span>

<span data-ttu-id="e43a7-104">有关已登录用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="e43a7-104">Information about the locale, including the preferred language and country/region, of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="e43a7-105">属性</span><span class="sxs-lookup"><span data-stu-id="e43a7-105">Properties</span></span>
| <span data-ttu-id="e43a7-106">属性</span><span class="sxs-lookup"><span data-stu-id="e43a7-106">Property</span></span>     | <span data-ttu-id="e43a7-107">类型</span><span class="sxs-lookup"><span data-stu-id="e43a7-107">Type</span></span>   |<span data-ttu-id="e43a7-108">说明</span><span class="sxs-lookup"><span data-stu-id="e43a7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e43a7-109">区域设置</span><span class="sxs-lookup"><span data-stu-id="e43a7-109">locale</span></span>|<span data-ttu-id="e43a7-110">string</span><span class="sxs-lookup"><span data-stu-id="e43a7-110">string</span></span>|<span data-ttu-id="e43a7-p101">用户的区域设置表示形式，其中包括用户的首选语言和国家/地区。例如，“en-us”。根据 [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm) 中的定义，语言组件前面是 2 个字母的代码；根据 [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm) 中的定义，国家/地区组件前面是 2 个字母的代码。</span><span class="sxs-lookup"><span data-stu-id="e43a7-p101">A locale representation for the user, which includes the user's preferred language and country/region. For example, "en-us". The language component follows 2-letter codes as defined in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), and the country component follows 2-letter codes as defined in [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span></span>|
|<span data-ttu-id="e43a7-114">displayName</span><span class="sxs-lookup"><span data-stu-id="e43a7-114">displayName</span></span>|<span data-ttu-id="e43a7-115">string</span><span class="sxs-lookup"><span data-stu-id="e43a7-115">string</span></span>|<span data-ttu-id="e43a7-116">用自然语言表示用户区域设置的名称，例如“English (United States)”。</span><span class="sxs-lookup"><span data-stu-id="e43a7-116">A name representing the user's locale in natural language, for example, "English (United States)".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e43a7-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e43a7-117">JSON representation</span></span>

<span data-ttu-id="e43a7-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e43a7-118">Here is a JSON representation of the resource.</span></span>

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