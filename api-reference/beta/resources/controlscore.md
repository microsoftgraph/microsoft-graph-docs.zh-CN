---
title: " controlScore 资源类型"
description: 此资源包含的租户分数和单个控件的说明。
ms.openlocfilehash: 67059c1a7382416411709f02c609c90b20a673b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042806"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="cec52-103">controlScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="cec52-103">controlScore resource type</span></span>

<span data-ttu-id="cec52-104">此资源包含的租户分数和单个控件的说明。</span><span class="sxs-lookup"><span data-stu-id="cec52-104">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="cec52-105">名称</span><span class="sxs-lookup"><span data-stu-id="cec52-105">Name</span></span> |<span data-ttu-id="cec52-106">类型</span><span class="sxs-lookup"><span data-stu-id="cec52-106">Type</span></span> |<span data-ttu-id="cec52-107">说明</span><span class="sxs-lookup"><span data-stu-id="cec52-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="cec52-108">控件名称</span><span class="sxs-lookup"><span data-stu-id="cec52-108">controlName</span></span> |   <span data-ttu-id="cec52-109">字符串</span><span class="sxs-lookup"><span data-stu-id="cec52-109">String</span></span>  |   <span data-ttu-id="cec52-110">控件的唯一名称</span><span class="sxs-lookup"><span data-stu-id="cec52-110">Control unique name</span></span> |
|   <span data-ttu-id="cec52-111">分数</span><span class="sxs-lookup"><span data-stu-id="cec52-111">score</span></span>   |   <span data-ttu-id="cec52-112">双精度数</span><span class="sxs-lookup"><span data-stu-id="cec52-112">Double</span></span>  |  <span data-ttu-id="cec52-113">租户实现 （它而异逐日控件上的租户操作） 的控件的分数。</span><span class="sxs-lookup"><span data-stu-id="cec52-113">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="cec52-114">controlCategory</span><span class="sxs-lookup"><span data-stu-id="cec52-114">controlCategory</span></span> |   <span data-ttu-id="cec52-115">字符串</span><span class="sxs-lookup"><span data-stu-id="cec52-115">String</span></span>  |  <span data-ttu-id="cec52-116">控制操作类别 （Identity、 数据、 设备、 应用程序、 基础结构）。</span><span class="sxs-lookup"><span data-stu-id="cec52-116">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="cec52-117">说明</span><span class="sxs-lookup"><span data-stu-id="cec52-117">description</span></span> |   <span data-ttu-id="cec52-118">字符串</span><span class="sxs-lookup"><span data-stu-id="cec52-118">String</span></span>  |  <span data-ttu-id="cec52-119">控件的说明。</span><span class="sxs-lookup"><span data-stu-id="cec52-119">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cec52-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cec52-120">JSON representation</span></span>

<span data-ttu-id="cec52-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cec52-121">The following is a JSON representation of the resource.</span></span>

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
