---
title: lanManagerAuthenticationLevel 枚举类型
description: LanManagerAuthenticationLevel 的可能值
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 68af209a005dc1d7e8d25672f5e97e1d929ba25b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866911"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="40d7a-103">lanManagerAuthenticationLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="40d7a-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="40d7a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="40d7a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40d7a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="40d7a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40d7a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="40d7a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40d7a-107">LanManagerAuthenticationLevel 的可能值</span><span class="sxs-lookup"><span data-stu-id="40d7a-107">Possible values for LanManagerAuthenticationLevel</span></span>
## <a name="members"></a><span data-ttu-id="40d7a-108">成员</span><span class="sxs-lookup"><span data-stu-id="40d7a-108">Members</span></span>
|<span data-ttu-id="40d7a-109">成员</span><span class="sxs-lookup"><span data-stu-id="40d7a-109">Member</span></span>|<span data-ttu-id="40d7a-110">值</span><span class="sxs-lookup"><span data-stu-id="40d7a-110">Value</span></span>|<span data-ttu-id="40d7a-111">Description</span><span class="sxs-lookup"><span data-stu-id="40d7a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40d7a-112">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="40d7a-112">lmAndNltm</span></span>|<span data-ttu-id="40d7a-113">0</span><span class="sxs-lookup"><span data-stu-id="40d7a-113">0</span></span>|<span data-ttu-id="40d7a-114">发送 LM 和 NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="40d7a-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="40d7a-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="40d7a-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="40d7a-116">1</span><span class="sxs-lookup"><span data-stu-id="40d7a-116">1</span></span>|<span data-ttu-id="40d7a-117">如果协商，发送 LM 和 NTLM 使用 NTLMv2 会话安全</span><span class="sxs-lookup"><span data-stu-id="40d7a-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="40d7a-118">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="40d7a-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="40d7a-119">2</span><span class="sxs-lookup"><span data-stu-id="40d7a-119">2</span></span>|<span data-ttu-id="40d7a-120">发送 LM 和 NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="40d7a-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="40d7a-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="40d7a-121">lmAndNtlmV2</span></span>|<span data-ttu-id="40d7a-122">3</span><span class="sxs-lookup"><span data-stu-id="40d7a-122">3</span></span>|<span data-ttu-id="40d7a-123">发送 LM 和 NTLMv2 响应</span><span class="sxs-lookup"><span data-stu-id="40d7a-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="40d7a-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="40d7a-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="40d7a-125">4</span><span class="sxs-lookup"><span data-stu-id="40d7a-125">4</span></span>|<span data-ttu-id="40d7a-126">发送 LM 和 NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="40d7a-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="40d7a-127">拒绝 LM</span><span class="sxs-lookup"><span data-stu-id="40d7a-127">Refuse LM</span></span>|
|<span data-ttu-id="40d7a-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="40d7a-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="40d7a-129">5</span><span class="sxs-lookup"><span data-stu-id="40d7a-129">5</span></span>|<span data-ttu-id="40d7a-130">发送 LM 和 NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="40d7a-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="40d7a-131">拒绝 LM 和 NTLM</span><span class="sxs-lookup"><span data-stu-id="40d7a-131">Refuse LM & NTLM</span></span>|





