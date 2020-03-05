---
title: " controlScore 资源类型"
description: 此资源包含单个控件的租户分数和说明。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f718e197e690d3779870e5996161461fe8f60915
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507413"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="6cb2c-103">controlScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="6cb2c-103">controlScore resource type</span></span>

<span data-ttu-id="6cb2c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6cb2c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6cb2c-105">此资源包含单个控件的租户分数和说明。</span><span class="sxs-lookup"><span data-stu-id="6cb2c-105">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="6cb2c-106">名称</span><span class="sxs-lookup"><span data-stu-id="6cb2c-106">Name</span></span> |<span data-ttu-id="6cb2c-107">类型</span><span class="sxs-lookup"><span data-stu-id="6cb2c-107">Type</span></span> |<span data-ttu-id="6cb2c-108">说明</span><span class="sxs-lookup"><span data-stu-id="6cb2c-108">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="6cb2c-109">controlName</span><span class="sxs-lookup"><span data-stu-id="6cb2c-109">controlName</span></span> |   <span data-ttu-id="6cb2c-110">String</span><span class="sxs-lookup"><span data-stu-id="6cb2c-110">String</span></span>  |   <span data-ttu-id="6cb2c-111">控件唯一名称</span><span class="sxs-lookup"><span data-stu-id="6cb2c-111">Control unique name</span></span> |
|   <span data-ttu-id="6cb2c-112">score</span><span class="sxs-lookup"><span data-stu-id="6cb2c-112">score</span></span>   |   <span data-ttu-id="6cb2c-113">双精度</span><span class="sxs-lookup"><span data-stu-id="6cb2c-113">Double</span></span>  |  <span data-ttu-id="6cb2c-114">租户实现的控制得分（根据控件上的租户操作，每天变化）。</span><span class="sxs-lookup"><span data-stu-id="6cb2c-114">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="6cb2c-115">controlCategory</span><span class="sxs-lookup"><span data-stu-id="6cb2c-115">controlCategory</span></span> |   <span data-ttu-id="6cb2c-116">String</span><span class="sxs-lookup"><span data-stu-id="6cb2c-116">String</span></span>  |  <span data-ttu-id="6cb2c-117">控制措施类别（标识、数据、设备、应用程序、基础结构）。</span><span class="sxs-lookup"><span data-stu-id="6cb2c-117">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="6cb2c-118">说明</span><span class="sxs-lookup"><span data-stu-id="6cb2c-118">description</span></span> |   <span data-ttu-id="6cb2c-119">String</span><span class="sxs-lookup"><span data-stu-id="6cb2c-119">String</span></span>  |  <span data-ttu-id="6cb2c-120">控件的说明。</span><span class="sxs-lookup"><span data-stu-id="6cb2c-120">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6cb2c-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6cb2c-121">JSON representation</span></span>

<span data-ttu-id="6cb2c-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6cb2c-122">The following is a JSON representation of the resource.</span></span>

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
