---
title: alertTrigger 资源类型
description: 包含有关触发检测属性的信息 （警报实体中存在属性）。
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 3a2f6818bad0c5600e4b2a2a2682707643d1900c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991256"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="85d11-103">alertTrigger 资源类型</span><span class="sxs-lookup"><span data-stu-id="85d11-103">alertTrigger resource type</span></span>

<span data-ttu-id="85d11-104">包含有关触发检测属性的信息 （警报实体中存在属性）。</span><span class="sxs-lookup"><span data-stu-id="85d11-104">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="85d11-105">属性</span><span class="sxs-lookup"><span data-stu-id="85d11-105">Properties</span></span>

| <span data-ttu-id="85d11-106">属性</span><span class="sxs-lookup"><span data-stu-id="85d11-106">Property</span></span>   | <span data-ttu-id="85d11-107">类型</span><span class="sxs-lookup"><span data-stu-id="85d11-107">Type</span></span>|<span data-ttu-id="85d11-108">说明</span><span class="sxs-lookup"><span data-stu-id="85d11-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85d11-109">name</span><span class="sxs-lookup"><span data-stu-id="85d11-109">name</span></span>|<span data-ttu-id="85d11-110">字符串</span><span class="sxs-lookup"><span data-stu-id="85d11-110">String</span></span>|<span data-ttu-id="85d11-111">充当检测触发器属性的名称。</span><span class="sxs-lookup"><span data-stu-id="85d11-111">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="85d11-112">type</span><span class="sxs-lookup"><span data-stu-id="85d11-112">type</span></span>|<span data-ttu-id="85d11-113">字符串</span><span class="sxs-lookup"><span data-stu-id="85d11-113">String</span></span>|<span data-ttu-id="85d11-114">用于解释： 键值对中属性的类型。</span><span class="sxs-lookup"><span data-stu-id="85d11-114">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="85d11-115">例如，String、 Boolean、 等。</span><span class="sxs-lookup"><span data-stu-id="85d11-115">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="85d11-116">值</span><span class="sxs-lookup"><span data-stu-id="85d11-116">value</span></span>|<span data-ttu-id="85d11-117">字符串</span><span class="sxs-lookup"><span data-stu-id="85d11-117">String</span></span>|<span data-ttu-id="85d11-118">充当检测触发器属性的值。</span><span class="sxs-lookup"><span data-stu-id="85d11-118">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="85d11-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85d11-119">JSON representation</span></span>

<span data-ttu-id="85d11-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85d11-120">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="85d11-121">示例</span><span class="sxs-lookup"><span data-stu-id="85d11-121">Example</span></span>

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
