---
title: " controlScore 资源类型"
description: 此资源包含单个控件的租户分数和说明。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 2b718851d1a27c3317a0ce77554be7ea3f8906a4
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811495"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="0346b-103">controlScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="0346b-103">controlScore resource type</span></span>

<span data-ttu-id="0346b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0346b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0346b-105">此资源包含单个控件的租户分数和说明。</span><span class="sxs-lookup"><span data-stu-id="0346b-105">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="0346b-106">名称</span><span class="sxs-lookup"><span data-stu-id="0346b-106">Name</span></span> |<span data-ttu-id="0346b-107">类型</span><span class="sxs-lookup"><span data-stu-id="0346b-107">Type</span></span> |<span data-ttu-id="0346b-108">说明</span><span class="sxs-lookup"><span data-stu-id="0346b-108">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="0346b-109">controlName</span><span class="sxs-lookup"><span data-stu-id="0346b-109">controlName</span></span> |   <span data-ttu-id="0346b-110">String</span><span class="sxs-lookup"><span data-stu-id="0346b-110">String</span></span>  |   <span data-ttu-id="0346b-111">控件唯一名称</span><span class="sxs-lookup"><span data-stu-id="0346b-111">Control unique name</span></span> |
|   <span data-ttu-id="0346b-112">分</span><span class="sxs-lookup"><span data-stu-id="0346b-112">score</span></span>   |   <span data-ttu-id="0346b-113">双精度</span><span class="sxs-lookup"><span data-stu-id="0346b-113">Double</span></span>  |  <span data-ttu-id="0346b-114">租户实现的控制分数 (根据控件) 上的租户操作，每日变化。</span><span class="sxs-lookup"><span data-stu-id="0346b-114">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="0346b-115">controlCategory</span><span class="sxs-lookup"><span data-stu-id="0346b-115">controlCategory</span></span> |   <span data-ttu-id="0346b-116">String</span><span class="sxs-lookup"><span data-stu-id="0346b-116">String</span></span>  |  <span data-ttu-id="0346b-117">控制操作类别 (标识、数据、设备、应用程序、基础结构) 。</span><span class="sxs-lookup"><span data-stu-id="0346b-117">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="0346b-118">description</span><span class="sxs-lookup"><span data-stu-id="0346b-118">description</span></span> |   <span data-ttu-id="0346b-119">String</span><span class="sxs-lookup"><span data-stu-id="0346b-119">String</span></span>  |  <span data-ttu-id="0346b-120">控件的说明。</span><span class="sxs-lookup"><span data-stu-id="0346b-120">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0346b-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0346b-121">JSON representation</span></span>

<span data-ttu-id="0346b-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0346b-122">The following is a JSON representation of the resource.</span></span>

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
