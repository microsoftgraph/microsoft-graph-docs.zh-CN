---
title: lanManagerAuthenticationLevel 枚举类型
description: LanManagerAuthenticationLevel 的可能值
ms.openlocfilehash: 9fb8113c4953a0cabcecfbc5303b9f62f685d5ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041943"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="061f9-103">lanManagerAuthenticationLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="061f9-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="061f9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="061f9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="061f9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="061f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="061f9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="061f9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="061f9-107">LanManagerAuthenticationLevel 的可能值</span><span class="sxs-lookup"><span data-stu-id="061f9-107">Possible values for LanManagerAuthenticationLevel</span></span>
## <a name="members"></a><span data-ttu-id="061f9-108">成员</span><span class="sxs-lookup"><span data-stu-id="061f9-108">Members</span></span>
|<span data-ttu-id="061f9-109">成员</span><span class="sxs-lookup"><span data-stu-id="061f9-109">Member</span></span>|<span data-ttu-id="061f9-110">值</span><span class="sxs-lookup"><span data-stu-id="061f9-110">Value</span></span>|<span data-ttu-id="061f9-111">说明</span><span class="sxs-lookup"><span data-stu-id="061f9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="061f9-112">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="061f9-112">lmAndNltm</span></span>|<span data-ttu-id="061f9-113">0</span><span class="sxs-lookup"><span data-stu-id="061f9-113">0</span></span>|<span data-ttu-id="061f9-114">发送 LM 和 NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="061f9-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="061f9-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="061f9-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="061f9-116">1</span><span class="sxs-lookup"><span data-stu-id="061f9-116">1</span></span>|<span data-ttu-id="061f9-117">如果协商，发送 LM 和 NTLM 使用 NTLMv2 会话安全</span><span class="sxs-lookup"><span data-stu-id="061f9-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="061f9-118">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="061f9-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="061f9-119">2</span><span class="sxs-lookup"><span data-stu-id="061f9-119">2</span></span>|<span data-ttu-id="061f9-120">发送 LM 和 NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="061f9-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="061f9-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="061f9-121">lmAndNtlmV2</span></span>|<span data-ttu-id="061f9-122">3</span><span class="sxs-lookup"><span data-stu-id="061f9-122">3</span></span>|<span data-ttu-id="061f9-123">发送 LM 和 NTLMv2 响应</span><span class="sxs-lookup"><span data-stu-id="061f9-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="061f9-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="061f9-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="061f9-125">4</span><span class="sxs-lookup"><span data-stu-id="061f9-125">4</span></span>|<span data-ttu-id="061f9-126">发送 LM 和 NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="061f9-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="061f9-127">拒绝 LM</span><span class="sxs-lookup"><span data-stu-id="061f9-127">Refuse LM</span></span>|
|<span data-ttu-id="061f9-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="061f9-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="061f9-129">5</span><span class="sxs-lookup"><span data-stu-id="061f9-129">5</span></span>|<span data-ttu-id="061f9-130">发送 LM 和 NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="061f9-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="061f9-131">拒绝 LM 和 NTLM</span><span class="sxs-lookup"><span data-stu-id="061f9-131">Refuse LM & NTLM</span></span>|





