---
title: appliedConditionalAccessPolicy 资源类型
description: 指示与应用的条件访问策略相关的属性, 或与相应登录活动触发的策略相关的属性。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bb5562b07e60b10a36dafac37d5839d9bacc060a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629339"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a><span data-ttu-id="05444-103">appliedConditionalAccessPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="05444-103">appliedConditionalAccessPolicy resource type</span></span>

<span data-ttu-id="05444-104">指示与应用的条件访问策略相关的属性, 或与相应登录活动触发的策略相关的属性。</span><span class="sxs-lookup"><span data-stu-id="05444-104">Indicates the attributes related to applied conditional access policy or policies that are triggered by the corresponding sign-in activity.</span></span>

## <a name="properties"></a><span data-ttu-id="05444-105">属性</span><span class="sxs-lookup"><span data-stu-id="05444-105">Properties</span></span>

| <span data-ttu-id="05444-106">属性</span><span class="sxs-lookup"><span data-stu-id="05444-106">Property</span></span>   | <span data-ttu-id="05444-107">类型</span><span class="sxs-lookup"><span data-stu-id="05444-107">Type</span></span> |<span data-ttu-id="05444-108">说明</span><span class="sxs-lookup"><span data-stu-id="05444-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05444-109">displayName</span><span class="sxs-lookup"><span data-stu-id="05444-109">displayName</span></span>|<span data-ttu-id="05444-110">String</span><span class="sxs-lookup"><span data-stu-id="05444-110">String</span></span>|<span data-ttu-id="05444-111">表示条件访问策略的名称 (示例: "需要对 Salesforce 进行 MFA")。</span><span class="sxs-lookup"><span data-stu-id="05444-111">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="05444-112">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="05444-112">enforcedGrantControls</span></span>|<span data-ttu-id="05444-113">String collection</span><span class="sxs-lookup"><span data-stu-id="05444-113">String collection</span></span>|<span data-ttu-id="05444-114">指由条件访问策略强制实施的授予控制 (示例: "需要多重身份验证")。</span><span class="sxs-lookup"><span data-stu-id="05444-114">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="05444-115">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="05444-115">enforcedSessionControls</span></span>|<span data-ttu-id="05444-116">String collection</span><span class="sxs-lookup"><span data-stu-id="05444-116">String collection</span></span>|<span data-ttu-id="05444-117">引用由条件访问策略强制实施的会话控件 (示例: "需要应用强制性控制措施")。</span><span class="sxs-lookup"><span data-stu-id="05444-117">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="05444-118">id</span><span class="sxs-lookup"><span data-stu-id="05444-118">id</span></span>|<span data-ttu-id="05444-119">字符串</span><span class="sxs-lookup"><span data-stu-id="05444-119">String</span></span>|<span data-ttu-id="05444-120">条件访问 polic 的唯一 GUID</span><span class="sxs-lookup"><span data-stu-id="05444-120">Unique GUID of the conditional access polic.y</span></span>|
|<span data-ttu-id="05444-121">result</span><span class="sxs-lookup"><span data-stu-id="05444-121">result</span></span>|<span data-ttu-id="05444-122">字符串</span><span class="sxs-lookup"><span data-stu-id="05444-122">String</span></span>| <span data-ttu-id="05444-123">指示已触发的 CA 策略的结果。</span><span class="sxs-lookup"><span data-stu-id="05444-123">Indicates the result of the CA policy that was triggered.</span></span> <span data-ttu-id="05444-124">可能的值是：</span><span class="sxs-lookup"><span data-stu-id="05444-124">Possible values are:</span></span><br/>`success`<br/>`failure`<br/><span data-ttu-id="05444-125">`notApplied`-由于未满足策略条件, 因此未应用策略。</span><span class="sxs-lookup"><span data-stu-id="05444-125">`notApplied` - Policy isn't applied because policy conditions were not met.</span></span><br/><span data-ttu-id="05444-126">`notEnabled`-这是由于策略处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="05444-126">`notEnabled` - This is due to the policy in disabled state.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="05444-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05444-127">JSON representation</span></span>

<span data-ttu-id="05444-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05444-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
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
  "description": "appliedConditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
