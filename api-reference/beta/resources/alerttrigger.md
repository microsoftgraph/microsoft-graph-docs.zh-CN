---
title: alertTrigger 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: e375538806f09f85539f7a03e31c8a1ae041afdc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866645"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="c248a-104">alertTrigger 资源类型</span><span class="sxs-lookup"><span data-stu-id="c248a-104">alertTrigger resource type</span></span>

 > <span data-ttu-id="c248a-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c248a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c248a-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c248a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c248a-107">包含有关触发检测属性的信息 （警报实体中存在属性）。</span><span class="sxs-lookup"><span data-stu-id="c248a-107">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="c248a-108">属性</span><span class="sxs-lookup"><span data-stu-id="c248a-108">Properties</span></span>

| <span data-ttu-id="c248a-109">属性</span><span class="sxs-lookup"><span data-stu-id="c248a-109">Property</span></span>   | <span data-ttu-id="c248a-110">类型</span><span class="sxs-lookup"><span data-stu-id="c248a-110">Type</span></span>|<span data-ttu-id="c248a-111">说明</span><span class="sxs-lookup"><span data-stu-id="c248a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c248a-112">name</span><span class="sxs-lookup"><span data-stu-id="c248a-112">name</span></span>|<span data-ttu-id="c248a-113">字符串</span><span class="sxs-lookup"><span data-stu-id="c248a-113">String</span></span>|<span data-ttu-id="c248a-114">充当检测触发器属性的名称。</span><span class="sxs-lookup"><span data-stu-id="c248a-114">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="c248a-115">type</span><span class="sxs-lookup"><span data-stu-id="c248a-115">type</span></span>|<span data-ttu-id="c248a-116">字符串</span><span class="sxs-lookup"><span data-stu-id="c248a-116">String</span></span>|<span data-ttu-id="c248a-117">用于解释： 键值对中属性的类型。</span><span class="sxs-lookup"><span data-stu-id="c248a-117">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="c248a-118">例如，String、 Boolean、 等。</span><span class="sxs-lookup"><span data-stu-id="c248a-118">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="c248a-119">值</span><span class="sxs-lookup"><span data-stu-id="c248a-119">value</span></span>|<span data-ttu-id="c248a-120">字符串</span><span class="sxs-lookup"><span data-stu-id="c248a-120">String</span></span>|<span data-ttu-id="c248a-121">充当检测触发器属性的值。</span><span class="sxs-lookup"><span data-stu-id="c248a-121">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c248a-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c248a-122">JSON representation</span></span>

<span data-ttu-id="c248a-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c248a-123">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="c248a-124">示例</span><span class="sxs-lookup"><span data-stu-id="c248a-124">Example</span></span>

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
