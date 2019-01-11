---
title: conditionalAccessPolicy 资源类型
description: 指示由相应的登录活动触发条件的访问策略相关的属性
localization_priority: Normal
ms.openlocfilehash: 7b043e739f84715fb02fbdbd25599e5cfccc284a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820641"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="23bfc-103">conditionalAccessPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="23bfc-103">conditionalAccessPolicy resource type</span></span>
<span data-ttu-id="23bfc-104">指示由相应的登录活动触发条件的访问策略相关的属性</span><span class="sxs-lookup"><span data-stu-id="23bfc-104">Indicates the attributes related a conditional access policy or policies that's triggered by the corresponding sign-in activity</span></span>



## <a name="properties"></a><span data-ttu-id="23bfc-105">属性</span><span class="sxs-lookup"><span data-stu-id="23bfc-105">Properties</span></span>
| <span data-ttu-id="23bfc-106">属性</span><span class="sxs-lookup"><span data-stu-id="23bfc-106">Property</span></span>     | <span data-ttu-id="23bfc-107">类型</span><span class="sxs-lookup"><span data-stu-id="23bfc-107">Type</span></span>   |<span data-ttu-id="23bfc-108">说明</span><span class="sxs-lookup"><span data-stu-id="23bfc-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23bfc-109">displayName</span><span class="sxs-lookup"><span data-stu-id="23bfc-109">displayName</span></span>|<span data-ttu-id="23bfc-110">字符串</span><span class="sxs-lookup"><span data-stu-id="23bfc-110">String</span></span>|<span data-ttu-id="23bfc-111">指的条件的访问策略的名称 (示例:"需要 MFA 的销售队伍")。</span><span class="sxs-lookup"><span data-stu-id="23bfc-111">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="23bfc-112">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="23bfc-112">enforcedGrantControls</span></span>|<span data-ttu-id="23bfc-113">String 集合</span><span class="sxs-lookup"><span data-stu-id="23bfc-113">String collection</span></span>|<span data-ttu-id="23bfc-114">指的是此条件访问策略强制实施的授予控件 (示例:"需要多因素身份验证")。</span><span class="sxs-lookup"><span data-stu-id="23bfc-114">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="23bfc-115">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="23bfc-115">enforcedSessionControls</span></span>|<span data-ttu-id="23bfc-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="23bfc-116">String collection</span></span>|<span data-ttu-id="23bfc-117">指的是此条件访问策略强制实施的会话控件 (示例:"需要应用程序强制实施控件")。</span><span class="sxs-lookup"><span data-stu-id="23bfc-117">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="23bfc-118">id</span><span class="sxs-lookup"><span data-stu-id="23bfc-118">id</span></span>|<span data-ttu-id="23bfc-119">字符串</span><span class="sxs-lookup"><span data-stu-id="23bfc-119">String</span></span>|<span data-ttu-id="23bfc-120">条件访问策略的唯一 GUID</span><span class="sxs-lookup"><span data-stu-id="23bfc-120">Unique GUID of the conditional access policy</span></span>|
|<span data-ttu-id="23bfc-121">结果</span><span class="sxs-lookup"><span data-stu-id="23bfc-121">result</span></span>|<span data-ttu-id="23bfc-122">字符串</span><span class="sxs-lookup"><span data-stu-id="23bfc-122">String</span></span>| <span data-ttu-id="23bfc-123">指示触发的 CA 策略的结果。可能的值为：</span><span class="sxs-lookup"><span data-stu-id="23bfc-123">Indicates the result of the CA policy that was triggered.Possible values are:</span></span><br/> `success` <br/> `failure` <br/> <span data-ttu-id="23bfc-124">`notApplied`由于策略条件不满足，不应用策略。</span><span class="sxs-lookup"><span data-stu-id="23bfc-124">`notApplied` - Policy isn't applied because policy conditions were not met.</span></span> <br/> <span data-ttu-id="23bfc-125">`notEnabled`-这是由于处于禁用状态策略。</span><span class="sxs-lookup"><span data-stu-id="23bfc-125">`notEnabled` - This is due to the policy in disabled state.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="23bfc-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23bfc-126">JSON representation</span></span>

<span data-ttu-id="23bfc-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23bfc-127">Here is a JSON representation of the resource.</span></span>

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
