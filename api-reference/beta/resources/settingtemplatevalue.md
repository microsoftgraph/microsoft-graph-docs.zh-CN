---
title: settingTemplateValue 资源类型
description: 表示单个模板设置定义, 包括设置的默认值 (如果未实例化设置)。
localization_priority: Normal
ms.openlocfilehash: 80b640419eb2084888dcd6887ece54b4fd4bdf3c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583675"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="99468-103">settingTemplateValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="99468-103">settingTemplateValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99468-104">表示单个模板设置定义, 包括设置的默认值 (如果未实例化设置)。</span><span class="sxs-lookup"><span data-stu-id="99468-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="99468-105">属性</span><span class="sxs-lookup"><span data-stu-id="99468-105">Properties</span></span>
| <span data-ttu-id="99468-106">属性</span><span class="sxs-lookup"><span data-stu-id="99468-106">Property</span></span>     | <span data-ttu-id="99468-107">类型</span><span class="sxs-lookup"><span data-stu-id="99468-107">Type</span></span>   |<span data-ttu-id="99468-108">说明</span><span class="sxs-lookup"><span data-stu-id="99468-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99468-109">默认</span><span class="sxs-lookup"><span data-stu-id="99468-109">defaultValue</span></span>|<span data-ttu-id="99468-110">string</span><span class="sxs-lookup"><span data-stu-id="99468-110">string</span></span>|<span data-ttu-id="99468-111">设置的默认值。</span><span class="sxs-lookup"><span data-stu-id="99468-111">Default value for the setting.</span></span> <span data-ttu-id="99468-112">只读。</span><span class="sxs-lookup"><span data-stu-id="99468-112">Read-only.</span></span>|
|<span data-ttu-id="99468-113">说明</span><span class="sxs-lookup"><span data-stu-id="99468-113">description</span></span>|<span data-ttu-id="99468-114">string</span><span class="sxs-lookup"><span data-stu-id="99468-114">string</span></span>|<span data-ttu-id="99468-115">设置的说明。</span><span class="sxs-lookup"><span data-stu-id="99468-115">Description of the setting.</span></span> <span data-ttu-id="99468-116">只读。</span><span class="sxs-lookup"><span data-stu-id="99468-116">Read-only.</span></span>|
|<span data-ttu-id="99468-117">name</span><span class="sxs-lookup"><span data-stu-id="99468-117">name</span></span>|<span data-ttu-id="99468-118">string</span><span class="sxs-lookup"><span data-stu-id="99468-118">string</span></span>|<span data-ttu-id="99468-119">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="99468-119">Name of the setting.</span></span> <span data-ttu-id="99468-120">只读。</span><span class="sxs-lookup"><span data-stu-id="99468-120">Read-only.</span></span>|
|<span data-ttu-id="99468-121">类型</span><span class="sxs-lookup"><span data-stu-id="99468-121">type</span></span>|<span data-ttu-id="99468-122">string</span><span class="sxs-lookup"><span data-stu-id="99468-122">string</span></span>|<span data-ttu-id="99468-123">设置的类型。</span><span class="sxs-lookup"><span data-stu-id="99468-123">Type of the setting.</span></span> <span data-ttu-id="99468-124">只读。</span><span class="sxs-lookup"><span data-stu-id="99468-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99468-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99468-125">JSON representation</span></span>

<span data-ttu-id="99468-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99468-126">Here is a JSON representation of the resource.</span></span>

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
