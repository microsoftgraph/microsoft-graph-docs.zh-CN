---
title: secureScoreControlStateUpdate 资源类型
description: 此资源包含用户更新的控件状态的历史记录（控件状态包括默认、忽略、ThirdParty、已审阅）。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0fe88741da75718b1509fd4f8015a37fcf7828bf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446959"
---
#  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="d678a-103">secureScoreControlStateUpdate 资源类型</span><span class="sxs-lookup"><span data-stu-id="d678a-103">secureScoreControlStateUpdate resource type</span></span>

<span data-ttu-id="d678a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d678a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d678a-105">包含用户更新的控件状态的历史记录（控件状态包括默认、忽略、ThirdParty、已审阅）。</span><span class="sxs-lookup"><span data-stu-id="d678a-105">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

## <a name="properties"></a><span data-ttu-id="d678a-106">属性</span><span class="sxs-lookup"><span data-stu-id="d678a-106">Properties</span></span>

|<span data-ttu-id="d678a-107">属性</span><span class="sxs-lookup"><span data-stu-id="d678a-107">Property</span></span> |<span data-ttu-id="d678a-108">类型</span><span class="sxs-lookup"><span data-stu-id="d678a-108">Type</span></span> |<span data-ttu-id="d678a-109">说明</span><span class="sxs-lookup"><span data-stu-id="d678a-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="d678a-110">assignedTo</span><span class="sxs-lookup"><span data-stu-id="d678a-110">assignedTo</span></span>|<span data-ttu-id="d678a-111">String</span><span class="sxs-lookup"><span data-stu-id="d678a-111">String</span></span>|<span data-ttu-id="d678a-112">将控件分配给将执行该操作的用户。</span><span class="sxs-lookup"><span data-stu-id="d678a-112">Assigns the control to the user who will take the action.</span></span> |
|<span data-ttu-id="d678a-113">注释</span><span class="sxs-lookup"><span data-stu-id="d678a-113">comment</span></span>|<span data-ttu-id="d678a-114">String</span><span class="sxs-lookup"><span data-stu-id="d678a-114">String</span></span>|<span data-ttu-id="d678a-115">提供有关控件的可选注释。</span><span class="sxs-lookup"><span data-stu-id="d678a-115">Provides optional comment about the control.</span></span> |
|<span data-ttu-id="d678a-116">state</span><span class="sxs-lookup"><span data-stu-id="d678a-116">state</span></span>|<span data-ttu-id="d678a-117">String</span><span class="sxs-lookup"><span data-stu-id="d678a-117">String</span></span>|<span data-ttu-id="d678a-118">控件的状态，可通过修补程序命令进行修改（例如，忽略、thirdParty）。</span><span class="sxs-lookup"><span data-stu-id="d678a-118">State of the control, which can be modified via a PATCH command (for example, ignored, thirdParty).</span></span> |
|<span data-ttu-id="d678a-119">updatedBy</span><span class="sxs-lookup"><span data-stu-id="d678a-119">updatedBy</span></span>|<span data-ttu-id="d678a-120">String</span><span class="sxs-lookup"><span data-stu-id="d678a-120">String</span></span>|<span data-ttu-id="d678a-121">更新了租户状态的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="d678a-121">ID of the user who updated tenant state.</span></span> |
|<span data-ttu-id="d678a-122">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d678a-122">updatedDateTime</span></span>|<span data-ttu-id="d678a-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d678a-123">DateTimeOffset</span></span>|<span data-ttu-id="d678a-124">控件状态的更新时间。</span><span class="sxs-lookup"><span data-stu-id="d678a-124">Time at which the control state was updated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d678a-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d678a-125">JSON representation</span></span>
 <span data-ttu-id="d678a-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d678a-126">The following is a JSON representation of the resource.</span></span>
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
