---
title: secureScoreControlStateUpdate 资源类型
description: 此资源包含用户更新的控件状态的历史记录 (控件状态包括默认、忽略、ThirdParty、已审阅)。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9e051f2c4319a2b2ae1e3dbd9ba633785a345c4a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034473"
---
#  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="0dd59-103">secureScoreControlStateUpdate 资源类型</span><span class="sxs-lookup"><span data-stu-id="0dd59-103">secureScoreControlStateUpdate resource type</span></span>

<span data-ttu-id="0dd59-104">包含用户更新的控件状态的历史记录 (控件状态包括默认、忽略、ThirdParty、已审阅)。</span><span class="sxs-lookup"><span data-stu-id="0dd59-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

## <a name="properties"></a><span data-ttu-id="0dd59-105">属性</span><span class="sxs-lookup"><span data-stu-id="0dd59-105">Properties</span></span>

|<span data-ttu-id="0dd59-106">属性</span><span class="sxs-lookup"><span data-stu-id="0dd59-106">Property</span></span> |<span data-ttu-id="0dd59-107">类型</span><span class="sxs-lookup"><span data-stu-id="0dd59-107">Type</span></span> |<span data-ttu-id="0dd59-108">说明</span><span class="sxs-lookup"><span data-stu-id="0dd59-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="0dd59-109">assignedTo</span><span class="sxs-lookup"><span data-stu-id="0dd59-109">assignedTo</span></span>|<span data-ttu-id="0dd59-110">String</span><span class="sxs-lookup"><span data-stu-id="0dd59-110">String</span></span>|<span data-ttu-id="0dd59-111">将控件分配给将执行该操作的用户。</span><span class="sxs-lookup"><span data-stu-id="0dd59-111">Assigns the control to the user who will take the action.</span></span> |
|<span data-ttu-id="0dd59-112">注释</span><span class="sxs-lookup"><span data-stu-id="0dd59-112">comment</span></span>|<span data-ttu-id="0dd59-113">String</span><span class="sxs-lookup"><span data-stu-id="0dd59-113">String</span></span>|<span data-ttu-id="0dd59-114">提供有关控件的可选注释。</span><span class="sxs-lookup"><span data-stu-id="0dd59-114">Provides optional comment about the control.</span></span> |
|<span data-ttu-id="0dd59-115">state</span><span class="sxs-lookup"><span data-stu-id="0dd59-115">state</span></span>|<span data-ttu-id="0dd59-116">String</span><span class="sxs-lookup"><span data-stu-id="0dd59-116">String</span></span>|<span data-ttu-id="0dd59-117">控件的状态, 可通过修补程序命令进行修改 (例如, 忽略、thirdParty)。</span><span class="sxs-lookup"><span data-stu-id="0dd59-117">State of the control, which can be modified via a PATCH command (for example, ignored, thirdParty).</span></span> |
|<span data-ttu-id="0dd59-118">updatedBy</span><span class="sxs-lookup"><span data-stu-id="0dd59-118">updatedBy</span></span>|<span data-ttu-id="0dd59-119">String</span><span class="sxs-lookup"><span data-stu-id="0dd59-119">String</span></span>|<span data-ttu-id="0dd59-120">更新了租户状态的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="0dd59-120">ID of the user who updated tenant state.</span></span> |
|<span data-ttu-id="0dd59-121">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="0dd59-121">updatedDateTime</span></span>|<span data-ttu-id="0dd59-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0dd59-122">DateTimeOffset</span></span>|<span data-ttu-id="0dd59-123">控件状态的更新时间。</span><span class="sxs-lookup"><span data-stu-id="0dd59-123">Time at which the control state was updated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0dd59-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0dd59-124">JSON representation</span></span>
 <span data-ttu-id="0dd59-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0dd59-125">The following is a JSON representation of the resource.</span></span>
 <!-- {
  "blockType": "resource",
  "optionalProperties": [
    
   ],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
 ```json
{
  "assignedTo": "String",
  "comment": "String",
  "state": "String",
  "updatedBy": "String",
  "updatedDateTime": "String (timestamp)"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
