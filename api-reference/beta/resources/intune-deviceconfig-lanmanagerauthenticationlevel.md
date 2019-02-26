---
title: lanManagerAuthenticationLevel 枚举类型
description: LanManagerAuthenticationLevel 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63f04f1ef2fc12fa0352aeec803c46fb4ebab3d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166568"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="431a8-103">lanManagerAuthenticationLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="431a8-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="431a8-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="431a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="431a8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="431a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="431a8-106">LanManagerAuthenticationLevel 的可能值</span><span class="sxs-lookup"><span data-stu-id="431a8-106">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="431a8-107">成员</span><span class="sxs-lookup"><span data-stu-id="431a8-107">Members</span></span>
|<span data-ttu-id="431a8-108">成员</span><span class="sxs-lookup"><span data-stu-id="431a8-108">Member</span></span>|<span data-ttu-id="431a8-109">值</span><span class="sxs-lookup"><span data-stu-id="431a8-109">Value</span></span>|<span data-ttu-id="431a8-110">说明</span><span class="sxs-lookup"><span data-stu-id="431a8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="431a8-111">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="431a8-111">lmAndNltm</span></span>|<span data-ttu-id="431a8-112">0</span><span class="sxs-lookup"><span data-stu-id="431a8-112">0</span></span>|<span data-ttu-id="431a8-113">发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="431a8-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="431a8-114">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="431a8-114">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="431a8-115">1</span><span class="sxs-lookup"><span data-stu-id="431a8-115">1</span></span>|<span data-ttu-id="431a8-116">发送 LM & NTLM-使用 NTLMv2 会话安全性 (如果协商)</span><span class="sxs-lookup"><span data-stu-id="431a8-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="431a8-117">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="431a8-117">lmAndNtlmOnly</span></span>|<span data-ttu-id="431a8-118">双面</span><span class="sxs-lookup"><span data-stu-id="431a8-118">2</span></span>|<span data-ttu-id="431a8-119">仅发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="431a8-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="431a8-120">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="431a8-120">lmAndNtlmV2</span></span>|<span data-ttu-id="431a8-121">第三章</span><span class="sxs-lookup"><span data-stu-id="431a8-121">3</span></span>|<span data-ttu-id="431a8-122">仅发送 LM & NTLMv2 响应</span><span class="sxs-lookup"><span data-stu-id="431a8-122">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="431a8-123">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="431a8-123">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="431a8-124">4</span><span class="sxs-lookup"><span data-stu-id="431a8-124">4</span></span>|<span data-ttu-id="431a8-125">仅发送 LM & NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="431a8-125">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="431a8-126">拒绝 LM</span><span class="sxs-lookup"><span data-stu-id="431a8-126">Refuse LM</span></span>|
|<span data-ttu-id="431a8-127">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="431a8-127">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="431a8-128">5</span><span class="sxs-lookup"><span data-stu-id="431a8-128">5</span></span>|<span data-ttu-id="431a8-129">仅发送 LM & NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="431a8-129">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="431a8-130">拒绝 LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="431a8-130">Refuse LM & NTLM</span></span>|




