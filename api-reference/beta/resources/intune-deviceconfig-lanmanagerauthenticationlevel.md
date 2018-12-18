---
title: lanManagerAuthenticationLevel 枚举类型
description: LanManagerAuthenticationLevel 的可能值
author: tfitzmac
ms.openlocfilehash: fd5d63f262b9b6e9a27060725e721cb81c495a57
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308741"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="73fbb-103">lanManagerAuthenticationLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="73fbb-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="73fbb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="73fbb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73fbb-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="73fbb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73fbb-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="73fbb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73fbb-107">LanManagerAuthenticationLevel 的可能值</span><span class="sxs-lookup"><span data-stu-id="73fbb-107">Possible values for LanManagerAuthenticationLevel</span></span>
## <a name="members"></a><span data-ttu-id="73fbb-108">成员</span><span class="sxs-lookup"><span data-stu-id="73fbb-108">Members</span></span>
|<span data-ttu-id="73fbb-109">成员</span><span class="sxs-lookup"><span data-stu-id="73fbb-109">Member</span></span>|<span data-ttu-id="73fbb-110">值</span><span class="sxs-lookup"><span data-stu-id="73fbb-110">Value</span></span>|<span data-ttu-id="73fbb-111">说明</span><span class="sxs-lookup"><span data-stu-id="73fbb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73fbb-112">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="73fbb-112">lmAndNltm</span></span>|<span data-ttu-id="73fbb-113">0</span><span class="sxs-lookup"><span data-stu-id="73fbb-113">0</span></span>|<span data-ttu-id="73fbb-114">发送 LM 和 NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="73fbb-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="73fbb-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="73fbb-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="73fbb-116">1</span><span class="sxs-lookup"><span data-stu-id="73fbb-116">1</span></span>|<span data-ttu-id="73fbb-117">如果协商，发送 LM 和 NTLM 使用 NTLMv2 会话安全</span><span class="sxs-lookup"><span data-stu-id="73fbb-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="73fbb-118">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="73fbb-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="73fbb-119">2</span><span class="sxs-lookup"><span data-stu-id="73fbb-119">2</span></span>|<span data-ttu-id="73fbb-120">发送 LM 和 NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="73fbb-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="73fbb-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="73fbb-121">lmAndNtlmV2</span></span>|<span data-ttu-id="73fbb-122">3</span><span class="sxs-lookup"><span data-stu-id="73fbb-122">3</span></span>|<span data-ttu-id="73fbb-123">发送 LM 和 NTLMv2 响应</span><span class="sxs-lookup"><span data-stu-id="73fbb-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="73fbb-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="73fbb-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="73fbb-125">4</span><span class="sxs-lookup"><span data-stu-id="73fbb-125">4</span></span>|<span data-ttu-id="73fbb-126">发送 LM 和 NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="73fbb-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="73fbb-127">拒绝 LM</span><span class="sxs-lookup"><span data-stu-id="73fbb-127">Refuse LM</span></span>|
|<span data-ttu-id="73fbb-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="73fbb-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="73fbb-129">5</span><span class="sxs-lookup"><span data-stu-id="73fbb-129">5</span></span>|<span data-ttu-id="73fbb-130">发送 LM 和 NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="73fbb-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="73fbb-131">拒绝 LM 和 NTLM</span><span class="sxs-lookup"><span data-stu-id="73fbb-131">Refuse LM & NTLM</span></span>|





