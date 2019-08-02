---
title: alertTrigger 资源类型
description: 包含有关触发检测的属性 (警报实体中存在属性) 的信息。
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 49a262e1ab0aa046f7326b935b8437824dcf8c08
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030112"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="723b5-103">alertTrigger 资源类型</span><span class="sxs-lookup"><span data-stu-id="723b5-103">alertTrigger resource type</span></span>

<span data-ttu-id="723b5-104">包含有关触发检测的属性 (警报实体中存在属性) 的信息。</span><span class="sxs-lookup"><span data-stu-id="723b5-104">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="723b5-105">属性</span><span class="sxs-lookup"><span data-stu-id="723b5-105">Properties</span></span>

| <span data-ttu-id="723b5-106">属性</span><span class="sxs-lookup"><span data-stu-id="723b5-106">Property</span></span>   | <span data-ttu-id="723b5-107">类型</span><span class="sxs-lookup"><span data-stu-id="723b5-107">Type</span></span>|<span data-ttu-id="723b5-108">说明</span><span class="sxs-lookup"><span data-stu-id="723b5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="723b5-109">name</span><span class="sxs-lookup"><span data-stu-id="723b5-109">name</span></span>|<span data-ttu-id="723b5-110">字符串</span><span class="sxs-lookup"><span data-stu-id="723b5-110">String</span></span>|<span data-ttu-id="723b5-111">充当检测触发器的属性的名称。</span><span class="sxs-lookup"><span data-stu-id="723b5-111">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="723b5-112">type</span><span class="sxs-lookup"><span data-stu-id="723b5-112">type</span></span>|<span data-ttu-id="723b5-113">String</span><span class="sxs-lookup"><span data-stu-id="723b5-113">String</span></span>|<span data-ttu-id="723b5-114">用于解释的键: 值对中的属性的类型。</span><span class="sxs-lookup"><span data-stu-id="723b5-114">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="723b5-115">例如, String、Boolean 等。</span><span class="sxs-lookup"><span data-stu-id="723b5-115">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="723b5-116">value</span><span class="sxs-lookup"><span data-stu-id="723b5-116">value</span></span>|<span data-ttu-id="723b5-117">String</span><span class="sxs-lookup"><span data-stu-id="723b5-117">String</span></span>|<span data-ttu-id="723b5-118">充当检测触发器的属性的值。</span><span class="sxs-lookup"><span data-stu-id="723b5-118">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="723b5-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="723b5-119">JSON representation</span></span>

<span data-ttu-id="723b5-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="723b5-120">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="723b5-121">示例</span><span class="sxs-lookup"><span data-stu-id="723b5-121">Example</span></span>

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
