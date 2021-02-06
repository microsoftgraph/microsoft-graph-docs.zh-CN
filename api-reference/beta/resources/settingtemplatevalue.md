---
title: settingTemplateValue 资源类型
description: 表示单个模板设置定义，包括设置的默认值（如果未实例化该设置）。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: dkershaw10
ms.openlocfilehash: 15110b88b62352476619501c50457a5bd1db5a89
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131626"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="f0e79-103">settingTemplateValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0e79-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="f0e79-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0e79-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0e79-105">表示单个模板设置定义，包括设置的默认值（如果未实例化该设置）。</span><span class="sxs-lookup"><span data-stu-id="f0e79-105">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="f0e79-106">属性</span><span class="sxs-lookup"><span data-stu-id="f0e79-106">Properties</span></span>
| <span data-ttu-id="f0e79-107">属性</span><span class="sxs-lookup"><span data-stu-id="f0e79-107">Property</span></span>     | <span data-ttu-id="f0e79-108">类型</span><span class="sxs-lookup"><span data-stu-id="f0e79-108">Type</span></span>   |<span data-ttu-id="f0e79-109">说明</span><span class="sxs-lookup"><span data-stu-id="f0e79-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0e79-110">defaultValue</span><span class="sxs-lookup"><span data-stu-id="f0e79-110">defaultValue</span></span>|<span data-ttu-id="f0e79-111">string</span><span class="sxs-lookup"><span data-stu-id="f0e79-111">string</span></span>|<span data-ttu-id="f0e79-112">设置的默认值。</span><span class="sxs-lookup"><span data-stu-id="f0e79-112">Default value for the setting.</span></span> <span data-ttu-id="f0e79-113">只读。</span><span class="sxs-lookup"><span data-stu-id="f0e79-113">Read-only.</span></span>|
|<span data-ttu-id="f0e79-114">说明</span><span class="sxs-lookup"><span data-stu-id="f0e79-114">description</span></span>|<span data-ttu-id="f0e79-115">string</span><span class="sxs-lookup"><span data-stu-id="f0e79-115">string</span></span>|<span data-ttu-id="f0e79-116">设置的说明。</span><span class="sxs-lookup"><span data-stu-id="f0e79-116">Description of the setting.</span></span> <span data-ttu-id="f0e79-117">只读。</span><span class="sxs-lookup"><span data-stu-id="f0e79-117">Read-only.</span></span>|
|<span data-ttu-id="f0e79-118">name</span><span class="sxs-lookup"><span data-stu-id="f0e79-118">name</span></span>|<span data-ttu-id="f0e79-119">string</span><span class="sxs-lookup"><span data-stu-id="f0e79-119">string</span></span>|<span data-ttu-id="f0e79-120">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="f0e79-120">Name of the setting.</span></span> <span data-ttu-id="f0e79-121">只读。</span><span class="sxs-lookup"><span data-stu-id="f0e79-121">Read-only.</span></span>|
|<span data-ttu-id="f0e79-122">类型</span><span class="sxs-lookup"><span data-stu-id="f0e79-122">type</span></span>|<span data-ttu-id="f0e79-123">string</span><span class="sxs-lookup"><span data-stu-id="f0e79-123">string</span></span>|<span data-ttu-id="f0e79-124">设置的类型。</span><span class="sxs-lookup"><span data-stu-id="f0e79-124">Type of the setting.</span></span> <span data-ttu-id="f0e79-125">只读。</span><span class="sxs-lookup"><span data-stu-id="f0e79-125">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0e79-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0e79-126">JSON representation</span></span>

<span data-ttu-id="f0e79-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0e79-127">Here is a JSON representation of the resource.</span></span>

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


