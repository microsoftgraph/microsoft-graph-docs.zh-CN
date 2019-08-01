---
title: settingTemplateValue 资源类型
description: 表示单个模板设置定义, 包括设置的默认值 (如果未实例化设置)。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f4ac39001e260d7f65b3a593d90976f94acd4693
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034389"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="05482-103">settingTemplateValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="05482-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="05482-104">表示单个模板设置定义, 包括设置的默认值 (如果未实例化设置)。</span><span class="sxs-lookup"><span data-stu-id="05482-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="05482-105">属性</span><span class="sxs-lookup"><span data-stu-id="05482-105">Properties</span></span>

| <span data-ttu-id="05482-106">属性</span><span class="sxs-lookup"><span data-stu-id="05482-106">Property</span></span> | <span data-ttu-id="05482-107">类型</span><span class="sxs-lookup"><span data-stu-id="05482-107">Type</span></span> | <span data-ttu-id="05482-108">说明</span><span class="sxs-lookup"><span data-stu-id="05482-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="05482-109">默认</span><span class="sxs-lookup"><span data-stu-id="05482-109">defaultValue</span></span>|<span data-ttu-id="05482-110">String</span><span class="sxs-lookup"><span data-stu-id="05482-110">String</span></span>| <span data-ttu-id="05482-111">设置的默认值。</span><span class="sxs-lookup"><span data-stu-id="05482-111">Default value for the setting.</span></span> |
|<span data-ttu-id="05482-112">说明</span><span class="sxs-lookup"><span data-stu-id="05482-112">description</span></span>|<span data-ttu-id="05482-113">String</span><span class="sxs-lookup"><span data-stu-id="05482-113">String</span></span>| <span data-ttu-id="05482-114">设置的说明。</span><span class="sxs-lookup"><span data-stu-id="05482-114">Description of the setting.</span></span> |
|<span data-ttu-id="05482-115">name</span><span class="sxs-lookup"><span data-stu-id="05482-115">name</span></span>|<span data-ttu-id="05482-116">String</span><span class="sxs-lookup"><span data-stu-id="05482-116">String</span></span>| <span data-ttu-id="05482-117">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="05482-117">Name of the setting.</span></span> |
|<span data-ttu-id="05482-118">type</span><span class="sxs-lookup"><span data-stu-id="05482-118">type</span></span>|<span data-ttu-id="05482-119">String</span><span class="sxs-lookup"><span data-stu-id="05482-119">String</span></span>| <span data-ttu-id="05482-120">设置的类型。</span><span class="sxs-lookup"><span data-stu-id="05482-120">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="05482-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05482-121">JSON representation</span></span>

<span data-ttu-id="05482-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05482-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "String",
  "description": "String",
  "name": "String",
  "type": "String"
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
