---
title: settingTemplateValue 资源类型
description: 如果该设置未被实例化，则表示单独的模板设置定义，包括设置的默认值。
localization_priority: Normal
ms.openlocfilehash: 80b640419eb2084888dcd6887ece54b4fd4bdf3c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528009"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="a53be-103">settingTemplateValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="a53be-103">settingTemplateValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a53be-104">如果该设置未被实例化，则表示单独的模板设置定义，包括设置的默认值。</span><span class="sxs-lookup"><span data-stu-id="a53be-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="a53be-105">属性</span><span class="sxs-lookup"><span data-stu-id="a53be-105">Properties</span></span>
| <span data-ttu-id="a53be-106">属性</span><span class="sxs-lookup"><span data-stu-id="a53be-106">Property</span></span>     | <span data-ttu-id="a53be-107">类型</span><span class="sxs-lookup"><span data-stu-id="a53be-107">Type</span></span>   |<span data-ttu-id="a53be-108">说明</span><span class="sxs-lookup"><span data-stu-id="a53be-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a53be-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="a53be-109">defaultValue</span></span>|<span data-ttu-id="a53be-110">string</span><span class="sxs-lookup"><span data-stu-id="a53be-110">string</span></span>|<span data-ttu-id="a53be-111">设置的默认值。</span><span class="sxs-lookup"><span data-stu-id="a53be-111">Default value for the setting.</span></span> <span data-ttu-id="a53be-112">只读。</span><span class="sxs-lookup"><span data-stu-id="a53be-112">Read-only.</span></span>|
|<span data-ttu-id="a53be-113">说明</span><span class="sxs-lookup"><span data-stu-id="a53be-113">description</span></span>|<span data-ttu-id="a53be-114">string</span><span class="sxs-lookup"><span data-stu-id="a53be-114">string</span></span>|<span data-ttu-id="a53be-115">设置的说明。</span><span class="sxs-lookup"><span data-stu-id="a53be-115">Description of the setting.</span></span> <span data-ttu-id="a53be-116">只读。</span><span class="sxs-lookup"><span data-stu-id="a53be-116">Read-only.</span></span>|
|<span data-ttu-id="a53be-117">name</span><span class="sxs-lookup"><span data-stu-id="a53be-117">name</span></span>|<span data-ttu-id="a53be-118">string</span><span class="sxs-lookup"><span data-stu-id="a53be-118">string</span></span>|<span data-ttu-id="a53be-119">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="a53be-119">Name of the setting.</span></span> <span data-ttu-id="a53be-120">只读。</span><span class="sxs-lookup"><span data-stu-id="a53be-120">Read-only.</span></span>|
|<span data-ttu-id="a53be-121">type</span><span class="sxs-lookup"><span data-stu-id="a53be-121">type</span></span>|<span data-ttu-id="a53be-122">字符串</span><span class="sxs-lookup"><span data-stu-id="a53be-122">string</span></span>|<span data-ttu-id="a53be-123">设置的类型。</span><span class="sxs-lookup"><span data-stu-id="a53be-123">Type of the setting.</span></span> <span data-ttu-id="a53be-124">只读。</span><span class="sxs-lookup"><span data-stu-id="a53be-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a53be-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a53be-125">JSON representation</span></span>

<span data-ttu-id="a53be-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a53be-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "string",
  "description": "string",
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/settingtemplatevalue.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
