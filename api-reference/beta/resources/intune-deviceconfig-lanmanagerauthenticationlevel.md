---
title: lanManagerAuthenticationLevel 枚举类型
description: LanManagerAuthenticationLevel 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b71f045ac937af455da428b98242f9d074b14840
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732535"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="e6b42-103">lanManagerAuthenticationLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e6b42-103">lanManagerAuthenticationLevel enum type</span></span>

<span data-ttu-id="e6b42-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6b42-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6b42-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e6b42-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6b42-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e6b42-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6b42-107">LanManagerAuthenticationLevel 的可能值</span><span class="sxs-lookup"><span data-stu-id="e6b42-107">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="e6b42-108">成员</span><span class="sxs-lookup"><span data-stu-id="e6b42-108">Members</span></span>
|<span data-ttu-id="e6b42-109">成员</span><span class="sxs-lookup"><span data-stu-id="e6b42-109">Member</span></span>|<span data-ttu-id="e6b42-110">值</span><span class="sxs-lookup"><span data-stu-id="e6b42-110">Value</span></span>|<span data-ttu-id="e6b42-111">说明</span><span class="sxs-lookup"><span data-stu-id="e6b42-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6b42-112">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="e6b42-112">lmAndNltm</span></span>|<span data-ttu-id="e6b42-113">0</span><span class="sxs-lookup"><span data-stu-id="e6b42-113">0</span></span>|<span data-ttu-id="e6b42-114">发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="e6b42-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="e6b42-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="e6b42-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="e6b42-116">1</span><span class="sxs-lookup"><span data-stu-id="e6b42-116">1</span></span>|<span data-ttu-id="e6b42-117">发送 LM & NTLM-如果协商，则使用 NTLMv2 会话安全性</span><span class="sxs-lookup"><span data-stu-id="e6b42-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="e6b42-118">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="e6b42-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="e6b42-119">双面</span><span class="sxs-lookup"><span data-stu-id="e6b42-119">2</span></span>|<span data-ttu-id="e6b42-120">仅发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="e6b42-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="e6b42-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="e6b42-121">lmAndNtlmV2</span></span>|<span data-ttu-id="e6b42-122">第三章</span><span class="sxs-lookup"><span data-stu-id="e6b42-122">3</span></span>|<span data-ttu-id="e6b42-123">仅发送 LM & NTLMv2 响应</span><span class="sxs-lookup"><span data-stu-id="e6b42-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="e6b42-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="e6b42-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="e6b42-125">4 </span><span class="sxs-lookup"><span data-stu-id="e6b42-125">4</span></span>|<span data-ttu-id="e6b42-126">仅发送 LM & NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="e6b42-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="e6b42-127">拒绝 LM</span><span class="sxs-lookup"><span data-stu-id="e6b42-127">Refuse LM</span></span>|
|<span data-ttu-id="e6b42-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="e6b42-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="e6b42-129">5 </span><span class="sxs-lookup"><span data-stu-id="e6b42-129">5</span></span>|<span data-ttu-id="e6b42-130">仅发送 LM & NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="e6b42-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="e6b42-131">拒绝 LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="e6b42-131">Refuse LM & NTLM</span></span>|





