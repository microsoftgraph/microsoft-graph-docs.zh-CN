---
title: lanManagerAuthenticationLevel 枚举类型
description: LanManagerAuthenticationLevel 的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 670cb0bec6915b79102eae227a261f26eb052413
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790375"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="c7724-103">lanManagerAuthenticationLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c7724-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="c7724-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c7724-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7724-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7724-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7724-106">LanManagerAuthenticationLevel 的可能值</span><span class="sxs-lookup"><span data-stu-id="c7724-106">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="c7724-107">成员</span><span class="sxs-lookup"><span data-stu-id="c7724-107">Members</span></span>
|<span data-ttu-id="c7724-108">成员</span><span class="sxs-lookup"><span data-stu-id="c7724-108">Member</span></span>|<span data-ttu-id="c7724-109">值</span><span class="sxs-lookup"><span data-stu-id="c7724-109">Value</span></span>|<span data-ttu-id="c7724-110">说明</span><span class="sxs-lookup"><span data-stu-id="c7724-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7724-111">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="c7724-111">lmAndNltm</span></span>|<span data-ttu-id="c7724-112">0</span><span class="sxs-lookup"><span data-stu-id="c7724-112">0</span></span>|<span data-ttu-id="c7724-113">发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="c7724-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="c7724-114">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="c7724-114">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="c7724-115">1</span><span class="sxs-lookup"><span data-stu-id="c7724-115">1</span></span>|<span data-ttu-id="c7724-116">发送 LM & NTLM-如果协商，则使用 NTLMv2 会话安全性</span><span class="sxs-lookup"><span data-stu-id="c7724-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="c7724-117">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="c7724-117">lmAndNtlmOnly</span></span>|<span data-ttu-id="c7724-118">双面</span><span class="sxs-lookup"><span data-stu-id="c7724-118">2</span></span>|<span data-ttu-id="c7724-119">仅发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="c7724-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="c7724-120">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="c7724-120">lmAndNtlmV2</span></span>|<span data-ttu-id="c7724-121">第三章</span><span class="sxs-lookup"><span data-stu-id="c7724-121">3</span></span>|<span data-ttu-id="c7724-122">仅发送 LM & NTLMv2 响应</span><span class="sxs-lookup"><span data-stu-id="c7724-122">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="c7724-123">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="c7724-123">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="c7724-124">4 </span><span class="sxs-lookup"><span data-stu-id="c7724-124">4</span></span>|<span data-ttu-id="c7724-125">仅发送 LM & NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="c7724-125">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="c7724-126">拒绝 LM</span><span class="sxs-lookup"><span data-stu-id="c7724-126">Refuse LM</span></span>|
|<span data-ttu-id="c7724-127">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="c7724-127">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="c7724-128">5 </span><span class="sxs-lookup"><span data-stu-id="c7724-128">5</span></span>|<span data-ttu-id="c7724-129">仅发送 LM & NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="c7724-129">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="c7724-130">拒绝 LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="c7724-130">Refuse LM & NTLM</span></span>|



