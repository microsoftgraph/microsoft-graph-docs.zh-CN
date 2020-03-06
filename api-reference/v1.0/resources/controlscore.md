---
title: controlScore 资源类型
description: 此资源包含单个控件的租户分数和说明。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fc3de6363784f62792d7c4e56906c79ed1be0c69
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531766"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="4edd7-103">controlScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="4edd7-103">controlScore resource type</span></span>

<span data-ttu-id="4edd7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4edd7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4edd7-105">包含单个控件的租户分数和说明。</span><span class="sxs-lookup"><span data-stu-id="4edd7-105">Contains a tenant score and description for an individual control.</span></span>

## <a name="properties"></a><span data-ttu-id="4edd7-106">属性</span><span class="sxs-lookup"><span data-stu-id="4edd7-106">Properties</span></span>

|<span data-ttu-id="4edd7-107">名称</span><span class="sxs-lookup"><span data-stu-id="4edd7-107">Name</span></span> |<span data-ttu-id="4edd7-108">类型</span><span class="sxs-lookup"><span data-stu-id="4edd7-108">Type</span></span> |<span data-ttu-id="4edd7-109">说明</span><span class="sxs-lookup"><span data-stu-id="4edd7-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="4edd7-110">controlName</span><span class="sxs-lookup"><span data-stu-id="4edd7-110">controlName</span></span>|<span data-ttu-id="4edd7-111">字符串</span><span class="sxs-lookup"><span data-stu-id="4edd7-111">String</span></span>|<span data-ttu-id="4edd7-112">控制唯一名称。</span><span class="sxs-lookup"><span data-stu-id="4edd7-112">Control unique name.</span></span>|
|<span data-ttu-id="4edd7-113">score</span><span class="sxs-lookup"><span data-stu-id="4edd7-113">score</span></span>|<span data-ttu-id="4edd7-114">双精度</span><span class="sxs-lookup"><span data-stu-id="4edd7-114">Double</span></span>|<span data-ttu-id="4edd7-115">租户实现的控制得分（根据控件上的租户操作，每天变化）。</span><span class="sxs-lookup"><span data-stu-id="4edd7-115">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span>|
|<span data-ttu-id="4edd7-116">controlCategory</span><span class="sxs-lookup"><span data-stu-id="4edd7-116">controlCategory</span></span>|<span data-ttu-id="4edd7-117">字符串</span><span class="sxs-lookup"><span data-stu-id="4edd7-117">String</span></span>|<span data-ttu-id="4edd7-118">控制措施类别（标识、数据、设备、应用程序、基础结构）。</span><span class="sxs-lookup"><span data-stu-id="4edd7-118">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="4edd7-119">说明</span><span class="sxs-lookup"><span data-stu-id="4edd7-119">description</span></span>|<span data-ttu-id="4edd7-120">字符串</span><span class="sxs-lookup"><span data-stu-id="4edd7-120">String</span></span>| <span data-ttu-id="4edd7-121">控件的说明。</span><span class="sxs-lookup"><span data-stu-id="4edd7-121">Description of the control.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4edd7-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4edd7-122">JSON representation</span></span>

<span data-ttu-id="4edd7-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4edd7-123">The following is a JSON representation of the resource.</span></span>

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
