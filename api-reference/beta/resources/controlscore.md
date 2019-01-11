---
title: " controlScore 资源类型"
description: 此资源包含的租户分数和单个控件的说明。
localization_priority: Normal
ms.openlocfilehash: d8c2d73205f00a9dd5f2f28fcee3c33778bb3276
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891467"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="ba7a0-103">controlScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba7a0-103">controlScore resource type</span></span>

<span data-ttu-id="ba7a0-104">此资源包含的租户分数和单个控件的说明。</span><span class="sxs-lookup"><span data-stu-id="ba7a0-104">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="ba7a0-105">名称</span><span class="sxs-lookup"><span data-stu-id="ba7a0-105">Name</span></span> |<span data-ttu-id="ba7a0-106">类型</span><span class="sxs-lookup"><span data-stu-id="ba7a0-106">Type</span></span> |<span data-ttu-id="ba7a0-107">Description</span><span class="sxs-lookup"><span data-stu-id="ba7a0-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="ba7a0-108">控件名称</span><span class="sxs-lookup"><span data-stu-id="ba7a0-108">controlName</span></span> |   <span data-ttu-id="ba7a0-109">字符串</span><span class="sxs-lookup"><span data-stu-id="ba7a0-109">String</span></span>  |   <span data-ttu-id="ba7a0-110">控件的唯一名称</span><span class="sxs-lookup"><span data-stu-id="ba7a0-110">Control unique name</span></span> |
|   <span data-ttu-id="ba7a0-111">分数</span><span class="sxs-lookup"><span data-stu-id="ba7a0-111">score</span></span>   |   <span data-ttu-id="ba7a0-112">Double</span><span class="sxs-lookup"><span data-stu-id="ba7a0-112">Double</span></span>  |  <span data-ttu-id="ba7a0-113">租户实现 （它而异逐日控件上的租户操作） 的控件的分数。</span><span class="sxs-lookup"><span data-stu-id="ba7a0-113">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="ba7a0-114">controlCategory</span><span class="sxs-lookup"><span data-stu-id="ba7a0-114">controlCategory</span></span> |   <span data-ttu-id="ba7a0-115">字符串</span><span class="sxs-lookup"><span data-stu-id="ba7a0-115">String</span></span>  |  <span data-ttu-id="ba7a0-116">控制操作类别 （Identity、 数据、 设备、 应用程序、 基础结构）。</span><span class="sxs-lookup"><span data-stu-id="ba7a0-116">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="ba7a0-117">说明</span><span class="sxs-lookup"><span data-stu-id="ba7a0-117">description</span></span> |   <span data-ttu-id="ba7a0-118">字符串</span><span class="sxs-lookup"><span data-stu-id="ba7a0-118">String</span></span>  |  <span data-ttu-id="ba7a0-119">控件的说明。</span><span class="sxs-lookup"><span data-stu-id="ba7a0-119">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ba7a0-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba7a0-120">JSON representation</span></span>

<span data-ttu-id="ba7a0-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba7a0-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.controlScore"
}-->

```json
{
  "controlName": "String",
  "score": "String",
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
