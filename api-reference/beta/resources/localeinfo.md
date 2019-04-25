---
title: localeInfo 资源类型
description: 有关已登录用户的区域设置信息，包括首选语言和国家/地区。
localization_priority: Normal
ms.openlocfilehash: 7414130c1ed1e85353c653d9bbd36a0e488bcea9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578150"
---
# <a name="localeinfo-resource-type"></a><span data-ttu-id="64039-103">localeInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="64039-103">localeInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64039-104">有关已登录用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="64039-104">Information about the locale, including the preferred language and country/region, of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="64039-105">属性</span><span class="sxs-lookup"><span data-stu-id="64039-105">Properties</span></span>
| <span data-ttu-id="64039-106">属性</span><span class="sxs-lookup"><span data-stu-id="64039-106">Property</span></span>     | <span data-ttu-id="64039-107">类型</span><span class="sxs-lookup"><span data-stu-id="64039-107">Type</span></span>   |<span data-ttu-id="64039-108">说明</span><span class="sxs-lookup"><span data-stu-id="64039-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64039-109">区域设置</span><span class="sxs-lookup"><span data-stu-id="64039-109">locale</span></span>|<span data-ttu-id="64039-110">string</span><span class="sxs-lookup"><span data-stu-id="64039-110">string</span></span>|<span data-ttu-id="64039-p101">用户的区域设置表示形式，其中包括用户的首选语言和国家/地区。例如，“en-us”。根据 [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm) 中的定义，语言组件前面是 2 个字母的代码；根据 [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm) 中的定义，国家/地区组件前面是 2 个字母的代码。</span><span class="sxs-lookup"><span data-stu-id="64039-p101">A locale representation for the user, which includes the user's preferred language and country/region. For example, "en-us". The language component follows 2-letter codes as defined in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), and the country component follows 2-letter codes as defined in [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span></span>|
|<span data-ttu-id="64039-114">displayName</span><span class="sxs-lookup"><span data-stu-id="64039-114">displayName</span></span>|<span data-ttu-id="64039-115">string</span><span class="sxs-lookup"><span data-stu-id="64039-115">string</span></span>|<span data-ttu-id="64039-116">用自然语言表示用户区域设置的名称，例如“English (United States)”。</span><span class="sxs-lookup"><span data-stu-id="64039-116">A name representing the user's locale in natural language, for example, "English (United States)".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="64039-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64039-117">JSON representation</span></span>

<span data-ttu-id="64039-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64039-118">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "localeInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/localeinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
