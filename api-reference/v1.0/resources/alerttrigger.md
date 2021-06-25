---
title: alertTrigger 资源类型
description: 包含有关触发检测的属性的信息， (警报实体中的属性) 。
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 6bdee4ee550b44694a572e3611652b19c7ff574c
ms.sourcegitcommit: 8a9be6f65f62f29973508d82e0348d4142c18f23
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2021
ms.locfileid: "53129437"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="bcbb3-103">alertTrigger 资源类型</span><span class="sxs-lookup"><span data-stu-id="bcbb3-103">alertTrigger resource type</span></span>

<span data-ttu-id="bcbb3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcbb3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bcbb3-105">包含有关触发检测的属性的信息， (警报实体中的属性) 。</span><span class="sxs-lookup"><span data-stu-id="bcbb3-105">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="bcbb3-106">属性</span><span class="sxs-lookup"><span data-stu-id="bcbb3-106">Properties</span></span>

| <span data-ttu-id="bcbb3-107">属性</span><span class="sxs-lookup"><span data-stu-id="bcbb3-107">Property</span></span>   | <span data-ttu-id="bcbb3-108">类型</span><span class="sxs-lookup"><span data-stu-id="bcbb3-108">Type</span></span>|<span data-ttu-id="bcbb3-109">说明</span><span class="sxs-lookup"><span data-stu-id="bcbb3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bcbb3-110">name</span><span class="sxs-lookup"><span data-stu-id="bcbb3-110">name</span></span>|<span data-ttu-id="bcbb3-111">String</span><span class="sxs-lookup"><span data-stu-id="bcbb3-111">String</span></span>|<span data-ttu-id="bcbb3-112">充当检测触发器的属性的名称。</span><span class="sxs-lookup"><span data-stu-id="bcbb3-112">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="bcbb3-113">type</span><span class="sxs-lookup"><span data-stu-id="bcbb3-113">type</span></span>|<span data-ttu-id="bcbb3-114">String</span><span class="sxs-lookup"><span data-stu-id="bcbb3-114">String</span></span>|<span data-ttu-id="bcbb3-115">用于解释的 key：value 对中的属性类型。</span><span class="sxs-lookup"><span data-stu-id="bcbb3-115">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="bcbb3-116">例如，String、Boolean 等。</span><span class="sxs-lookup"><span data-stu-id="bcbb3-116">For example, String, Boolean etc.</span></span>|
|<span data-ttu-id="bcbb3-117">value</span><span class="sxs-lookup"><span data-stu-id="bcbb3-117">value</span></span>|<span data-ttu-id="bcbb3-118">String</span><span class="sxs-lookup"><span data-stu-id="bcbb3-118">String</span></span>|<span data-ttu-id="bcbb3-119">用作检测触发器的属性的值。</span><span class="sxs-lookup"><span data-stu-id="bcbb3-119">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bcbb3-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bcbb3-120">JSON representation</span></span>

<span data-ttu-id="bcbb3-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bcbb3-121">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="bcbb3-122">示例</span><span class="sxs-lookup"><span data-stu-id="bcbb3-122">Example</span></span>

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

