---
title: conditionalAccessPolicy 资源类型
description: 指示与相应登录活动触发的条件访问策略或策略相关的属性
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2c45be8ee32c26187ccf42154ba6c06b60f5efc1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973214"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="81b14-103">conditionalAccessPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="81b14-103">conditionalAccessPolicy resource type</span></span>
<span data-ttu-id="81b14-104">指示与相应登录活动触发的条件访问策略或策略相关的属性</span><span class="sxs-lookup"><span data-stu-id="81b14-104">Indicates the attributes related a conditional access policy or policies that's triggered by the corresponding sign-in activity</span></span>



## <a name="properties"></a><span data-ttu-id="81b14-105">属性</span><span class="sxs-lookup"><span data-stu-id="81b14-105">Properties</span></span>
| <span data-ttu-id="81b14-106">属性</span><span class="sxs-lookup"><span data-stu-id="81b14-106">Property</span></span>     | <span data-ttu-id="81b14-107">类型</span><span class="sxs-lookup"><span data-stu-id="81b14-107">Type</span></span>   |<span data-ttu-id="81b14-108">说明</span><span class="sxs-lookup"><span data-stu-id="81b14-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81b14-109">displayName</span><span class="sxs-lookup"><span data-stu-id="81b14-109">displayName</span></span>|<span data-ttu-id="81b14-110">String</span><span class="sxs-lookup"><span data-stu-id="81b14-110">String</span></span>|<span data-ttu-id="81b14-111">表示条件访问策略的名称 (示例: "需要对 Salesforce 进行 MFA")。</span><span class="sxs-lookup"><span data-stu-id="81b14-111">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="81b14-112">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="81b14-112">enforcedGrantControls</span></span>|<span data-ttu-id="81b14-113">String collection</span><span class="sxs-lookup"><span data-stu-id="81b14-113">String collection</span></span>|<span data-ttu-id="81b14-114">指由条件访问策略强制实施的授予控制 (示例: "需要多重身份验证")。</span><span class="sxs-lookup"><span data-stu-id="81b14-114">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="81b14-115">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="81b14-115">enforcedSessionControls</span></span>|<span data-ttu-id="81b14-116">String collection</span><span class="sxs-lookup"><span data-stu-id="81b14-116">String collection</span></span>|<span data-ttu-id="81b14-117">引用由条件访问策略强制实施的会话控件 (示例: "需要应用强制性控制措施")。</span><span class="sxs-lookup"><span data-stu-id="81b14-117">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="81b14-118">id</span><span class="sxs-lookup"><span data-stu-id="81b14-118">id</span></span>|<span data-ttu-id="81b14-119">String</span><span class="sxs-lookup"><span data-stu-id="81b14-119">String</span></span>|<span data-ttu-id="81b14-120">条件访问策略的唯一 GUID</span><span class="sxs-lookup"><span data-stu-id="81b14-120">Unique GUID of the conditional access policy</span></span>|
|<span data-ttu-id="81b14-121">result</span><span class="sxs-lookup"><span data-stu-id="81b14-121">result</span></span>|<span data-ttu-id="81b14-122">String</span><span class="sxs-lookup"><span data-stu-id="81b14-122">String</span></span>| <span data-ttu-id="81b14-123">指示已触发的 CA 策略的结果。可能的值包括:</span><span class="sxs-lookup"><span data-stu-id="81b14-123">Indicates the result of the CA policy that was triggered.Possible values are:</span></span><br/> `success` <br/> `failure` <br/> <span data-ttu-id="81b14-124">`notApplied`-由于未满足策略条件, 因此未应用策略。</span><span class="sxs-lookup"><span data-stu-id="81b14-124">`notApplied` - Policy isn't applied because policy conditions were not met.</span></span> <br/> <span data-ttu-id="81b14-125">`notEnabled`-这是由于策略处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="81b14-125">`notEnabled` - This is due to the policy in disabled state.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81b14-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81b14-126">JSON representation</span></span>

<span data-ttu-id="81b14-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81b14-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
}-->

```json
{
  "displayName": "String",
  "enforcedGrantControls": ["String"],
  "enforcedSessionControls": ["String"],
  "id": "String",
  "result": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
