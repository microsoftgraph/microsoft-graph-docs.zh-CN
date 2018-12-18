---
title: alertTrigger 资源类型
description: 包含有关触发检测属性的信息 （警报实体中存在属性）。
author: Preetikr
ms.openlocfilehash: f0888e6caf78d806909f818a8b72fb21320e7796
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341264"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="be5c6-103">alertTrigger 资源类型</span><span class="sxs-lookup"><span data-stu-id="be5c6-103">alertTrigger resource type</span></span>

<span data-ttu-id="be5c6-104">包含有关触发检测属性的信息 （警报实体中存在属性）。</span><span class="sxs-lookup"><span data-stu-id="be5c6-104">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="be5c6-105">属性</span><span class="sxs-lookup"><span data-stu-id="be5c6-105">Properties</span></span>

| <span data-ttu-id="be5c6-106">属性</span><span class="sxs-lookup"><span data-stu-id="be5c6-106">Property</span></span>   | <span data-ttu-id="be5c6-107">类型</span><span class="sxs-lookup"><span data-stu-id="be5c6-107">Type</span></span>|<span data-ttu-id="be5c6-108">说明</span><span class="sxs-lookup"><span data-stu-id="be5c6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be5c6-109">name</span><span class="sxs-lookup"><span data-stu-id="be5c6-109">name</span></span>|<span data-ttu-id="be5c6-110">字符串</span><span class="sxs-lookup"><span data-stu-id="be5c6-110">String</span></span>|<span data-ttu-id="be5c6-111">充当检测触发器属性的名称。</span><span class="sxs-lookup"><span data-stu-id="be5c6-111">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="be5c6-112">type</span><span class="sxs-lookup"><span data-stu-id="be5c6-112">type</span></span>|<span data-ttu-id="be5c6-113">字符串</span><span class="sxs-lookup"><span data-stu-id="be5c6-113">String</span></span>|<span data-ttu-id="be5c6-114">用于解释： 键值对中属性的类型。</span><span class="sxs-lookup"><span data-stu-id="be5c6-114">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="be5c6-115">例如，String、 Boolean、 等。</span><span class="sxs-lookup"><span data-stu-id="be5c6-115">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="be5c6-116">值</span><span class="sxs-lookup"><span data-stu-id="be5c6-116">value</span></span>|<span data-ttu-id="be5c6-117">字符串</span><span class="sxs-lookup"><span data-stu-id="be5c6-117">String</span></span>|<span data-ttu-id="be5c6-118">充当检测触发器属性的值。</span><span class="sxs-lookup"><span data-stu-id="be5c6-118">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be5c6-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be5c6-119">JSON representation</span></span>

<span data-ttu-id="be5c6-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be5c6-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a><span data-ttu-id="be5c6-121">示例</span><span class="sxs-lookup"><span data-stu-id="be5c6-121">Example</span></span>

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->