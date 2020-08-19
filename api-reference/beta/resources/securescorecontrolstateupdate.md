---
title: " secureScoreControlStateUpdate 资源类型"
description: 此资源包含由用户更新的控制状态的历史记录 (控制状态包括默认、已忽略、ThirdParty、已审阅) 。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f3b69838a6de68938efac12acdfbcd4fd977c684
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810403"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="dd77b-103">secureScoreControlStateUpdate 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd77b-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="dd77b-104">包含用户更新的控件状态的历史记录 (控件状态包括默认值、被忽略的 ThirdParty、已审阅的) 。</span><span class="sxs-lookup"><span data-stu-id="dd77b-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="dd77b-105">属性</span><span class="sxs-lookup"><span data-stu-id="dd77b-105">Property</span></span> |<span data-ttu-id="dd77b-106">类型</span><span class="sxs-lookup"><span data-stu-id="dd77b-106">Type</span></span> |<span data-ttu-id="dd77b-107">说明</span><span class="sxs-lookup"><span data-stu-id="dd77b-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="dd77b-108">assignedTo</span><span class="sxs-lookup"><span data-stu-id="dd77b-108">assignedTo</span></span> | <span data-ttu-id="dd77b-109">string</span><span class="sxs-lookup"><span data-stu-id="dd77b-109">string</span></span> | <span data-ttu-id="dd77b-110">将控件分配给将执行该操作的用户</span><span class="sxs-lookup"><span data-stu-id="dd77b-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="dd77b-111">comment</span><span class="sxs-lookup"><span data-stu-id="dd77b-111">comment</span></span> | <span data-ttu-id="dd77b-112">string</span><span class="sxs-lookup"><span data-stu-id="dd77b-112">string</span></span> | <span data-ttu-id="dd77b-113">提供有关控件的可选注释</span><span class="sxs-lookup"><span data-stu-id="dd77b-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="dd77b-114">state</span><span class="sxs-lookup"><span data-stu-id="dd77b-114">state</span></span> | <span data-ttu-id="dd77b-115">string</span><span class="sxs-lookup"><span data-stu-id="dd77b-115">string</span></span> | <span data-ttu-id="dd77b-116">可以使用 PATCH 命令修改控件的状态 (Ex：忽略、thirdParty 等) </span><span class="sxs-lookup"><span data-stu-id="dd77b-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="dd77b-117">updatedBy</span><span class="sxs-lookup"><span data-stu-id="dd77b-117">updatedBy</span></span> | <span data-ttu-id="dd77b-118">string</span><span class="sxs-lookup"><span data-stu-id="dd77b-118">string</span></span> |<span data-ttu-id="dd77b-119">更新了租户状态的用户的 ID</span><span class="sxs-lookup"><span data-stu-id="dd77b-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="dd77b-120">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd77b-120">updatedDateTime</span></span> | <span data-ttu-id="dd77b-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd77b-121">DateTimeOffset</span></span> |<span data-ttu-id="dd77b-122">更新控件状态的时间</span><span class="sxs-lookup"><span data-stu-id="dd77b-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="dd77b-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd77b-123">JSON representation</span></span>
 <span data-ttu-id="dd77b-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd77b-124">The following is a JSON representation of the resource.</span></span>
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
