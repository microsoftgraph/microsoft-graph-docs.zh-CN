---
title: settingTemplateValue 资源类型
description: 如果该设置未被实例化，则表示单独的模板设置定义，包括设置的默认值。
localization_priority: Normal
ms.openlocfilehash: e941630ab72363db1c4be40079cf2af9e40ff002
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811863"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="99ac0-103">settingTemplateValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="99ac0-103">settingTemplateValue resource type</span></span>

> <span data-ttu-id="99ac0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="99ac0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99ac0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="99ac0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99ac0-106">如果该设置未被实例化，则表示单独的模板设置定义，包括设置的默认值。</span><span class="sxs-lookup"><span data-stu-id="99ac0-106">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="99ac0-107">属性</span><span class="sxs-lookup"><span data-stu-id="99ac0-107">Properties</span></span>
| <span data-ttu-id="99ac0-108">属性</span><span class="sxs-lookup"><span data-stu-id="99ac0-108">Property</span></span>     | <span data-ttu-id="99ac0-109">类型</span><span class="sxs-lookup"><span data-stu-id="99ac0-109">Type</span></span>   |<span data-ttu-id="99ac0-110">说明</span><span class="sxs-lookup"><span data-stu-id="99ac0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99ac0-111">defaultValue</span><span class="sxs-lookup"><span data-stu-id="99ac0-111">defaultValue</span></span>|<span data-ttu-id="99ac0-112">string</span><span class="sxs-lookup"><span data-stu-id="99ac0-112">string</span></span>|<span data-ttu-id="99ac0-113">设置的默认值。</span><span class="sxs-lookup"><span data-stu-id="99ac0-113">Default value for the setting.</span></span> <span data-ttu-id="99ac0-114">只读。</span><span class="sxs-lookup"><span data-stu-id="99ac0-114">Read-only.</span></span>|
|<span data-ttu-id="99ac0-115">说明</span><span class="sxs-lookup"><span data-stu-id="99ac0-115">description</span></span>|<span data-ttu-id="99ac0-116">string</span><span class="sxs-lookup"><span data-stu-id="99ac0-116">string</span></span>|<span data-ttu-id="99ac0-117">设置的说明。</span><span class="sxs-lookup"><span data-stu-id="99ac0-117">Description of the setting.</span></span> <span data-ttu-id="99ac0-118">只读。</span><span class="sxs-lookup"><span data-stu-id="99ac0-118">Read-only.</span></span>|
|<span data-ttu-id="99ac0-119">name</span><span class="sxs-lookup"><span data-stu-id="99ac0-119">name</span></span>|<span data-ttu-id="99ac0-120">string</span><span class="sxs-lookup"><span data-stu-id="99ac0-120">string</span></span>|<span data-ttu-id="99ac0-121">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="99ac0-121">Name of the setting.</span></span> <span data-ttu-id="99ac0-122">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="99ac0-122">Read-only.</span></span>|
|<span data-ttu-id="99ac0-123">type</span><span class="sxs-lookup"><span data-stu-id="99ac0-123">type</span></span>|<span data-ttu-id="99ac0-124">string</span><span class="sxs-lookup"><span data-stu-id="99ac0-124">string</span></span>|<span data-ttu-id="99ac0-125">设置的类型。</span><span class="sxs-lookup"><span data-stu-id="99ac0-125">Type of the setting.</span></span> <span data-ttu-id="99ac0-126">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="99ac0-126">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99ac0-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99ac0-127">JSON representation</span></span>

<span data-ttu-id="99ac0-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99ac0-128">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
