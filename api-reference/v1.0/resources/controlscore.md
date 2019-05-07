---
title: controlScore 资源类型
description: 此资源包含单个控件的租户分数和说明。
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 64b5377fce01273ab31d7ec293f5dc7a6e1342ff
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629283"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="6b992-103">controlScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b992-103">controlScore resource type</span></span>

<span data-ttu-id="6b992-104">包含单个控件的租户分数和说明。</span><span class="sxs-lookup"><span data-stu-id="6b992-104">Contains a tenant score and description for an individual control.</span></span>

## <a name="properties"></a><span data-ttu-id="6b992-105">属性</span><span class="sxs-lookup"><span data-stu-id="6b992-105">Properties</span></span>

|<span data-ttu-id="6b992-106">名称</span><span class="sxs-lookup"><span data-stu-id="6b992-106">Name</span></span> |<span data-ttu-id="6b992-107">类型</span><span class="sxs-lookup"><span data-stu-id="6b992-107">Type</span></span> |<span data-ttu-id="6b992-108">说明</span><span class="sxs-lookup"><span data-stu-id="6b992-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="6b992-109">controlName</span><span class="sxs-lookup"><span data-stu-id="6b992-109">controlName</span></span>|<span data-ttu-id="6b992-110">字符串</span><span class="sxs-lookup"><span data-stu-id="6b992-110">String</span></span>|<span data-ttu-id="6b992-111">控制唯一名称。</span><span class="sxs-lookup"><span data-stu-id="6b992-111">Control unique name.</span></span>|
|<span data-ttu-id="6b992-112">score</span><span class="sxs-lookup"><span data-stu-id="6b992-112">score</span></span>|<span data-ttu-id="6b992-113">双精度</span><span class="sxs-lookup"><span data-stu-id="6b992-113">Double</span></span>|<span data-ttu-id="6b992-114">租户实现的控制得分 (根据控件上的租户操作, 每天变化)。</span><span class="sxs-lookup"><span data-stu-id="6b992-114">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span>|
|<span data-ttu-id="6b992-115">controlCategory</span><span class="sxs-lookup"><span data-stu-id="6b992-115">controlCategory</span></span>|<span data-ttu-id="6b992-116">字符串</span><span class="sxs-lookup"><span data-stu-id="6b992-116">String</span></span>|<span data-ttu-id="6b992-117">控制措施类别 (标识、数据、设备、应用程序、基础结构)。</span><span class="sxs-lookup"><span data-stu-id="6b992-117">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="6b992-118">说明</span><span class="sxs-lookup"><span data-stu-id="6b992-118">description</span></span>|<span data-ttu-id="6b992-119">字符串</span><span class="sxs-lookup"><span data-stu-id="6b992-119">String</span></span>| <span data-ttu-id="6b992-120">控件的说明。</span><span class="sxs-lookup"><span data-stu-id="6b992-120">Description of the control.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b992-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b992-121">JSON representation</span></span>

<span data-ttu-id="6b992-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b992-122">The following is a JSON representation of the resource.</span></span>

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
