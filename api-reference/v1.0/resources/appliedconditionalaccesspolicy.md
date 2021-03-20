---
title: appliedConditionalAccessPolicy 资源类型
description: 指示与由相应登录活动触发的已应用的条件访问策略相关的属性。
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: e69125d4119e7d2083189f459ad7c86816ddcd8e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952555"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a><span data-ttu-id="f3d5a-103">appliedConditionalAccessPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="f3d5a-103">appliedConditionalAccessPolicy resource type</span></span>

<span data-ttu-id="f3d5a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3d5a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f3d5a-105">指示与由相应登录活动触发的已应用的条件访问策略相关的属性。</span><span class="sxs-lookup"><span data-stu-id="f3d5a-105">Indicates the attributes related to applied conditional access policy or policies that are triggered by the corresponding sign-in activity.</span></span>

## <a name="properties"></a><span data-ttu-id="f3d5a-106">属性</span><span class="sxs-lookup"><span data-stu-id="f3d5a-106">Properties</span></span>

| <span data-ttu-id="f3d5a-107">属性</span><span class="sxs-lookup"><span data-stu-id="f3d5a-107">Property</span></span>   | <span data-ttu-id="f3d5a-108">类型</span><span class="sxs-lookup"><span data-stu-id="f3d5a-108">Type</span></span> |<span data-ttu-id="f3d5a-109">说明</span><span class="sxs-lookup"><span data-stu-id="f3d5a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3d5a-110">displayName</span><span class="sxs-lookup"><span data-stu-id="f3d5a-110">displayName</span></span>|<span data-ttu-id="f3d5a-111">String</span><span class="sxs-lookup"><span data-stu-id="f3d5a-111">String</span></span>|<span data-ttu-id="f3d5a-112">请参阅条件访问策略的名称，例如 (Salesforce 需要 MFA") 。</span><span class="sxs-lookup"><span data-stu-id="f3d5a-112">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="f3d5a-113">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="f3d5a-113">enforcedGrantControls</span></span>|<span data-ttu-id="f3d5a-114">String collection</span><span class="sxs-lookup"><span data-stu-id="f3d5a-114">String collection</span></span>|<span data-ttu-id="f3d5a-115">请参阅条件访问策略强制实施的授予 (示例："需要多重身份验证") 。</span><span class="sxs-lookup"><span data-stu-id="f3d5a-115">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="f3d5a-116">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="f3d5a-116">enforcedSessionControls</span></span>|<span data-ttu-id="f3d5a-117">String collection</span><span class="sxs-lookup"><span data-stu-id="f3d5a-117">String collection</span></span>|<span data-ttu-id="f3d5a-118">引用条件访问策略强制的会话 (示例："要求应用强制执行的控件") 。</span><span class="sxs-lookup"><span data-stu-id="f3d5a-118">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="f3d5a-119">id</span><span class="sxs-lookup"><span data-stu-id="f3d5a-119">id</span></span>|<span data-ttu-id="f3d5a-120">String</span><span class="sxs-lookup"><span data-stu-id="f3d5a-120">String</span></span>|<span data-ttu-id="f3d5a-121">条件访问策略的标识符。</span><span class="sxs-lookup"><span data-stu-id="f3d5a-121">An identifier of the conditional access policy.</span></span>|
|<span data-ttu-id="f3d5a-122">result</span><span class="sxs-lookup"><span data-stu-id="f3d5a-122">result</span></span>|<span data-ttu-id="f3d5a-123">appliedConditionalAccessPolicyResult</span><span class="sxs-lookup"><span data-stu-id="f3d5a-123">appliedConditionalAccessPolicyResult</span></span>| <span data-ttu-id="f3d5a-124">指示触发的 CA 策略的结果。</span><span class="sxs-lookup"><span data-stu-id="f3d5a-124">Indicates the result of the CA policy that was triggered.</span></span> <span data-ttu-id="f3d5a-125">可能的值是：、、 (策略未应用，因为策略条件未) ， (这是因为策略处于禁用状态 `success` `failure` `notApplied` `notEnabled`) 、 `unknown` 、 `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="f3d5a-125">Possible values are: `success`, `failure`, `notApplied` (Policy isn't applied because policy conditions were not met),`notEnabled` (This is due to the policy in disabled state), `unknown`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f3d5a-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f3d5a-126">JSON representation</span></span>

<span data-ttu-id="f3d5a-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3d5a-127">Here is a JSON representation of the resource.</span></span>

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

