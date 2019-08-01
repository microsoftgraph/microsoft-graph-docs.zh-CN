---
title: settingValue 资源类型
description: 由名称/值对表示的设置。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f37a429fd9bb8e8d3cf65aef55d6af5033f4a598
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034354"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="14cde-103">settingValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="14cde-103">settingValue resource type</span></span>

<span data-ttu-id="14cde-104">由名称/值对表示的设置。</span><span class="sxs-lookup"><span data-stu-id="14cde-104">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="14cde-105">属性</span><span class="sxs-lookup"><span data-stu-id="14cde-105">Properties</span></span>

| <span data-ttu-id="14cde-106">属性</span><span class="sxs-lookup"><span data-stu-id="14cde-106">Property</span></span> | <span data-ttu-id="14cde-107">类型</span><span class="sxs-lookup"><span data-stu-id="14cde-107">Type</span></span> | <span data-ttu-id="14cde-108">说明</span><span class="sxs-lookup"><span data-stu-id="14cde-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="14cde-109">name</span><span class="sxs-lookup"><span data-stu-id="14cde-109">name</span></span>|<span data-ttu-id="14cde-110">String</span><span class="sxs-lookup"><span data-stu-id="14cde-110">String</span></span>| <span data-ttu-id="14cde-111">设置的名称 (由[groupSettingTemplate](groupsettingtemplate.md)定义)。</span><span class="sxs-lookup"><span data-stu-id="14cde-111">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="14cde-112">value</span><span class="sxs-lookup"><span data-stu-id="14cde-112">value</span></span>|<span data-ttu-id="14cde-113">String</span><span class="sxs-lookup"><span data-stu-id="14cde-113">String</span></span>| <span data-ttu-id="14cde-114">设置的值。</span><span class="sxs-lookup"><span data-stu-id="14cde-114">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="14cde-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14cde-115">JSON representation</span></span>

<span data-ttu-id="14cde-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14cde-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
