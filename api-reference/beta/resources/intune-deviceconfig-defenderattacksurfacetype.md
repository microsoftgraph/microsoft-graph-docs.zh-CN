---
title: defenderAttackSurfaceType 枚举类型
description: Defender 攻击面减少规则的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 435ce477f60f14437a05e22fd5c670cbe1b25796
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256650"
---
# <a name="defenderattacksurfacetype-enum-type"></a><span data-ttu-id="cc0d3-103">defenderAttackSurfaceType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cc0d3-103">defenderAttackSurfaceType enum type</span></span>

<span data-ttu-id="cc0d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc0d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc0d3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cc0d3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc0d3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cc0d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc0d3-107">Defender 攻击面减少规则的可能值</span><span class="sxs-lookup"><span data-stu-id="cc0d3-107">Possible values of Defender Attack Surface Reduction Rules</span></span>

## <a name="members"></a><span data-ttu-id="cc0d3-108">成员</span><span class="sxs-lookup"><span data-stu-id="cc0d3-108">Members</span></span>
|<span data-ttu-id="cc0d3-109">成员</span><span class="sxs-lookup"><span data-stu-id="cc0d3-109">Member</span></span>|<span data-ttu-id="cc0d3-110">值</span><span class="sxs-lookup"><span data-stu-id="cc0d3-110">Value</span></span>|<span data-ttu-id="cc0d3-111">说明</span><span class="sxs-lookup"><span data-stu-id="cc0d3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc0d3-112">定制</span><span class="sxs-lookup"><span data-stu-id="cc0d3-112">userDefined</span></span>|<span data-ttu-id="cc0d3-113">0</span><span class="sxs-lookup"><span data-stu-id="cc0d3-113">0</span></span>|<span data-ttu-id="cc0d3-114">默认值，它禁用攻击面降低规则。</span><span class="sxs-lookup"><span data-stu-id="cc0d3-114">Default, which disables attack surface reduction rule.</span></span>|
|<span data-ttu-id="cc0d3-115">数据</span><span class="sxs-lookup"><span data-stu-id="cc0d3-115">block</span></span>|<span data-ttu-id="cc0d3-116">1</span><span class="sxs-lookup"><span data-stu-id="cc0d3-116">1</span></span>|<span data-ttu-id="cc0d3-117">启用攻击面降低规则。</span><span class="sxs-lookup"><span data-stu-id="cc0d3-117">Enable the attack surface reduction rule.</span></span>|
|<span data-ttu-id="cc0d3-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="cc0d3-118">auditMode</span></span>|<span data-ttu-id="cc0d3-119">双面</span><span class="sxs-lookup"><span data-stu-id="cc0d3-119">2</span></span>|<span data-ttu-id="cc0d3-120">如果启用，请评估 ASR 规则将如何影响你的组织。</span><span class="sxs-lookup"><span data-stu-id="cc0d3-120">Evaluate how the ASR rule would impact your organization if enabled.</span></span> <span data-ttu-id="cc0d3-121">不会更改功能，而是生成日志。</span><span class="sxs-lookup"><span data-stu-id="cc0d3-121">Does not change functionality but generate logs.</span></span>|
|<span data-ttu-id="cc0d3-122">警告</span><span class="sxs-lookup"><span data-stu-id="cc0d3-122">warn</span></span>|<span data-ttu-id="cc0d3-123">6 </span><span class="sxs-lookup"><span data-stu-id="cc0d3-123">6</span></span>|<span data-ttu-id="cc0d3-124">向最终用户发出的警告消息，能够绕过受攻击面降低规则阻止的阻止。</span><span class="sxs-lookup"><span data-stu-id="cc0d3-124">Warning message to end user with ability to bypass block from attack surface reduction rule.</span></span>|
|<span data-ttu-id="cc0d3-125">disable</span><span class="sxs-lookup"><span data-stu-id="cc0d3-125">disable</span></span>|<span data-ttu-id="cc0d3-126">99</span><span class="sxs-lookup"><span data-stu-id="cc0d3-126">99</span></span>|<span data-ttu-id="cc0d3-127">禁用攻击面降低规则</span><span class="sxs-lookup"><span data-stu-id="cc0d3-127">Disable the attack surface reduction rule</span></span>|




