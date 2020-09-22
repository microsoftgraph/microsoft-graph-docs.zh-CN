---
title: " secureScoreControlStateUpdate 资源类型"
description: 此资源包含由用户更新的控制状态的历史记录 (控制状态包括默认、已忽略、ThirdParty、已审阅) 。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: d1678d4fe77ade738f7eb298221772ced381e2d1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087549"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="e7bbe-103">secureScoreControlStateUpdate 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7bbe-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="e7bbe-104">包含用户更新的控件状态的历史记录 (控件状态包括默认值、被忽略的 ThirdParty、已审阅的) 。</span><span class="sxs-lookup"><span data-stu-id="e7bbe-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="e7bbe-105">属性</span><span class="sxs-lookup"><span data-stu-id="e7bbe-105">Property</span></span> |<span data-ttu-id="e7bbe-106">类型</span><span class="sxs-lookup"><span data-stu-id="e7bbe-106">Type</span></span> |<span data-ttu-id="e7bbe-107">说明</span><span class="sxs-lookup"><span data-stu-id="e7bbe-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="e7bbe-108">assignedTo</span><span class="sxs-lookup"><span data-stu-id="e7bbe-108">assignedTo</span></span> | <span data-ttu-id="e7bbe-109">string</span><span class="sxs-lookup"><span data-stu-id="e7bbe-109">string</span></span> | <span data-ttu-id="e7bbe-110">将控件分配给将执行该操作的用户</span><span class="sxs-lookup"><span data-stu-id="e7bbe-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="e7bbe-111">comment</span><span class="sxs-lookup"><span data-stu-id="e7bbe-111">comment</span></span> | <span data-ttu-id="e7bbe-112">string</span><span class="sxs-lookup"><span data-stu-id="e7bbe-112">string</span></span> | <span data-ttu-id="e7bbe-113">提供有关控件的可选注释</span><span class="sxs-lookup"><span data-stu-id="e7bbe-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="e7bbe-114">state</span><span class="sxs-lookup"><span data-stu-id="e7bbe-114">state</span></span> | <span data-ttu-id="e7bbe-115">string</span><span class="sxs-lookup"><span data-stu-id="e7bbe-115">string</span></span> | <span data-ttu-id="e7bbe-116">可以使用 PATCH 命令修改控件的状态 (Ex：忽略、thirdParty 等) </span><span class="sxs-lookup"><span data-stu-id="e7bbe-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="e7bbe-117">updatedBy</span><span class="sxs-lookup"><span data-stu-id="e7bbe-117">updatedBy</span></span> | <span data-ttu-id="e7bbe-118">string</span><span class="sxs-lookup"><span data-stu-id="e7bbe-118">string</span></span> |<span data-ttu-id="e7bbe-119">更新了租户状态的用户的 ID</span><span class="sxs-lookup"><span data-stu-id="e7bbe-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="e7bbe-120">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7bbe-120">updatedDateTime</span></span> | <span data-ttu-id="e7bbe-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7bbe-121">DateTimeOffset</span></span> |<span data-ttu-id="e7bbe-122">更新控件状态的时间</span><span class="sxs-lookup"><span data-stu-id="e7bbe-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="e7bbe-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7bbe-123">JSON representation</span></span>
 <span data-ttu-id="e7bbe-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7bbe-124">The following is a JSON representation of the resource.</span></span>
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


