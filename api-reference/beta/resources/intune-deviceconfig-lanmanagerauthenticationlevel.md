---
title: lanManagerAuthenticationLevel 枚举类型
description: LanManagerAuthenticationLevel 的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ade139765c9a362cd0c9f9365af0026c51ecb4ce
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356723"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="0494c-103">lanManagerAuthenticationLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0494c-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="0494c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0494c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0494c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0494c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0494c-106">LanManagerAuthenticationLevel 的可能值</span><span class="sxs-lookup"><span data-stu-id="0494c-106">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="0494c-107">成员</span><span class="sxs-lookup"><span data-stu-id="0494c-107">Members</span></span>
|<span data-ttu-id="0494c-108">成员</span><span class="sxs-lookup"><span data-stu-id="0494c-108">Member</span></span>|<span data-ttu-id="0494c-109">值</span><span class="sxs-lookup"><span data-stu-id="0494c-109">Value</span></span>|<span data-ttu-id="0494c-110">说明</span><span class="sxs-lookup"><span data-stu-id="0494c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0494c-111">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="0494c-111">lmAndNltm</span></span>|<span data-ttu-id="0494c-112">0</span><span class="sxs-lookup"><span data-stu-id="0494c-112">0</span></span>|<span data-ttu-id="0494c-113">发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="0494c-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="0494c-114">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="0494c-114">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="0494c-115">1</span><span class="sxs-lookup"><span data-stu-id="0494c-115">1</span></span>|<span data-ttu-id="0494c-116">发送 LM & NTLM-如果协商, 则使用 NTLMv2 会话安全性</span><span class="sxs-lookup"><span data-stu-id="0494c-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="0494c-117">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="0494c-117">lmAndNtlmOnly</span></span>|<span data-ttu-id="0494c-118">双面</span><span class="sxs-lookup"><span data-stu-id="0494c-118">2</span></span>|<span data-ttu-id="0494c-119">仅发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="0494c-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="0494c-120">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="0494c-120">lmAndNtlmV2</span></span>|<span data-ttu-id="0494c-121">第三章</span><span class="sxs-lookup"><span data-stu-id="0494c-121">3</span></span>|<span data-ttu-id="0494c-122">仅发送 LM & NTLMv2 响应</span><span class="sxs-lookup"><span data-stu-id="0494c-122">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="0494c-123">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="0494c-123">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="0494c-124">4</span><span class="sxs-lookup"><span data-stu-id="0494c-124">4</span></span>|<span data-ttu-id="0494c-125">仅发送 LM & NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="0494c-125">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="0494c-126">拒绝 LM</span><span class="sxs-lookup"><span data-stu-id="0494c-126">Refuse LM</span></span>|
|<span data-ttu-id="0494c-127">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="0494c-127">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="0494c-128">5</span><span class="sxs-lookup"><span data-stu-id="0494c-128">5</span></span>|<span data-ttu-id="0494c-129">仅发送 LM & NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="0494c-129">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="0494c-130">拒绝 LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="0494c-130">Refuse LM & NTLM</span></span>|



