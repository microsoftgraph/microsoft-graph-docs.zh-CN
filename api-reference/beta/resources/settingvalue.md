---
title: settingValue 资源类型
description: 由名称/值对表示的设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d8e652501f8cd96e3e820e61b4ad9d353b61f3fd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008472"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="29b84-103">settingValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="29b84-103">settingValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29b84-104">由名称/值对表示的设置。</span><span class="sxs-lookup"><span data-stu-id="29b84-104">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="29b84-105">属性</span><span class="sxs-lookup"><span data-stu-id="29b84-105">Properties</span></span>
| <span data-ttu-id="29b84-106">属性</span><span class="sxs-lookup"><span data-stu-id="29b84-106">Property</span></span>     | <span data-ttu-id="29b84-107">类型</span><span class="sxs-lookup"><span data-stu-id="29b84-107">Type</span></span>   |<span data-ttu-id="29b84-108">说明</span><span class="sxs-lookup"><span data-stu-id="29b84-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29b84-109">name</span><span class="sxs-lookup"><span data-stu-id="29b84-109">name</span></span>|<span data-ttu-id="29b84-110">string</span><span class="sxs-lookup"><span data-stu-id="29b84-110">string</span></span>|<span data-ttu-id="29b84-111">设置的名称 (由 directorySettingTemplate 定义)。</span><span class="sxs-lookup"><span data-stu-id="29b84-111">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="29b84-112">value</span><span class="sxs-lookup"><span data-stu-id="29b84-112">value</span></span>|<span data-ttu-id="29b84-113">string</span><span class="sxs-lookup"><span data-stu-id="29b84-113">string</span></span>|<span data-ttu-id="29b84-114">设置的值。</span><span class="sxs-lookup"><span data-stu-id="29b84-114">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29b84-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29b84-115">JSON representation</span></span>

<span data-ttu-id="29b84-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29b84-116">Here is a JSON representation of the resource.</span></span>

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
