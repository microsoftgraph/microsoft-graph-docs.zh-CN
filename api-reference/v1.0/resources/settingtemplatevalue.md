---
title: settingTemplateValue 资源类型
description: 表示单个模板设置定义，包括设置的默认值（如果未实例化设置）。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: eea9f77b26ee0ce88e2c97c87e7cca50cbf48491
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533744"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="2589c-103">settingTemplateValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="2589c-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="2589c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2589c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2589c-105">表示单个模板设置定义，包括设置的默认值（如果未实例化设置）。</span><span class="sxs-lookup"><span data-stu-id="2589c-105">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="2589c-106">属性</span><span class="sxs-lookup"><span data-stu-id="2589c-106">Properties</span></span>

| <span data-ttu-id="2589c-107">属性</span><span class="sxs-lookup"><span data-stu-id="2589c-107">Property</span></span> | <span data-ttu-id="2589c-108">类型</span><span class="sxs-lookup"><span data-stu-id="2589c-108">Type</span></span> | <span data-ttu-id="2589c-109">说明</span><span class="sxs-lookup"><span data-stu-id="2589c-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2589c-110">默认</span><span class="sxs-lookup"><span data-stu-id="2589c-110">defaultValue</span></span>|<span data-ttu-id="2589c-111">字符串</span><span class="sxs-lookup"><span data-stu-id="2589c-111">String</span></span>| <span data-ttu-id="2589c-112">设置的默认值。</span><span class="sxs-lookup"><span data-stu-id="2589c-112">Default value for the setting.</span></span> |
|<span data-ttu-id="2589c-113">说明</span><span class="sxs-lookup"><span data-stu-id="2589c-113">description</span></span>|<span data-ttu-id="2589c-114">字符串</span><span class="sxs-lookup"><span data-stu-id="2589c-114">String</span></span>| <span data-ttu-id="2589c-115">设置的说明。</span><span class="sxs-lookup"><span data-stu-id="2589c-115">Description of the setting.</span></span> |
|<span data-ttu-id="2589c-116">name</span><span class="sxs-lookup"><span data-stu-id="2589c-116">name</span></span>|<span data-ttu-id="2589c-117">String</span><span class="sxs-lookup"><span data-stu-id="2589c-117">String</span></span>| <span data-ttu-id="2589c-118">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="2589c-118">Name of the setting.</span></span> |
|<span data-ttu-id="2589c-119">type</span><span class="sxs-lookup"><span data-stu-id="2589c-119">type</span></span>|<span data-ttu-id="2589c-120">字符串</span><span class="sxs-lookup"><span data-stu-id="2589c-120">String</span></span>| <span data-ttu-id="2589c-121">设置的类型。</span><span class="sxs-lookup"><span data-stu-id="2589c-121">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="2589c-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2589c-122">JSON representation</span></span>

<span data-ttu-id="2589c-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2589c-123">Here is a JSON representation of the resource.</span></span>

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
