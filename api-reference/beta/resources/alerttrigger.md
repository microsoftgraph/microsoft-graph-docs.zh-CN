---
title: alertTrigger 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 9142c4d86b627f1d1e1e790c9b3b279b07005ad2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339154"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="7de6d-104">alertTrigger 资源类型</span><span class="sxs-lookup"><span data-stu-id="7de6d-104">alertTrigger resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7de6d-105">包含有关触发检测的属性 (警报实体中存在属性) 的信息。</span><span class="sxs-lookup"><span data-stu-id="7de6d-105">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="7de6d-106">属性</span><span class="sxs-lookup"><span data-stu-id="7de6d-106">Properties</span></span>

| <span data-ttu-id="7de6d-107">属性</span><span class="sxs-lookup"><span data-stu-id="7de6d-107">Property</span></span>   | <span data-ttu-id="7de6d-108">类型</span><span class="sxs-lookup"><span data-stu-id="7de6d-108">Type</span></span>|<span data-ttu-id="7de6d-109">说明</span><span class="sxs-lookup"><span data-stu-id="7de6d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7de6d-110">name</span><span class="sxs-lookup"><span data-stu-id="7de6d-110">name</span></span>|<span data-ttu-id="7de6d-111">字符串</span><span class="sxs-lookup"><span data-stu-id="7de6d-111">String</span></span>|<span data-ttu-id="7de6d-112">充当检测触发器的属性的名称。</span><span class="sxs-lookup"><span data-stu-id="7de6d-112">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="7de6d-113">type</span><span class="sxs-lookup"><span data-stu-id="7de6d-113">type</span></span>|<span data-ttu-id="7de6d-114">String</span><span class="sxs-lookup"><span data-stu-id="7de6d-114">String</span></span>|<span data-ttu-id="7de6d-115">用于解释的键: 值对中的属性的类型。</span><span class="sxs-lookup"><span data-stu-id="7de6d-115">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="7de6d-116">例如, String、Boolean 等。</span><span class="sxs-lookup"><span data-stu-id="7de6d-116">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="7de6d-117">value</span><span class="sxs-lookup"><span data-stu-id="7de6d-117">value</span></span>|<span data-ttu-id="7de6d-118">String</span><span class="sxs-lookup"><span data-stu-id="7de6d-118">String</span></span>|<span data-ttu-id="7de6d-119">充当检测触发器的属性的值。</span><span class="sxs-lookup"><span data-stu-id="7de6d-119">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7de6d-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7de6d-120">JSON representation</span></span>

<span data-ttu-id="7de6d-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7de6d-121">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="7de6d-122">示例</span><span class="sxs-lookup"><span data-stu-id="7de6d-122">Example</span></span>

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
