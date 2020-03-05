---
title: lanManagerAuthenticationLevel 枚举类型
description: LanManagerAuthenticationLevel 的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8b979c66469ac29339045dd9d1341f85839084bf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529763"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="c4085-103">lanManagerAuthenticationLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c4085-103">lanManagerAuthenticationLevel enum type</span></span>

<span data-ttu-id="c4085-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c4085-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4085-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c4085-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4085-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c4085-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4085-107">LanManagerAuthenticationLevel 的可能值</span><span class="sxs-lookup"><span data-stu-id="c4085-107">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="c4085-108">成员</span><span class="sxs-lookup"><span data-stu-id="c4085-108">Members</span></span>
|<span data-ttu-id="c4085-109">成员</span><span class="sxs-lookup"><span data-stu-id="c4085-109">Member</span></span>|<span data-ttu-id="c4085-110">值</span><span class="sxs-lookup"><span data-stu-id="c4085-110">Value</span></span>|<span data-ttu-id="c4085-111">说明</span><span class="sxs-lookup"><span data-stu-id="c4085-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4085-112">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="c4085-112">lmAndNltm</span></span>|<span data-ttu-id="c4085-113">0</span><span class="sxs-lookup"><span data-stu-id="c4085-113">0</span></span>|<span data-ttu-id="c4085-114">发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="c4085-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="c4085-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="c4085-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="c4085-116">1 </span><span class="sxs-lookup"><span data-stu-id="c4085-116">1</span></span>|<span data-ttu-id="c4085-117">发送 LM & NTLM-如果协商，则使用 NTLMv2 会话安全性</span><span class="sxs-lookup"><span data-stu-id="c4085-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="c4085-118">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="c4085-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="c4085-119">2 </span><span class="sxs-lookup"><span data-stu-id="c4085-119">2</span></span>|<span data-ttu-id="c4085-120">仅发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="c4085-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="c4085-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="c4085-121">lmAndNtlmV2</span></span>|<span data-ttu-id="c4085-122">3 </span><span class="sxs-lookup"><span data-stu-id="c4085-122">3</span></span>|<span data-ttu-id="c4085-123">仅发送 LM & NTLMv2 响应</span><span class="sxs-lookup"><span data-stu-id="c4085-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="c4085-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="c4085-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="c4085-125">4 </span><span class="sxs-lookup"><span data-stu-id="c4085-125">4</span></span>|<span data-ttu-id="c4085-126">仅发送 LM & NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="c4085-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="c4085-127">拒绝 LM</span><span class="sxs-lookup"><span data-stu-id="c4085-127">Refuse LM</span></span>|
|<span data-ttu-id="c4085-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="c4085-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="c4085-129">5 </span><span class="sxs-lookup"><span data-stu-id="c4085-129">5</span></span>|<span data-ttu-id="c4085-130">仅发送 LM & NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="c4085-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="c4085-131">拒绝 LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="c4085-131">Refuse LM & NTLM</span></span>|



