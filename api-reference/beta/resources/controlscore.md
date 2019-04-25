---
title: " controlScore 资源类型"
description: 此资源包含单个控件的租户分数和说明。
localization_priority: Normal
ms.openlocfilehash: d8c2d73205f00a9dd5f2f28fcee3c33778bb3276
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543376"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="30fa3-103">controlScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="30fa3-103">controlScore resource type</span></span>

<span data-ttu-id="30fa3-104">此资源包含单个控件的租户分数和说明。</span><span class="sxs-lookup"><span data-stu-id="30fa3-104">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="30fa3-105">名称</span><span class="sxs-lookup"><span data-stu-id="30fa3-105">Name</span></span> |<span data-ttu-id="30fa3-106">类型</span><span class="sxs-lookup"><span data-stu-id="30fa3-106">Type</span></span> |<span data-ttu-id="30fa3-107">说明</span><span class="sxs-lookup"><span data-stu-id="30fa3-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="30fa3-108">controlName</span><span class="sxs-lookup"><span data-stu-id="30fa3-108">controlName</span></span> |   <span data-ttu-id="30fa3-109">String</span><span class="sxs-lookup"><span data-stu-id="30fa3-109">String</span></span>  |   <span data-ttu-id="30fa3-110">控件唯一名称</span><span class="sxs-lookup"><span data-stu-id="30fa3-110">Control unique name</span></span> |
|   <span data-ttu-id="30fa3-111">score</span><span class="sxs-lookup"><span data-stu-id="30fa3-111">score</span></span>   |   <span data-ttu-id="30fa3-112">双精度</span><span class="sxs-lookup"><span data-stu-id="30fa3-112">Double</span></span>  |  <span data-ttu-id="30fa3-113">租户实现的控制得分 (根据控件上的租户操作, 每天变化)。</span><span class="sxs-lookup"><span data-stu-id="30fa3-113">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="30fa3-114">controlCategory</span><span class="sxs-lookup"><span data-stu-id="30fa3-114">controlCategory</span></span> |   <span data-ttu-id="30fa3-115">String</span><span class="sxs-lookup"><span data-stu-id="30fa3-115">String</span></span>  |  <span data-ttu-id="30fa3-116">控制措施类别 (标识、数据、设备、应用程序、基础结构)。</span><span class="sxs-lookup"><span data-stu-id="30fa3-116">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="30fa3-117">description</span><span class="sxs-lookup"><span data-stu-id="30fa3-117">description</span></span> |   <span data-ttu-id="30fa3-118">String</span><span class="sxs-lookup"><span data-stu-id="30fa3-118">String</span></span>  |  <span data-ttu-id="30fa3-119">控件的说明。</span><span class="sxs-lookup"><span data-stu-id="30fa3-119">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="30fa3-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30fa3-120">JSON representation</span></span>

<span data-ttu-id="30fa3-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30fa3-121">The following is a JSON representation of the resource.</span></span>

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
