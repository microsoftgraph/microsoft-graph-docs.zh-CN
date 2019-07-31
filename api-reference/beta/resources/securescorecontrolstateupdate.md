---
title: " secureScoreControlStateUpdate 资源类型"
description: 此资源包含用户更新的控制状态的历史记录 (控件状态包括默认、忽略、ThirdParty、已审阅)。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 92616569a87a6ccf91c17ea7c845b8185bd33e8b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965227"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="d6647-103">secureScoreControlStateUpdate 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6647-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="d6647-104">包含用户更新的控件状态的历史记录 (控件状态包括默认、忽略、ThirdParty、已审阅)。</span><span class="sxs-lookup"><span data-stu-id="d6647-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="d6647-105">属性</span><span class="sxs-lookup"><span data-stu-id="d6647-105">Property</span></span> |<span data-ttu-id="d6647-106">类型</span><span class="sxs-lookup"><span data-stu-id="d6647-106">Type</span></span> |<span data-ttu-id="d6647-107">说明</span><span class="sxs-lookup"><span data-stu-id="d6647-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="d6647-108">assignedTo</span><span class="sxs-lookup"><span data-stu-id="d6647-108">assignedTo</span></span> | <span data-ttu-id="d6647-109">string</span><span class="sxs-lookup"><span data-stu-id="d6647-109">string</span></span> | <span data-ttu-id="d6647-110">将控件分配给将执行该操作的用户</span><span class="sxs-lookup"><span data-stu-id="d6647-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="d6647-111">comment</span><span class="sxs-lookup"><span data-stu-id="d6647-111">comment</span></span> | <span data-ttu-id="d6647-112">string</span><span class="sxs-lookup"><span data-stu-id="d6647-112">string</span></span> | <span data-ttu-id="d6647-113">提供有关控件的可选注释</span><span class="sxs-lookup"><span data-stu-id="d6647-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="d6647-114">state</span><span class="sxs-lookup"><span data-stu-id="d6647-114">state</span></span> | <span data-ttu-id="d6647-115">string</span><span class="sxs-lookup"><span data-stu-id="d6647-115">string</span></span> | <span data-ttu-id="d6647-116">可以使用 "修补程序" 命令修改控件的状态 (Ex: 忽略、thirdParty 等)</span><span class="sxs-lookup"><span data-stu-id="d6647-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="d6647-117">updatedBy</span><span class="sxs-lookup"><span data-stu-id="d6647-117">updatedBy</span></span> | <span data-ttu-id="d6647-118">string</span><span class="sxs-lookup"><span data-stu-id="d6647-118">string</span></span> |<span data-ttu-id="d6647-119">更新了租户状态的用户的 ID</span><span class="sxs-lookup"><span data-stu-id="d6647-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="d6647-120">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6647-120">updatedDateTime</span></span> | <span data-ttu-id="d6647-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6647-121">DateTimeOffset</span></span> |<span data-ttu-id="d6647-122">更新控件状态的时间</span><span class="sxs-lookup"><span data-stu-id="d6647-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="d6647-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6647-123">JSON representation</span></span>
 <span data-ttu-id="d6647-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6647-124">The following is a JSON representation of the resource.</span></span>
 <!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
 ```json
{
  "assignedTo": "String",
  "comment": "string",
  "state": "string",
  "updatedBy": "string",
  "updatedDateTime": "DateTimeOffset"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
