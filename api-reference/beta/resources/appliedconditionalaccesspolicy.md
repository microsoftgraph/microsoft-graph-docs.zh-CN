---
title: appliedConditionalAccessPolicy 资源类型
description: 指示与由相应登录活动触发的已应用的条件访问策略相关的属性。
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: ffb91b315772d017ce039237e353df68daa47bfc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952221"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a><span data-ttu-id="a3d07-103">appliedConditionalAccessPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="a3d07-103">appliedConditionalAccessPolicy resource type</span></span>

<span data-ttu-id="a3d07-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3d07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3d07-105">指示与由相应登录活动触发的已应用的条件访问策略相关的属性。</span><span class="sxs-lookup"><span data-stu-id="a3d07-105">Indicates the attributes related to applied conditional access policy or policies that are triggered by the corresponding sign-in activity.</span></span>

## <a name="properties"></a><span data-ttu-id="a3d07-106">属性</span><span class="sxs-lookup"><span data-stu-id="a3d07-106">Properties</span></span>

| <span data-ttu-id="a3d07-107">属性</span><span class="sxs-lookup"><span data-stu-id="a3d07-107">Property</span></span>   | <span data-ttu-id="a3d07-108">类型</span><span class="sxs-lookup"><span data-stu-id="a3d07-108">Type</span></span> |<span data-ttu-id="a3d07-109">说明</span><span class="sxs-lookup"><span data-stu-id="a3d07-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3d07-110">conditionsSatisfied</span><span class="sxs-lookup"><span data-stu-id="a3d07-110">conditionsSatisfied</span></span>|<span data-ttu-id="a3d07-111">conditionalAccessConditions</span><span class="sxs-lookup"><span data-stu-id="a3d07-111">conditionalAccessConditions</span></span>|<span data-ttu-id="a3d07-112">引用满足的条件访问策略条件。</span><span class="sxs-lookup"><span data-stu-id="a3d07-112">Refers to the conditional access policy conditions that are satisfied.</span></span> <span data-ttu-id="a3d07-113">可取值为：`none`、`application`、`users`、`devicePlatform`、`location`、`clientType`、`signInRisk`、`userRisk`、`time`、`deviceState`、`client`。</span><span class="sxs-lookup"><span data-stu-id="a3d07-113">Possible values are: `none`, `application`, `users`, `devicePlatform`, `location`, `clientType`, `signInRisk`, `userRisk`, `time`, `deviceState`, `client`.</span></span>|
|<span data-ttu-id="a3d07-114">conditionsNotSatisfied</span><span class="sxs-lookup"><span data-stu-id="a3d07-114">conditionsNotSatisfied</span></span>|<span data-ttu-id="a3d07-115">conditionalAccessConditions</span><span class="sxs-lookup"><span data-stu-id="a3d07-115">conditionalAccessConditions</span></span>|<span data-ttu-id="a3d07-116">引用不满足的条件访问策略条件。</span><span class="sxs-lookup"><span data-stu-id="a3d07-116">Refers to the conditional access policy conditions that are not satisfied.</span></span> <span data-ttu-id="a3d07-117">可取值为：`none`、`application`、`users`、`devicePlatform`、`location`、`clientType`、`signInRisk`、`userRisk`、`time`、`deviceState`、`client`。</span><span class="sxs-lookup"><span data-stu-id="a3d07-117">Possible values are: `none`, `application`, `users`, `devicePlatform`, `location`, `clientType`, `signInRisk`, `userRisk`, `time`, `deviceState`, `client`.</span></span>|
|<span data-ttu-id="a3d07-118">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="a3d07-118">enforcedGrantControls</span></span>|<span data-ttu-id="a3d07-119">String collection</span><span class="sxs-lookup"><span data-stu-id="a3d07-119">String collection</span></span>|<span data-ttu-id="a3d07-120">请参阅条件访问策略强制实施的授予 (示例："需要多重身份验证") 。</span><span class="sxs-lookup"><span data-stu-id="a3d07-120">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="a3d07-121">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="a3d07-121">enforcedSessionControls</span></span>|<span data-ttu-id="a3d07-122">String collection</span><span class="sxs-lookup"><span data-stu-id="a3d07-122">String collection</span></span>|<span data-ttu-id="a3d07-123">引用条件访问策略强制的会话 (示例："要求应用强制执行的控件") 。</span><span class="sxs-lookup"><span data-stu-id="a3d07-123">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="a3d07-124">id</span><span class="sxs-lookup"><span data-stu-id="a3d07-124">id</span></span>|<span data-ttu-id="a3d07-125">String</span><span class="sxs-lookup"><span data-stu-id="a3d07-125">String</span></span>|<span data-ttu-id="a3d07-126">条件访问策略的标识符。</span><span class="sxs-lookup"><span data-stu-id="a3d07-126">Identifier of the conditional access policy.</span></span>|
|<span data-ttu-id="a3d07-127">result</span><span class="sxs-lookup"><span data-stu-id="a3d07-127">result</span></span>|<span data-ttu-id="a3d07-128">appliedConditionalAccessPolicyResult</span><span class="sxs-lookup"><span data-stu-id="a3d07-128">appliedConditionalAccessPolicyResult</span></span>| <span data-ttu-id="a3d07-129">指示触发的 CA 策略的结果。</span><span class="sxs-lookup"><span data-stu-id="a3d07-129">Indicates the result of the CA policy that was triggered.</span></span> <span data-ttu-id="a3d07-130">可能的值是：、、 (Policy 未应用，因为策略条件未满足) ， (这是因为策略处于禁用状态 `success` `failure` `notApplied` `notEnabled`) 、 `unknown` `unknownFutureValue` `reportOnlySuccess` `reportOnlyFailure` `reportOnlyNotApplied``reportOnlyInterrupted`</span><span class="sxs-lookup"><span data-stu-id="a3d07-130">Possible values are: `success`, `failure`, `notApplied` (Policy isn't applied because policy conditions were not met),`notEnabled` (This is due to the policy in disabled state), `unknown`, `unknownFutureValue`, `reportOnlySuccess`, `reportOnlyFailure`, `reportOnlyNotApplied`, `reportOnlyInterrupted`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a3d07-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3d07-131">JSON representation</span></span>

<span data-ttu-id="a3d07-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3d07-132">Here is a JSON representation of the resource.</span></span>

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
