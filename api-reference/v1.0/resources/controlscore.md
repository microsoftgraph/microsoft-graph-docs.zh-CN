---
title: controlScore 资源类型
description: 此资源包含单个控件的租户分数和说明。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9e4470d1ce22f5ffbf3c805adc5328398d57d9fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056922"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="6ab42-103">controlScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ab42-103">controlScore resource type</span></span>

<span data-ttu-id="6ab42-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ab42-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6ab42-105">包含单个控件的租户分数和说明。</span><span class="sxs-lookup"><span data-stu-id="6ab42-105">Contains a tenant score and description for an individual control.</span></span>

## <a name="properties"></a><span data-ttu-id="6ab42-106">属性</span><span class="sxs-lookup"><span data-stu-id="6ab42-106">Properties</span></span>

|<span data-ttu-id="6ab42-107">名称</span><span class="sxs-lookup"><span data-stu-id="6ab42-107">Name</span></span> |<span data-ttu-id="6ab42-108">类型</span><span class="sxs-lookup"><span data-stu-id="6ab42-108">Type</span></span> |<span data-ttu-id="6ab42-109">说明</span><span class="sxs-lookup"><span data-stu-id="6ab42-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="6ab42-110">controlName</span><span class="sxs-lookup"><span data-stu-id="6ab42-110">controlName</span></span>|<span data-ttu-id="6ab42-111">String</span><span class="sxs-lookup"><span data-stu-id="6ab42-111">String</span></span>|<span data-ttu-id="6ab42-112">控制唯一名称。</span><span class="sxs-lookup"><span data-stu-id="6ab42-112">Control unique name.</span></span>|
|<span data-ttu-id="6ab42-113">分</span><span class="sxs-lookup"><span data-stu-id="6ab42-113">score</span></span>|<span data-ttu-id="6ab42-114">双精度</span><span class="sxs-lookup"><span data-stu-id="6ab42-114">Double</span></span>|<span data-ttu-id="6ab42-115">租户实现的控制分数 (根据控件) 上的租户操作，每日变化。</span><span class="sxs-lookup"><span data-stu-id="6ab42-115">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span>|
|<span data-ttu-id="6ab42-116">controlCategory</span><span class="sxs-lookup"><span data-stu-id="6ab42-116">controlCategory</span></span>|<span data-ttu-id="6ab42-117">String</span><span class="sxs-lookup"><span data-stu-id="6ab42-117">String</span></span>|<span data-ttu-id="6ab42-118">控制操作类别 (标识、数据、设备、应用程序、基础结构) 。</span><span class="sxs-lookup"><span data-stu-id="6ab42-118">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="6ab42-119">description</span><span class="sxs-lookup"><span data-stu-id="6ab42-119">description</span></span>|<span data-ttu-id="6ab42-120">String</span><span class="sxs-lookup"><span data-stu-id="6ab42-120">String</span></span>| <span data-ttu-id="6ab42-121">控件的说明。</span><span class="sxs-lookup"><span data-stu-id="6ab42-121">Description of the control.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6ab42-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ab42-122">JSON representation</span></span>

<span data-ttu-id="6ab42-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ab42-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.controlScore"
}-->

```json
{
  "controlName": "String",
  "score": "Double",
  "controlCategory": "String",
  "description": "String"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "controlScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

