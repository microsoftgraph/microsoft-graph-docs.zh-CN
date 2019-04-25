---
title: " secureScoreControlStateUpdate 资源类型"
description: 此资源包含用户更新的控制状态的历史记录 (控件状态包括默认、忽略、ThirdParty、已审阅)。
localization_priority: Normal
ms.openlocfilehash: 8d8c3122a6263ebc7b10b5edfb823953e2d587fc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549137"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="9a5ef-103">secureScoreControlStateUpdate 资源类型</span><span class="sxs-lookup"><span data-stu-id="9a5ef-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="9a5ef-104">包含用户更新的控件状态的历史记录 (控件状态包括默认、忽略、ThirdParty、已审阅)。</span><span class="sxs-lookup"><span data-stu-id="9a5ef-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="9a5ef-105">属性</span><span class="sxs-lookup"><span data-stu-id="9a5ef-105">Property</span></span> |<span data-ttu-id="9a5ef-106">类型</span><span class="sxs-lookup"><span data-stu-id="9a5ef-106">Type</span></span> |<span data-ttu-id="9a5ef-107">说明</span><span class="sxs-lookup"><span data-stu-id="9a5ef-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="9a5ef-108">assignedTo</span><span class="sxs-lookup"><span data-stu-id="9a5ef-108">assignedTo</span></span> | <span data-ttu-id="9a5ef-109">string</span><span class="sxs-lookup"><span data-stu-id="9a5ef-109">string</span></span> | <span data-ttu-id="9a5ef-110">将控件分配给将执行该操作的用户</span><span class="sxs-lookup"><span data-stu-id="9a5ef-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="9a5ef-111">comment</span><span class="sxs-lookup"><span data-stu-id="9a5ef-111">comment</span></span> | <span data-ttu-id="9a5ef-112">string</span><span class="sxs-lookup"><span data-stu-id="9a5ef-112">string</span></span> | <span data-ttu-id="9a5ef-113">提供有关控件的可选注释</span><span class="sxs-lookup"><span data-stu-id="9a5ef-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="9a5ef-114">state</span><span class="sxs-lookup"><span data-stu-id="9a5ef-114">state</span></span> | <span data-ttu-id="9a5ef-115">string</span><span class="sxs-lookup"><span data-stu-id="9a5ef-115">string</span></span> | <span data-ttu-id="9a5ef-116">可以使用 "修补程序" 命令修改控件的状态 (Ex: 忽略、thirdParty 等)</span><span class="sxs-lookup"><span data-stu-id="9a5ef-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="9a5ef-117">updatedBy</span><span class="sxs-lookup"><span data-stu-id="9a5ef-117">updatedBy</span></span> | <span data-ttu-id="9a5ef-118">string</span><span class="sxs-lookup"><span data-stu-id="9a5ef-118">string</span></span> |<span data-ttu-id="9a5ef-119">更新了租户状态的用户的 ID</span><span class="sxs-lookup"><span data-stu-id="9a5ef-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="9a5ef-120">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a5ef-120">updatedDateTime</span></span> | <span data-ttu-id="9a5ef-121">DateTimeOffset?</span><span class="sxs-lookup"><span data-stu-id="9a5ef-121">DateTimeOffset?</span></span> |<span data-ttu-id="9a5ef-122">更新控件状态的时间</span><span class="sxs-lookup"><span data-stu-id="9a5ef-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="9a5ef-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a5ef-123">JSON representation</span></span>
 <span data-ttu-id="9a5ef-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a5ef-124">The following is a JSON representation of the resource.</span></span>
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
