---
title: lanManagerAuthenticationLevel 枚举类型
description: LanManagerAuthenticationLevel 的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 92cb5b32d8b4768af63d92461597c32f858c0a7c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946152"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="4d86d-103">lanManagerAuthenticationLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4d86d-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="4d86d-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4d86d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d86d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4d86d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d86d-106">LanManagerAuthenticationLevel 的可能值</span><span class="sxs-lookup"><span data-stu-id="4d86d-106">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="4d86d-107">成员</span><span class="sxs-lookup"><span data-stu-id="4d86d-107">Members</span></span>
|<span data-ttu-id="4d86d-108">成员</span><span class="sxs-lookup"><span data-stu-id="4d86d-108">Member</span></span>|<span data-ttu-id="4d86d-109">值</span><span class="sxs-lookup"><span data-stu-id="4d86d-109">Value</span></span>|<span data-ttu-id="4d86d-110">说明</span><span class="sxs-lookup"><span data-stu-id="4d86d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d86d-111">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="4d86d-111">lmAndNltm</span></span>|<span data-ttu-id="4d86d-112">0</span><span class="sxs-lookup"><span data-stu-id="4d86d-112">0</span></span>|<span data-ttu-id="4d86d-113">发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="4d86d-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="4d86d-114">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="4d86d-114">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="4d86d-115">1</span><span class="sxs-lookup"><span data-stu-id="4d86d-115">1</span></span>|<span data-ttu-id="4d86d-116">发送 LM & NTLM-使用 NTLMv2 会话安全性 (如果协商)</span><span class="sxs-lookup"><span data-stu-id="4d86d-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="4d86d-117">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="4d86d-117">lmAndNtlmOnly</span></span>|<span data-ttu-id="4d86d-118">双面</span><span class="sxs-lookup"><span data-stu-id="4d86d-118">2</span></span>|<span data-ttu-id="4d86d-119">仅发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="4d86d-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="4d86d-120">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="4d86d-120">lmAndNtlmV2</span></span>|<span data-ttu-id="4d86d-121">第三章</span><span class="sxs-lookup"><span data-stu-id="4d86d-121">3</span></span>|<span data-ttu-id="4d86d-122">仅发送 LM & NTLMv2 响应</span><span class="sxs-lookup"><span data-stu-id="4d86d-122">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="4d86d-123">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="4d86d-123">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="4d86d-124">4</span><span class="sxs-lookup"><span data-stu-id="4d86d-124">4</span></span>|<span data-ttu-id="4d86d-125">仅发送 LM & NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="4d86d-125">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="4d86d-126">拒绝 LM</span><span class="sxs-lookup"><span data-stu-id="4d86d-126">Refuse LM</span></span>|
|<span data-ttu-id="4d86d-127">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="4d86d-127">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="4d86d-128">5</span><span class="sxs-lookup"><span data-stu-id="4d86d-128">5</span></span>|<span data-ttu-id="4d86d-129">仅发送 LM & NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="4d86d-129">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="4d86d-130">拒绝 LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="4d86d-130">Refuse LM & NTLM</span></span>|




