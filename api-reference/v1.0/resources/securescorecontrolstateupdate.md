---
title: secureScoreControlStateUpdate 资源类型
description: 此资源包含用户更新的控件状态的历史记录 (控件状态包括默认、忽略、ThirdParty、已审阅)。
localization_priority: Normal
author: preetikr
ms.openlocfilehash: ac66fb2085949e375c79b18bfdfd39e84392159d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629248"
---
#  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="a08e7-103">secureScoreControlStateUpdate 资源类型</span><span class="sxs-lookup"><span data-stu-id="a08e7-103">secureScoreControlStateUpdate resource type</span></span>

<span data-ttu-id="a08e7-104">包含用户更新的控件状态的历史记录 (控件状态包括默认、忽略、ThirdParty、已审阅)。</span><span class="sxs-lookup"><span data-stu-id="a08e7-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

## <a name="properties"></a><span data-ttu-id="a08e7-105">属性</span><span class="sxs-lookup"><span data-stu-id="a08e7-105">Properties</span></span>

|<span data-ttu-id="a08e7-106">属性</span><span class="sxs-lookup"><span data-stu-id="a08e7-106">Property</span></span> |<span data-ttu-id="a08e7-107">类型</span><span class="sxs-lookup"><span data-stu-id="a08e7-107">Type</span></span> |<span data-ttu-id="a08e7-108">说明</span><span class="sxs-lookup"><span data-stu-id="a08e7-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="a08e7-109">assignedTo</span><span class="sxs-lookup"><span data-stu-id="a08e7-109">assignedTo</span></span>|<span data-ttu-id="a08e7-110">String</span><span class="sxs-lookup"><span data-stu-id="a08e7-110">String</span></span>|<span data-ttu-id="a08e7-111">将控件分配给将执行该操作的用户。</span><span class="sxs-lookup"><span data-stu-id="a08e7-111">Assigns the control to the user who will take the action.</span></span> |
|<span data-ttu-id="a08e7-112">注释</span><span class="sxs-lookup"><span data-stu-id="a08e7-112">comment</span></span>|<span data-ttu-id="a08e7-113">字符串</span><span class="sxs-lookup"><span data-stu-id="a08e7-113">String</span></span>|<span data-ttu-id="a08e7-114">提供有关控件的可选注释。</span><span class="sxs-lookup"><span data-stu-id="a08e7-114">Provides optional comment about the control.</span></span> |
|<span data-ttu-id="a08e7-115">state</span><span class="sxs-lookup"><span data-stu-id="a08e7-115">state</span></span>|<span data-ttu-id="a08e7-116">String</span><span class="sxs-lookup"><span data-stu-id="a08e7-116">String</span></span>|<span data-ttu-id="a08e7-117">控件的状态, 可通过修补程序命令进行修改 (例如, 忽略、thirdParty)。</span><span class="sxs-lookup"><span data-stu-id="a08e7-117">State of the control, which can be modified via a PATCH command (for example, ignored, thirdParty).</span></span> |
|<span data-ttu-id="a08e7-118">updatedBy</span><span class="sxs-lookup"><span data-stu-id="a08e7-118">updatedBy</span></span>|<span data-ttu-id="a08e7-119">字符串</span><span class="sxs-lookup"><span data-stu-id="a08e7-119">String</span></span>|<span data-ttu-id="a08e7-120">更新了租户状态的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="a08e7-120">ID of the user who updated tenant state.</span></span> |
|<span data-ttu-id="a08e7-121">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="a08e7-121">updatedDateTime</span></span>|<span data-ttu-id="a08e7-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a08e7-122">DateTimeOffset</span></span>|<span data-ttu-id="a08e7-123">控件状态的更新时间。</span><span class="sxs-lookup"><span data-stu-id="a08e7-123">Time at which the control state was updated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a08e7-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a08e7-124">JSON representation</span></span>
 <span data-ttu-id="a08e7-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a08e7-125">The following is a JSON representation of the resource.</span></span>
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
