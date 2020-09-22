---
title: " controlScore 资源类型"
description: 此资源包含单个控件的租户分数和说明。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 964de9f9567c419b4e14d38e79cdff92867fb5ea
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016805"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="fc29e-103">controlScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="fc29e-103">controlScore resource type</span></span>

<span data-ttu-id="fc29e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc29e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fc29e-105">此资源包含单个控件的租户分数和说明。</span><span class="sxs-lookup"><span data-stu-id="fc29e-105">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="fc29e-106">名称</span><span class="sxs-lookup"><span data-stu-id="fc29e-106">Name</span></span> |<span data-ttu-id="fc29e-107">类型</span><span class="sxs-lookup"><span data-stu-id="fc29e-107">Type</span></span> |<span data-ttu-id="fc29e-108">说明</span><span class="sxs-lookup"><span data-stu-id="fc29e-108">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="fc29e-109">controlName</span><span class="sxs-lookup"><span data-stu-id="fc29e-109">controlName</span></span> |   <span data-ttu-id="fc29e-110">String</span><span class="sxs-lookup"><span data-stu-id="fc29e-110">String</span></span>  |   <span data-ttu-id="fc29e-111">控件唯一名称</span><span class="sxs-lookup"><span data-stu-id="fc29e-111">Control unique name</span></span> |
|   <span data-ttu-id="fc29e-112">分</span><span class="sxs-lookup"><span data-stu-id="fc29e-112">score</span></span>   |   <span data-ttu-id="fc29e-113">双精度</span><span class="sxs-lookup"><span data-stu-id="fc29e-113">Double</span></span>  |  <span data-ttu-id="fc29e-114">租户实现的控制分数 (根据控件) 上的租户操作，每日变化。</span><span class="sxs-lookup"><span data-stu-id="fc29e-114">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="fc29e-115">controlCategory</span><span class="sxs-lookup"><span data-stu-id="fc29e-115">controlCategory</span></span> |   <span data-ttu-id="fc29e-116">String</span><span class="sxs-lookup"><span data-stu-id="fc29e-116">String</span></span>  |  <span data-ttu-id="fc29e-117">控制操作类别 (标识、数据、设备、应用程序、基础结构) 。</span><span class="sxs-lookup"><span data-stu-id="fc29e-117">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="fc29e-118">description</span><span class="sxs-lookup"><span data-stu-id="fc29e-118">description</span></span> |   <span data-ttu-id="fc29e-119">String</span><span class="sxs-lookup"><span data-stu-id="fc29e-119">String</span></span>  |  <span data-ttu-id="fc29e-120">控件的说明。</span><span class="sxs-lookup"><span data-stu-id="fc29e-120">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fc29e-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fc29e-121">JSON representation</span></span>

<span data-ttu-id="fc29e-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc29e-122">The following is a JSON representation of the resource.</span></span>

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


