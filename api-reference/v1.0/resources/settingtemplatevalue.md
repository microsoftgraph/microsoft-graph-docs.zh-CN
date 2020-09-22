---
title: settingTemplateValue 资源类型
description: 表示单个模板设置定义，包括设置的默认值（如果未实例化设置）。
localization_priority: Normal
author: dkershaw10
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c39762290577c6279a4ecb52bd832ac9c961dbdb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009196"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="a288a-103">settingTemplateValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="a288a-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="a288a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a288a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a288a-105">表示单个模板设置定义，包括设置的默认值（如果未实例化设置）。</span><span class="sxs-lookup"><span data-stu-id="a288a-105">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="a288a-106">属性</span><span class="sxs-lookup"><span data-stu-id="a288a-106">Properties</span></span>

| <span data-ttu-id="a288a-107">属性</span><span class="sxs-lookup"><span data-stu-id="a288a-107">Property</span></span> | <span data-ttu-id="a288a-108">类型</span><span class="sxs-lookup"><span data-stu-id="a288a-108">Type</span></span> | <span data-ttu-id="a288a-109">说明</span><span class="sxs-lookup"><span data-stu-id="a288a-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a288a-110">默认</span><span class="sxs-lookup"><span data-stu-id="a288a-110">defaultValue</span></span>|<span data-ttu-id="a288a-111">String</span><span class="sxs-lookup"><span data-stu-id="a288a-111">String</span></span>| <span data-ttu-id="a288a-112">设置的默认值。</span><span class="sxs-lookup"><span data-stu-id="a288a-112">Default value for the setting.</span></span> |
|<span data-ttu-id="a288a-113">description</span><span class="sxs-lookup"><span data-stu-id="a288a-113">description</span></span>|<span data-ttu-id="a288a-114">String</span><span class="sxs-lookup"><span data-stu-id="a288a-114">String</span></span>| <span data-ttu-id="a288a-115">设置的说明。</span><span class="sxs-lookup"><span data-stu-id="a288a-115">Description of the setting.</span></span> |
|<span data-ttu-id="a288a-116">name</span><span class="sxs-lookup"><span data-stu-id="a288a-116">name</span></span>|<span data-ttu-id="a288a-117">String</span><span class="sxs-lookup"><span data-stu-id="a288a-117">String</span></span>| <span data-ttu-id="a288a-118">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="a288a-118">Name of the setting.</span></span> |
|<span data-ttu-id="a288a-119">type</span><span class="sxs-lookup"><span data-stu-id="a288a-119">type</span></span>|<span data-ttu-id="a288a-120">String</span><span class="sxs-lookup"><span data-stu-id="a288a-120">String</span></span>| <span data-ttu-id="a288a-121">设置的类型。</span><span class="sxs-lookup"><span data-stu-id="a288a-121">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="a288a-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a288a-122">JSON representation</span></span>

<span data-ttu-id="a288a-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a288a-123">Here is a JSON representation of the resource.</span></span>

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

