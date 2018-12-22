---
title: " secureScoreControlStateUpdate 资源类型"
description: 此资源包含控件状态更新的用户的历史记录 （控件状态包括默认、 忽略、 ThirdParty、 已审阅）。
ms.openlocfilehash: ba98f2fc85f3f8e12355f9acf5d232599a7f29f7
ms.sourcegitcommit: 8feddb85e436be5581557a199f2e46d5b4ebfa21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/22/2018
ms.locfileid: "27428838"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="3a6b4-103">secureScoreControlStateUpdate 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a6b4-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="3a6b4-104">包含由用户更新控件状态的历史记录 （控件状态包括默认、 忽略、 ThirdParty、 已审阅）。</span><span class="sxs-lookup"><span data-stu-id="3a6b4-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="3a6b4-105">属性</span><span class="sxs-lookup"><span data-stu-id="3a6b4-105">Property</span></span> |<span data-ttu-id="3a6b4-106">类型</span><span class="sxs-lookup"><span data-stu-id="3a6b4-106">Type</span></span> |<span data-ttu-id="3a6b4-107">说明</span><span class="sxs-lookup"><span data-stu-id="3a6b4-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="3a6b4-108">assignedTo</span><span class="sxs-lookup"><span data-stu-id="3a6b4-108">assignedTo</span></span> | <span data-ttu-id="3a6b4-109">string</span><span class="sxs-lookup"><span data-stu-id="3a6b4-109">string</span></span> | <span data-ttu-id="3a6b4-110">分配将执行的操作的用户控件</span><span class="sxs-lookup"><span data-stu-id="3a6b4-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="3a6b4-111">批注</span><span class="sxs-lookup"><span data-stu-id="3a6b4-111">comment</span></span> | <span data-ttu-id="3a6b4-112">string</span><span class="sxs-lookup"><span data-stu-id="3a6b4-112">string</span></span> | <span data-ttu-id="3a6b4-113">提供有关控件的可选注释</span><span class="sxs-lookup"><span data-stu-id="3a6b4-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="3a6b4-114">state</span><span class="sxs-lookup"><span data-stu-id="3a6b4-114">state</span></span> | <span data-ttu-id="3a6b4-115">string</span><span class="sxs-lookup"><span data-stu-id="3a6b4-115">string</span></span> | <span data-ttu-id="3a6b4-116">可以使用修补程序命令修改控件的状态 (例如： 忽略，第三方等)</span><span class="sxs-lookup"><span data-stu-id="3a6b4-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="3a6b4-117">updatedBy</span><span class="sxs-lookup"><span data-stu-id="3a6b4-117">updatedBy</span></span> | <span data-ttu-id="3a6b4-118">string</span><span class="sxs-lookup"><span data-stu-id="3a6b4-118">string</span></span> |<span data-ttu-id="3a6b4-119">更新租户状态的用户的 ID</span><span class="sxs-lookup"><span data-stu-id="3a6b4-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="3a6b4-120">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a6b4-120">updatedDateTime</span></span> | <span data-ttu-id="3a6b4-121">方法？</span><span class="sxs-lookup"><span data-stu-id="3a6b4-121">DateTimeOffset?</span></span> |<span data-ttu-id="3a6b4-122">在哪个控件更新状态的时间</span><span class="sxs-lookup"><span data-stu-id="3a6b4-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="3a6b4-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a6b4-123">JSON representation</span></span>
 <span data-ttu-id="3a6b4-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a6b4-124">The following is a JSON representation of the resource.</span></span>
 <!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
 ```json
{
  "assignedTo": "String",
  "comment": "Double",
  "state": "Double",
  "updatedBy": "Double",
  "updatedDateTime": "Double"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
