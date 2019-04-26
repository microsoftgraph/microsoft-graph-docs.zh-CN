---
title: " controlScore 资源类型"
description: 此资源包含单个控件的租户分数和说明。
localization_priority: Normal
ms.openlocfilehash: 34e94128ff3993a01d37770bea1ad046f936405f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341181"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="443b6-103">controlScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="443b6-103">controlScore resource type</span></span>

<span data-ttu-id="443b6-104">此资源包含单个控件的租户分数和说明。</span><span class="sxs-lookup"><span data-stu-id="443b6-104">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="443b6-105">名称</span><span class="sxs-lookup"><span data-stu-id="443b6-105">Name</span></span> |<span data-ttu-id="443b6-106">类型</span><span class="sxs-lookup"><span data-stu-id="443b6-106">Type</span></span> |<span data-ttu-id="443b6-107">说明</span><span class="sxs-lookup"><span data-stu-id="443b6-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="443b6-108">controlName</span><span class="sxs-lookup"><span data-stu-id="443b6-108">controlName</span></span> |   <span data-ttu-id="443b6-109">String</span><span class="sxs-lookup"><span data-stu-id="443b6-109">String</span></span>  |   <span data-ttu-id="443b6-110">控件唯一名称</span><span class="sxs-lookup"><span data-stu-id="443b6-110">Control unique name</span></span> |
|   <span data-ttu-id="443b6-111">score</span><span class="sxs-lookup"><span data-stu-id="443b6-111">score</span></span>   |   <span data-ttu-id="443b6-112">双精度</span><span class="sxs-lookup"><span data-stu-id="443b6-112">Double</span></span>  |  <span data-ttu-id="443b6-113">租户实现的控制得分 (根据控件上的租户操作, 每天变化)。</span><span class="sxs-lookup"><span data-stu-id="443b6-113">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="443b6-114">controlCategory</span><span class="sxs-lookup"><span data-stu-id="443b6-114">controlCategory</span></span> |   <span data-ttu-id="443b6-115">String</span><span class="sxs-lookup"><span data-stu-id="443b6-115">String</span></span>  |  <span data-ttu-id="443b6-116">控制措施类别 (标识、数据、设备、应用程序、基础结构)。</span><span class="sxs-lookup"><span data-stu-id="443b6-116">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="443b6-117">说明</span><span class="sxs-lookup"><span data-stu-id="443b6-117">description</span></span> |   <span data-ttu-id="443b6-118">String</span><span class="sxs-lookup"><span data-stu-id="443b6-118">String</span></span>  |  <span data-ttu-id="443b6-119">控件的说明。</span><span class="sxs-lookup"><span data-stu-id="443b6-119">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="443b6-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="443b6-120">JSON representation</span></span>

<span data-ttu-id="443b6-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="443b6-121">The following is a JSON representation of the resource.</span></span>

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
