---
title: settingTemplateValue 资源类型
description: 表示单个模板设置定义，包括设置的默认值（如果未实例化该设置）。
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e53a8f07f325b023deea32e01fe217feeb35f49d
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547048"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="89d50-103">settingTemplateValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="89d50-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="89d50-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89d50-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89d50-105">表示单个模板设置定义，包括设置的默认值（如果未实例化该设置）。</span><span class="sxs-lookup"><span data-stu-id="89d50-105">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="89d50-106">属性</span><span class="sxs-lookup"><span data-stu-id="89d50-106">Properties</span></span>

| <span data-ttu-id="89d50-107">属性</span><span class="sxs-lookup"><span data-stu-id="89d50-107">Property</span></span> | <span data-ttu-id="89d50-108">类型</span><span class="sxs-lookup"><span data-stu-id="89d50-108">Type</span></span> | <span data-ttu-id="89d50-109">描述</span><span class="sxs-lookup"><span data-stu-id="89d50-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="89d50-110">defaultValue</span><span class="sxs-lookup"><span data-stu-id="89d50-110">defaultValue</span></span>|<span data-ttu-id="89d50-111">字符串</span><span class="sxs-lookup"><span data-stu-id="89d50-111">String</span></span>| <span data-ttu-id="89d50-112">设置的默认值。</span><span class="sxs-lookup"><span data-stu-id="89d50-112">Default value for the setting.</span></span> |
|<span data-ttu-id="89d50-113">说明</span><span class="sxs-lookup"><span data-stu-id="89d50-113">description</span></span>|<span data-ttu-id="89d50-114">字符串</span><span class="sxs-lookup"><span data-stu-id="89d50-114">String</span></span>| <span data-ttu-id="89d50-115">设置的说明。</span><span class="sxs-lookup"><span data-stu-id="89d50-115">Description of the setting.</span></span> |
|<span data-ttu-id="89d50-116">name</span><span class="sxs-lookup"><span data-stu-id="89d50-116">name</span></span>|<span data-ttu-id="89d50-117">字符串</span><span class="sxs-lookup"><span data-stu-id="89d50-117">String</span></span>| <span data-ttu-id="89d50-118">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="89d50-118">Name of the setting.</span></span> |
|<span data-ttu-id="89d50-119">type</span><span class="sxs-lookup"><span data-stu-id="89d50-119">type</span></span>|<span data-ttu-id="89d50-120">字符串</span><span class="sxs-lookup"><span data-stu-id="89d50-120">String</span></span>| <span data-ttu-id="89d50-121">设置的类型。</span><span class="sxs-lookup"><span data-stu-id="89d50-121">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="89d50-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89d50-122">JSON representation</span></span>

<span data-ttu-id="89d50-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89d50-123">Here is a JSON representation of the resource.</span></span>

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

