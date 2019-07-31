---
title: settingTemplateValue 资源类型
description: 表示单个模板设置定义, 包括设置的默认值 (如果未实例化设置)。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9a49dd291bd9cc7baa31d90ba8e247ac984b1906
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965185"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="30e64-103">settingTemplateValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="30e64-103">settingTemplateValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30e64-104">表示单个模板设置定义, 包括设置的默认值 (如果未实例化设置)。</span><span class="sxs-lookup"><span data-stu-id="30e64-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="30e64-105">属性</span><span class="sxs-lookup"><span data-stu-id="30e64-105">Properties</span></span>
| <span data-ttu-id="30e64-106">属性</span><span class="sxs-lookup"><span data-stu-id="30e64-106">Property</span></span>     | <span data-ttu-id="30e64-107">类型</span><span class="sxs-lookup"><span data-stu-id="30e64-107">Type</span></span>   |<span data-ttu-id="30e64-108">说明</span><span class="sxs-lookup"><span data-stu-id="30e64-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30e64-109">默认</span><span class="sxs-lookup"><span data-stu-id="30e64-109">defaultValue</span></span>|<span data-ttu-id="30e64-110">string</span><span class="sxs-lookup"><span data-stu-id="30e64-110">string</span></span>|<span data-ttu-id="30e64-111">设置的默认值。</span><span class="sxs-lookup"><span data-stu-id="30e64-111">Default value for the setting.</span></span> <span data-ttu-id="30e64-112">只读。</span><span class="sxs-lookup"><span data-stu-id="30e64-112">Read-only.</span></span>|
|<span data-ttu-id="30e64-113">说明</span><span class="sxs-lookup"><span data-stu-id="30e64-113">description</span></span>|<span data-ttu-id="30e64-114">string</span><span class="sxs-lookup"><span data-stu-id="30e64-114">string</span></span>|<span data-ttu-id="30e64-115">设置的说明。</span><span class="sxs-lookup"><span data-stu-id="30e64-115">Description of the setting.</span></span> <span data-ttu-id="30e64-116">只读。</span><span class="sxs-lookup"><span data-stu-id="30e64-116">Read-only.</span></span>|
|<span data-ttu-id="30e64-117">name</span><span class="sxs-lookup"><span data-stu-id="30e64-117">name</span></span>|<span data-ttu-id="30e64-118">string</span><span class="sxs-lookup"><span data-stu-id="30e64-118">string</span></span>|<span data-ttu-id="30e64-119">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="30e64-119">Name of the setting.</span></span> <span data-ttu-id="30e64-120">只读。</span><span class="sxs-lookup"><span data-stu-id="30e64-120">Read-only.</span></span>|
|<span data-ttu-id="30e64-121">类型</span><span class="sxs-lookup"><span data-stu-id="30e64-121">type</span></span>|<span data-ttu-id="30e64-122">string</span><span class="sxs-lookup"><span data-stu-id="30e64-122">string</span></span>|<span data-ttu-id="30e64-123">设置的类型。</span><span class="sxs-lookup"><span data-stu-id="30e64-123">Type of the setting.</span></span> <span data-ttu-id="30e64-124">只读。</span><span class="sxs-lookup"><span data-stu-id="30e64-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="30e64-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30e64-125">JSON representation</span></span>

<span data-ttu-id="30e64-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30e64-126">Here is a JSON representation of the resource.</span></span>

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
