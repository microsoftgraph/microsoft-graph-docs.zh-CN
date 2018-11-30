---
title: alertTrigger 资源类型
description: 包含有关触发检测属性的信息 （警报实体中存在属性）。
ms.openlocfilehash: b4af3be67669fd27f27e888cbc28b60b0c1c67a5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010957"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="44521-103">alertTrigger 资源类型</span><span class="sxs-lookup"><span data-stu-id="44521-103">alertTrigger resource type</span></span>

<span data-ttu-id="44521-104">包含有关触发检测属性的信息 （警报实体中存在属性）。</span><span class="sxs-lookup"><span data-stu-id="44521-104">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="44521-105">属性</span><span class="sxs-lookup"><span data-stu-id="44521-105">Properties</span></span>

| <span data-ttu-id="44521-106">属性</span><span class="sxs-lookup"><span data-stu-id="44521-106">Property</span></span>   | <span data-ttu-id="44521-107">类型</span><span class="sxs-lookup"><span data-stu-id="44521-107">Type</span></span>|<span data-ttu-id="44521-108">说明</span><span class="sxs-lookup"><span data-stu-id="44521-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44521-109">name</span><span class="sxs-lookup"><span data-stu-id="44521-109">name</span></span>|<span data-ttu-id="44521-110">字符串</span><span class="sxs-lookup"><span data-stu-id="44521-110">String</span></span>|<span data-ttu-id="44521-111">充当检测触发器属性的名称。</span><span class="sxs-lookup"><span data-stu-id="44521-111">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="44521-112">type</span><span class="sxs-lookup"><span data-stu-id="44521-112">type</span></span>|<span data-ttu-id="44521-113">字符串</span><span class="sxs-lookup"><span data-stu-id="44521-113">String</span></span>|<span data-ttu-id="44521-114">用于解释： 键值对中属性的类型。</span><span class="sxs-lookup"><span data-stu-id="44521-114">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="44521-115">例如，String、 Boolean、 等。</span><span class="sxs-lookup"><span data-stu-id="44521-115">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="44521-116">值</span><span class="sxs-lookup"><span data-stu-id="44521-116">value</span></span>|<span data-ttu-id="44521-117">字符串</span><span class="sxs-lookup"><span data-stu-id="44521-117">String</span></span>|<span data-ttu-id="44521-118">充当检测触发器属性的值。</span><span class="sxs-lookup"><span data-stu-id="44521-118">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44521-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44521-119">JSON representation</span></span>

<span data-ttu-id="44521-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44521-120">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="44521-121">示例</span><span class="sxs-lookup"><span data-stu-id="44521-121">Example</span></span>

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