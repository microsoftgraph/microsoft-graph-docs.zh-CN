---
title: appliedConditionalAccessPolicy 资源类型
description: 指示与由相应登录活动触发的已应用的条件访问策略相关的属性。
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3aa114c23888ccc6852314e2274b8a89ca440344
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761526"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a><span data-ttu-id="35b1e-103">appliedConditionalAccessPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="35b1e-103">appliedConditionalAccessPolicy resource type</span></span>

<span data-ttu-id="35b1e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35b1e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35b1e-105">指示与由相应登录活动触发的已应用的条件访问策略相关的属性。</span><span class="sxs-lookup"><span data-stu-id="35b1e-105">Indicates the attributes related to applied conditional access policy or policies that are triggered by the corresponding sign-in activity.</span></span>

## <a name="properties"></a><span data-ttu-id="35b1e-106">属性</span><span class="sxs-lookup"><span data-stu-id="35b1e-106">Properties</span></span>

| <span data-ttu-id="35b1e-107">属性</span><span class="sxs-lookup"><span data-stu-id="35b1e-107">Property</span></span>   | <span data-ttu-id="35b1e-108">类型</span><span class="sxs-lookup"><span data-stu-id="35b1e-108">Type</span></span> |<span data-ttu-id="35b1e-109">说明</span><span class="sxs-lookup"><span data-stu-id="35b1e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35b1e-110">displayName</span><span class="sxs-lookup"><span data-stu-id="35b1e-110">displayName</span></span>|<span data-ttu-id="35b1e-111">字符串</span><span class="sxs-lookup"><span data-stu-id="35b1e-111">String</span></span>|<span data-ttu-id="35b1e-112">请参阅条件访问策略的名称，例如 (Salesforce 需要 MFA") 。</span><span class="sxs-lookup"><span data-stu-id="35b1e-112">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="35b1e-113">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="35b1e-113">enforcedGrantControls</span></span>|<span data-ttu-id="35b1e-114">字符串集合</span><span class="sxs-lookup"><span data-stu-id="35b1e-114">String collection</span></span>|<span data-ttu-id="35b1e-115">请参阅条件访问策略强制实施的授予 (示例："需要多重身份验证") 。</span><span class="sxs-lookup"><span data-stu-id="35b1e-115">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="35b1e-116">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="35b1e-116">enforcedSessionControls</span></span>|<span data-ttu-id="35b1e-117">字符串集合</span><span class="sxs-lookup"><span data-stu-id="35b1e-117">String collection</span></span>|<span data-ttu-id="35b1e-118">引用条件访问策略强制的会话 (示例："要求应用强制执行的控件") 。</span><span class="sxs-lookup"><span data-stu-id="35b1e-118">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="35b1e-119">id</span><span class="sxs-lookup"><span data-stu-id="35b1e-119">id</span></span>|<span data-ttu-id="35b1e-120">字符串</span><span class="sxs-lookup"><span data-stu-id="35b1e-120">String</span></span>|<span data-ttu-id="35b1e-121">条件访问策略的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="35b1e-121">Unique GUID of the conditional access policy.</span></span>|
|<span data-ttu-id="35b1e-122">result</span><span class="sxs-lookup"><span data-stu-id="35b1e-122">result</span></span>|<span data-ttu-id="35b1e-123">字符串</span><span class="sxs-lookup"><span data-stu-id="35b1e-123">String</span></span>| <span data-ttu-id="35b1e-124">指示触发的 CA 策略的结果。</span><span class="sxs-lookup"><span data-stu-id="35b1e-124">Indicates the result of the CA policy that was triggered.</span></span> <span data-ttu-id="35b1e-125">可能的值是：</span><span class="sxs-lookup"><span data-stu-id="35b1e-125">Possible values are:</span></span><br/>`success`<br/>`failure`<br/><span data-ttu-id="35b1e-126">`notApplied` - 未应用策略，因为未满足策略条件。</span><span class="sxs-lookup"><span data-stu-id="35b1e-126">`notApplied` - Policy isn't applied because policy conditions were not met.</span></span><br/><span data-ttu-id="35b1e-127">`notEnabled` - 这是因为策略处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="35b1e-127">`notEnabled` - This is due to the policy in disabled state.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35b1e-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35b1e-128">JSON representation</span></span>

<span data-ttu-id="35b1e-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35b1e-129">Here is a JSON representation of the resource.</span></span>

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

