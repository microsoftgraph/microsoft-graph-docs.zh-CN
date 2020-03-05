---
title: alertTrigger 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 28bfd51a403077ee4ab456f6ca17fb176addf58d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508336"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="28dd6-104">alertTrigger 资源类型</span><span class="sxs-lookup"><span data-stu-id="28dd6-104">alertTrigger resource type</span></span>

<span data-ttu-id="28dd6-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="28dd6-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28dd6-106">包含有关触发检测的属性（警报实体中存在属性）的信息。</span><span class="sxs-lookup"><span data-stu-id="28dd6-106">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="28dd6-107">属性</span><span class="sxs-lookup"><span data-stu-id="28dd6-107">Properties</span></span>

| <span data-ttu-id="28dd6-108">属性</span><span class="sxs-lookup"><span data-stu-id="28dd6-108">Property</span></span>   | <span data-ttu-id="28dd6-109">类型</span><span class="sxs-lookup"><span data-stu-id="28dd6-109">Type</span></span>|<span data-ttu-id="28dd6-110">说明</span><span class="sxs-lookup"><span data-stu-id="28dd6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28dd6-111">name</span><span class="sxs-lookup"><span data-stu-id="28dd6-111">name</span></span>|<span data-ttu-id="28dd6-112">字符串</span><span class="sxs-lookup"><span data-stu-id="28dd6-112">String</span></span>|<span data-ttu-id="28dd6-113">充当检测触发器的属性的名称。</span><span class="sxs-lookup"><span data-stu-id="28dd6-113">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="28dd6-114">type</span><span class="sxs-lookup"><span data-stu-id="28dd6-114">type</span></span>|<span data-ttu-id="28dd6-115">String</span><span class="sxs-lookup"><span data-stu-id="28dd6-115">String</span></span>|<span data-ttu-id="28dd6-116">用于解释的键：值对中的属性的类型。</span><span class="sxs-lookup"><span data-stu-id="28dd6-116">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="28dd6-117">例如，String、Boolean 等。</span><span class="sxs-lookup"><span data-stu-id="28dd6-117">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="28dd6-118">value</span><span class="sxs-lookup"><span data-stu-id="28dd6-118">value</span></span>|<span data-ttu-id="28dd6-119">String</span><span class="sxs-lookup"><span data-stu-id="28dd6-119">String</span></span>|<span data-ttu-id="28dd6-120">充当检测触发器的属性的值。</span><span class="sxs-lookup"><span data-stu-id="28dd6-120">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="28dd6-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28dd6-121">JSON representation</span></span>

<span data-ttu-id="28dd6-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28dd6-122">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="28dd6-123">示例</span><span class="sxs-lookup"><span data-stu-id="28dd6-123">Example</span></span>

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
