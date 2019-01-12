---
title: alertTrigger 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 56034fb566f960ec858b86cdb4bcac86e5b9b47a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946425"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="b77ef-104">alertTrigger 资源类型</span><span class="sxs-lookup"><span data-stu-id="b77ef-104">alertTrigger resource type</span></span>

 > <span data-ttu-id="b77ef-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b77ef-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b77ef-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b77ef-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b77ef-107">包含有关触发检测属性的信息 （警报实体中存在属性）。</span><span class="sxs-lookup"><span data-stu-id="b77ef-107">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="b77ef-108">属性</span><span class="sxs-lookup"><span data-stu-id="b77ef-108">Properties</span></span>

| <span data-ttu-id="b77ef-109">属性</span><span class="sxs-lookup"><span data-stu-id="b77ef-109">Property</span></span>   | <span data-ttu-id="b77ef-110">类型</span><span class="sxs-lookup"><span data-stu-id="b77ef-110">Type</span></span>|<span data-ttu-id="b77ef-111">说明</span><span class="sxs-lookup"><span data-stu-id="b77ef-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b77ef-112">name</span><span class="sxs-lookup"><span data-stu-id="b77ef-112">name</span></span>|<span data-ttu-id="b77ef-113">字符串</span><span class="sxs-lookup"><span data-stu-id="b77ef-113">String</span></span>|<span data-ttu-id="b77ef-114">充当检测触发器属性的名称。</span><span class="sxs-lookup"><span data-stu-id="b77ef-114">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="b77ef-115">type</span><span class="sxs-lookup"><span data-stu-id="b77ef-115">type</span></span>|<span data-ttu-id="b77ef-116">字符串</span><span class="sxs-lookup"><span data-stu-id="b77ef-116">String</span></span>|<span data-ttu-id="b77ef-117">用于解释： 键值对中属性的类型。</span><span class="sxs-lookup"><span data-stu-id="b77ef-117">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="b77ef-118">例如，String、 Boolean、 等。</span><span class="sxs-lookup"><span data-stu-id="b77ef-118">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="b77ef-119">值</span><span class="sxs-lookup"><span data-stu-id="b77ef-119">value</span></span>|<span data-ttu-id="b77ef-120">字符串</span><span class="sxs-lookup"><span data-stu-id="b77ef-120">String</span></span>|<span data-ttu-id="b77ef-121">充当检测触发器属性的值。</span><span class="sxs-lookup"><span data-stu-id="b77ef-121">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b77ef-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b77ef-122">JSON representation</span></span>

<span data-ttu-id="b77ef-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b77ef-123">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="b77ef-124">示例</span><span class="sxs-lookup"><span data-stu-id="b77ef-124">Example</span></span>

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
