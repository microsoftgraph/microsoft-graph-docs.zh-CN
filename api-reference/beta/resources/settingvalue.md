---
title: settingValue 资源类型
description: 由名称/值对表示的设置。
localization_priority: Normal
ms.openlocfilehash: aa30fd61c1498be08be4d87175d18015c58323ba
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584094"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="2d23d-103">settingValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="2d23d-103">settingValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d23d-104">由名称/值对表示的设置。</span><span class="sxs-lookup"><span data-stu-id="2d23d-104">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="2d23d-105">属性</span><span class="sxs-lookup"><span data-stu-id="2d23d-105">Properties</span></span>
| <span data-ttu-id="2d23d-106">属性</span><span class="sxs-lookup"><span data-stu-id="2d23d-106">Property</span></span>     | <span data-ttu-id="2d23d-107">类型</span><span class="sxs-lookup"><span data-stu-id="2d23d-107">Type</span></span>   |<span data-ttu-id="2d23d-108">说明</span><span class="sxs-lookup"><span data-stu-id="2d23d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d23d-109">name</span><span class="sxs-lookup"><span data-stu-id="2d23d-109">name</span></span>|<span data-ttu-id="2d23d-110">string</span><span class="sxs-lookup"><span data-stu-id="2d23d-110">string</span></span>|<span data-ttu-id="2d23d-111">设置的名称 (由 directorySettingTemplate 定义)。</span><span class="sxs-lookup"><span data-stu-id="2d23d-111">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="2d23d-112">value</span><span class="sxs-lookup"><span data-stu-id="2d23d-112">value</span></span>|<span data-ttu-id="2d23d-113">string</span><span class="sxs-lookup"><span data-stu-id="2d23d-113">string</span></span>|<span data-ttu-id="2d23d-114">设置的值。</span><span class="sxs-lookup"><span data-stu-id="2d23d-114">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d23d-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d23d-115">JSON representation</span></span>

<span data-ttu-id="2d23d-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d23d-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/settingvalue.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
