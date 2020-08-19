---
title: settingTemplateValue 资源类型
description: 表示单个模板设置定义，包括设置的默认值（如果未实例化设置）。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: dkershaw10
ms.openlocfilehash: 024007ef05edbb4c3e2e9f8cc901d654734a39ab
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806266"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="e9c22-103">settingTemplateValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="e9c22-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="e9c22-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9c22-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9c22-105">表示单个模板设置定义，包括设置的默认值（如果未实例化设置）。</span><span class="sxs-lookup"><span data-stu-id="e9c22-105">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="e9c22-106">属性</span><span class="sxs-lookup"><span data-stu-id="e9c22-106">Properties</span></span>
| <span data-ttu-id="e9c22-107">属性</span><span class="sxs-lookup"><span data-stu-id="e9c22-107">Property</span></span>     | <span data-ttu-id="e9c22-108">类型</span><span class="sxs-lookup"><span data-stu-id="e9c22-108">Type</span></span>   |<span data-ttu-id="e9c22-109">说明</span><span class="sxs-lookup"><span data-stu-id="e9c22-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9c22-110">默认</span><span class="sxs-lookup"><span data-stu-id="e9c22-110">defaultValue</span></span>|<span data-ttu-id="e9c22-111">string</span><span class="sxs-lookup"><span data-stu-id="e9c22-111">string</span></span>|<span data-ttu-id="e9c22-112">设置的默认值。</span><span class="sxs-lookup"><span data-stu-id="e9c22-112">Default value for the setting.</span></span> <span data-ttu-id="e9c22-113">只读。</span><span class="sxs-lookup"><span data-stu-id="e9c22-113">Read-only.</span></span>|
|<span data-ttu-id="e9c22-114">说明</span><span class="sxs-lookup"><span data-stu-id="e9c22-114">description</span></span>|<span data-ttu-id="e9c22-115">string</span><span class="sxs-lookup"><span data-stu-id="e9c22-115">string</span></span>|<span data-ttu-id="e9c22-116">设置的说明。</span><span class="sxs-lookup"><span data-stu-id="e9c22-116">Description of the setting.</span></span> <span data-ttu-id="e9c22-117">只读。</span><span class="sxs-lookup"><span data-stu-id="e9c22-117">Read-only.</span></span>|
|<span data-ttu-id="e9c22-118">name</span><span class="sxs-lookup"><span data-stu-id="e9c22-118">name</span></span>|<span data-ttu-id="e9c22-119">string</span><span class="sxs-lookup"><span data-stu-id="e9c22-119">string</span></span>|<span data-ttu-id="e9c22-120">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="e9c22-120">Name of the setting.</span></span> <span data-ttu-id="e9c22-121">只读。</span><span class="sxs-lookup"><span data-stu-id="e9c22-121">Read-only.</span></span>|
|<span data-ttu-id="e9c22-122">类型</span><span class="sxs-lookup"><span data-stu-id="e9c22-122">type</span></span>|<span data-ttu-id="e9c22-123">string</span><span class="sxs-lookup"><span data-stu-id="e9c22-123">string</span></span>|<span data-ttu-id="e9c22-124">设置的类型。</span><span class="sxs-lookup"><span data-stu-id="e9c22-124">Type of the setting.</span></span> <span data-ttu-id="e9c22-125">只读。</span><span class="sxs-lookup"><span data-stu-id="e9c22-125">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9c22-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e9c22-126">JSON representation</span></span>

<span data-ttu-id="e9c22-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9c22-127">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
