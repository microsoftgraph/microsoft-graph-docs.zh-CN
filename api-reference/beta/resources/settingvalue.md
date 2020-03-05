---
title: settingValue 资源类型
description: 由名称/值对表示的设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 673627d726475708c79445f818f23104f0582ef7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520820"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="c15d4-103">settingValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="c15d4-103">settingValue resource type</span></span>

<span data-ttu-id="c15d4-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c15d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c15d4-105">由名称/值对表示的设置。</span><span class="sxs-lookup"><span data-stu-id="c15d4-105">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="c15d4-106">属性</span><span class="sxs-lookup"><span data-stu-id="c15d4-106">Properties</span></span>
| <span data-ttu-id="c15d4-107">属性</span><span class="sxs-lookup"><span data-stu-id="c15d4-107">Property</span></span>     | <span data-ttu-id="c15d4-108">类型</span><span class="sxs-lookup"><span data-stu-id="c15d4-108">Type</span></span>   |<span data-ttu-id="c15d4-109">说明</span><span class="sxs-lookup"><span data-stu-id="c15d4-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c15d4-110">name</span><span class="sxs-lookup"><span data-stu-id="c15d4-110">name</span></span>|<span data-ttu-id="c15d4-111">string</span><span class="sxs-lookup"><span data-stu-id="c15d4-111">string</span></span>|<span data-ttu-id="c15d4-112">设置的名称（由 directorySettingTemplate 定义）。</span><span class="sxs-lookup"><span data-stu-id="c15d4-112">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="c15d4-113">value</span><span class="sxs-lookup"><span data-stu-id="c15d4-113">value</span></span>|<span data-ttu-id="c15d4-114">string</span><span class="sxs-lookup"><span data-stu-id="c15d4-114">string</span></span>|<span data-ttu-id="c15d4-115">设置的值。</span><span class="sxs-lookup"><span data-stu-id="c15d4-115">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c15d4-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c15d4-116">JSON representation</span></span>

<span data-ttu-id="c15d4-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c15d4-117">Here is a JSON representation of the resource.</span></span>

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
