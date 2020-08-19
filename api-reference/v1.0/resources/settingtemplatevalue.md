---
title: settingTemplateValue 资源类型
description: 表示单个模板设置定义，包括设置的默认值（如果未实例化设置）。
localization_priority: Normal
author: dkershaw10
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a2046017dec6439c6db35169de15eb6bb49413b1
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806735"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="5526d-103">settingTemplateValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="5526d-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="5526d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5526d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5526d-105">表示单个模板设置定义，包括设置的默认值（如果未实例化设置）。</span><span class="sxs-lookup"><span data-stu-id="5526d-105">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="5526d-106">属性</span><span class="sxs-lookup"><span data-stu-id="5526d-106">Properties</span></span>

| <span data-ttu-id="5526d-107">属性</span><span class="sxs-lookup"><span data-stu-id="5526d-107">Property</span></span> | <span data-ttu-id="5526d-108">类型</span><span class="sxs-lookup"><span data-stu-id="5526d-108">Type</span></span> | <span data-ttu-id="5526d-109">说明</span><span class="sxs-lookup"><span data-stu-id="5526d-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5526d-110">默认</span><span class="sxs-lookup"><span data-stu-id="5526d-110">defaultValue</span></span>|<span data-ttu-id="5526d-111">String</span><span class="sxs-lookup"><span data-stu-id="5526d-111">String</span></span>| <span data-ttu-id="5526d-112">设置的默认值。</span><span class="sxs-lookup"><span data-stu-id="5526d-112">Default value for the setting.</span></span> |
|<span data-ttu-id="5526d-113">description</span><span class="sxs-lookup"><span data-stu-id="5526d-113">description</span></span>|<span data-ttu-id="5526d-114">String</span><span class="sxs-lookup"><span data-stu-id="5526d-114">String</span></span>| <span data-ttu-id="5526d-115">设置的说明。</span><span class="sxs-lookup"><span data-stu-id="5526d-115">Description of the setting.</span></span> |
|<span data-ttu-id="5526d-116">name</span><span class="sxs-lookup"><span data-stu-id="5526d-116">name</span></span>|<span data-ttu-id="5526d-117">String</span><span class="sxs-lookup"><span data-stu-id="5526d-117">String</span></span>| <span data-ttu-id="5526d-118">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="5526d-118">Name of the setting.</span></span> |
|<span data-ttu-id="5526d-119">type</span><span class="sxs-lookup"><span data-stu-id="5526d-119">type</span></span>|<span data-ttu-id="5526d-120">String</span><span class="sxs-lookup"><span data-stu-id="5526d-120">String</span></span>| <span data-ttu-id="5526d-121">设置的类型。</span><span class="sxs-lookup"><span data-stu-id="5526d-121">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="5526d-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5526d-122">JSON representation</span></span>

<span data-ttu-id="5526d-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5526d-123">Here is a JSON representation of the resource.</span></span>

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
