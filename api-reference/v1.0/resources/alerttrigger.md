---
title: alertTrigger 资源类型
description: 包含有关触发检测的属性 (警报实体中存在属性) 的信息。
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 3a2f6818bad0c5600e4b2a2a2682707643d1900c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569464"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="c7d1a-103">alertTrigger 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7d1a-103">alertTrigger resource type</span></span>

<span data-ttu-id="c7d1a-104">包含有关触发检测的属性 (警报实体中存在属性) 的信息。</span><span class="sxs-lookup"><span data-stu-id="c7d1a-104">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="c7d1a-105">属性</span><span class="sxs-lookup"><span data-stu-id="c7d1a-105">Properties</span></span>

| <span data-ttu-id="c7d1a-106">属性</span><span class="sxs-lookup"><span data-stu-id="c7d1a-106">Property</span></span>   | <span data-ttu-id="c7d1a-107">类型</span><span class="sxs-lookup"><span data-stu-id="c7d1a-107">Type</span></span>|<span data-ttu-id="c7d1a-108">说明</span><span class="sxs-lookup"><span data-stu-id="c7d1a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7d1a-109">name</span><span class="sxs-lookup"><span data-stu-id="c7d1a-109">name</span></span>|<span data-ttu-id="c7d1a-110">字符串</span><span class="sxs-lookup"><span data-stu-id="c7d1a-110">String</span></span>|<span data-ttu-id="c7d1a-111">充当检测触发器的属性的名称。</span><span class="sxs-lookup"><span data-stu-id="c7d1a-111">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="c7d1a-112">type</span><span class="sxs-lookup"><span data-stu-id="c7d1a-112">type</span></span>|<span data-ttu-id="c7d1a-113">String</span><span class="sxs-lookup"><span data-stu-id="c7d1a-113">String</span></span>|<span data-ttu-id="c7d1a-114">用于解释的键: 值对中的属性的类型。</span><span class="sxs-lookup"><span data-stu-id="c7d1a-114">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="c7d1a-115">例如, String、Boolean 等。</span><span class="sxs-lookup"><span data-stu-id="c7d1a-115">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="c7d1a-116">value</span><span class="sxs-lookup"><span data-stu-id="c7d1a-116">value</span></span>|<span data-ttu-id="c7d1a-117">String</span><span class="sxs-lookup"><span data-stu-id="c7d1a-117">String</span></span>|<span data-ttu-id="c7d1a-118">充当检测触发器的属性的值。</span><span class="sxs-lookup"><span data-stu-id="c7d1a-118">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7d1a-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7d1a-119">JSON representation</span></span>

<span data-ttu-id="c7d1a-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7d1a-120">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="c7d1a-121">示例</span><span class="sxs-lookup"><span data-stu-id="c7d1a-121">Example</span></span>

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
