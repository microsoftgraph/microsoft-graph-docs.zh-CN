---
title: settingValue 资源类型
description: 由名称/值对表示的设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: dkershaw10
ms.openlocfilehash: d1be40f6ad2046895c1a14f3395185662ae0ff62
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133376"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="392c3-103">settingValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="392c3-103">settingValue resource type</span></span>

<span data-ttu-id="392c3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="392c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="392c3-105">由名称/值对表示的设置。</span><span class="sxs-lookup"><span data-stu-id="392c3-105">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="392c3-106">属性</span><span class="sxs-lookup"><span data-stu-id="392c3-106">Properties</span></span>
| <span data-ttu-id="392c3-107">属性</span><span class="sxs-lookup"><span data-stu-id="392c3-107">Property</span></span>     | <span data-ttu-id="392c3-108">类型</span><span class="sxs-lookup"><span data-stu-id="392c3-108">Type</span></span>   |<span data-ttu-id="392c3-109">说明</span><span class="sxs-lookup"><span data-stu-id="392c3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="392c3-110">name</span><span class="sxs-lookup"><span data-stu-id="392c3-110">name</span></span>|<span data-ttu-id="392c3-111">string</span><span class="sxs-lookup"><span data-stu-id="392c3-111">string</span></span>|<span data-ttu-id="392c3-112">由 directorySettingTemplate (定义的设置) 。</span><span class="sxs-lookup"><span data-stu-id="392c3-112">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="392c3-113">value</span><span class="sxs-lookup"><span data-stu-id="392c3-113">value</span></span>|<span data-ttu-id="392c3-114">string</span><span class="sxs-lookup"><span data-stu-id="392c3-114">string</span></span>|<span data-ttu-id="392c3-115">设置的值。</span><span class="sxs-lookup"><span data-stu-id="392c3-115">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="392c3-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="392c3-116">JSON representation</span></span>

<span data-ttu-id="392c3-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="392c3-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


