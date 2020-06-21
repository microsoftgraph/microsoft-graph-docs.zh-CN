---
title: appliedConditionalAccessPolicy 资源类型
description: 指示与应用的条件访问策略相关的属性，或与相应登录活动触发的策略相关的属性。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0e58058a174b630daa5022aed0dff78b7c2f3099
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44788687"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a><span data-ttu-id="6a976-103">appliedConditionalAccessPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a976-103">appliedConditionalAccessPolicy resource type</span></span>

<span data-ttu-id="6a976-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a976-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6a976-105">指示与应用的条件访问策略相关的属性，或与相应登录活动触发的策略相关的属性。</span><span class="sxs-lookup"><span data-stu-id="6a976-105">Indicates the attributes related to applied conditional access policy or policies that are triggered by the corresponding sign-in activity.</span></span>

## <a name="properties"></a><span data-ttu-id="6a976-106">属性</span><span class="sxs-lookup"><span data-stu-id="6a976-106">Properties</span></span>

| <span data-ttu-id="6a976-107">属性</span><span class="sxs-lookup"><span data-stu-id="6a976-107">Property</span></span>   | <span data-ttu-id="6a976-108">类型</span><span class="sxs-lookup"><span data-stu-id="6a976-108">Type</span></span> |<span data-ttu-id="6a976-109">说明</span><span class="sxs-lookup"><span data-stu-id="6a976-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a976-110">displayName</span><span class="sxs-lookup"><span data-stu-id="6a976-110">displayName</span></span>|<span data-ttu-id="6a976-111">String</span><span class="sxs-lookup"><span data-stu-id="6a976-111">String</span></span>|<span data-ttu-id="6a976-112">表示条件访问策略的名称（示例： "需要对 Salesforce 进行 MFA"）。</span><span class="sxs-lookup"><span data-stu-id="6a976-112">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="6a976-113">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="6a976-113">enforcedGrantControls</span></span>|<span data-ttu-id="6a976-114">String collection</span><span class="sxs-lookup"><span data-stu-id="6a976-114">String collection</span></span>|<span data-ttu-id="6a976-115">指由条件访问策略强制实施的授予控制（示例： "需要多重身份验证"）。</span><span class="sxs-lookup"><span data-stu-id="6a976-115">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="6a976-116">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="6a976-116">enforcedSessionControls</span></span>|<span data-ttu-id="6a976-117">String collection</span><span class="sxs-lookup"><span data-stu-id="6a976-117">String collection</span></span>|<span data-ttu-id="6a976-118">引用由条件访问策略强制实施的会话控件（示例： "需要应用强制性控制措施"）。</span><span class="sxs-lookup"><span data-stu-id="6a976-118">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="6a976-119">id</span><span class="sxs-lookup"><span data-stu-id="6a976-119">id</span></span>|<span data-ttu-id="6a976-120">String</span><span class="sxs-lookup"><span data-stu-id="6a976-120">String</span></span>|<span data-ttu-id="6a976-121">条件访问策略的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="6a976-121">Unique GUID of the conditional access policy.</span></span>|
|<span data-ttu-id="6a976-122">result</span><span class="sxs-lookup"><span data-stu-id="6a976-122">result</span></span>|<span data-ttu-id="6a976-123">String</span><span class="sxs-lookup"><span data-stu-id="6a976-123">String</span></span>| <span data-ttu-id="6a976-124">指示已触发的 CA 策略的结果。</span><span class="sxs-lookup"><span data-stu-id="6a976-124">Indicates the result of the CA policy that was triggered.</span></span> <span data-ttu-id="6a976-125">可能的值是：</span><span class="sxs-lookup"><span data-stu-id="6a976-125">Possible values are:</span></span><br/>`success`<br/>`failure`<br/><span data-ttu-id="6a976-126">`notApplied`-由于未满足策略条件，因此未应用策略。</span><span class="sxs-lookup"><span data-stu-id="6a976-126">`notApplied` - Policy isn't applied because policy conditions were not met.</span></span><br/><span data-ttu-id="6a976-127">`notEnabled`-这是由于策略处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="6a976-127">`notEnabled` - This is due to the policy in disabled state.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6a976-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a976-128">JSON representation</span></span>

<span data-ttu-id="6a976-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a976-129">Here is a JSON representation of the resource.</span></span>

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
