---
title: lanManagerAuthenticationLevel 枚举类型
description: LanManagerAuthenticationLevel 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3b93f229661de3e2fbb28f764288983b2fd83bb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801244"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="cd414-103">lanManagerAuthenticationLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cd414-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="cd414-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cd414-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd414-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cd414-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd414-106">LanManagerAuthenticationLevel 的可能值</span><span class="sxs-lookup"><span data-stu-id="cd414-106">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="cd414-107">成员</span><span class="sxs-lookup"><span data-stu-id="cd414-107">Members</span></span>
|<span data-ttu-id="cd414-108">成员</span><span class="sxs-lookup"><span data-stu-id="cd414-108">Member</span></span>|<span data-ttu-id="cd414-109">值</span><span class="sxs-lookup"><span data-stu-id="cd414-109">Value</span></span>|<span data-ttu-id="cd414-110">说明</span><span class="sxs-lookup"><span data-stu-id="cd414-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd414-111">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="cd414-111">lmAndNltm</span></span>|<span data-ttu-id="cd414-112">0</span><span class="sxs-lookup"><span data-stu-id="cd414-112">0</span></span>|<span data-ttu-id="cd414-113">发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="cd414-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="cd414-114">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="cd414-114">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="cd414-115">1</span><span class="sxs-lookup"><span data-stu-id="cd414-115">1</span></span>|<span data-ttu-id="cd414-116">发送 LM & NTLM-使用 NTLMv2 会话安全性 (如果协商)</span><span class="sxs-lookup"><span data-stu-id="cd414-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="cd414-117">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="cd414-117">lmAndNtlmOnly</span></span>|<span data-ttu-id="cd414-118">双面</span><span class="sxs-lookup"><span data-stu-id="cd414-118">2</span></span>|<span data-ttu-id="cd414-119">仅发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="cd414-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="cd414-120">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="cd414-120">lmAndNtlmV2</span></span>|<span data-ttu-id="cd414-121">第三章</span><span class="sxs-lookup"><span data-stu-id="cd414-121">3</span></span>|<span data-ttu-id="cd414-122">仅发送 LM & NTLMv2 响应</span><span class="sxs-lookup"><span data-stu-id="cd414-122">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="cd414-123">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="cd414-123">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="cd414-124">4</span><span class="sxs-lookup"><span data-stu-id="cd414-124">4</span></span>|<span data-ttu-id="cd414-125">仅发送 LM & NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="cd414-125">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="cd414-126">拒绝 LM</span><span class="sxs-lookup"><span data-stu-id="cd414-126">Refuse LM</span></span>|
|<span data-ttu-id="cd414-127">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="cd414-127">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="cd414-128">5</span><span class="sxs-lookup"><span data-stu-id="cd414-128">5</span></span>|<span data-ttu-id="cd414-129">仅发送 LM & NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="cd414-129">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="cd414-130">拒绝 LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="cd414-130">Refuse LM & NTLM</span></span>|





