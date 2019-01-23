---
title: lanManagerAuthenticationLevel 枚举类型
description: LanManagerAuthenticationLevel 的可能值
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6e8c7b3df6f515d3dad0d7619b6c0b755ad799d7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397454"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="53de2-103">lanManagerAuthenticationLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="53de2-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="53de2-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="53de2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="53de2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="53de2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53de2-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="53de2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53de2-107">LanManagerAuthenticationLevel 的可能值</span><span class="sxs-lookup"><span data-stu-id="53de2-107">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="53de2-108">成员</span><span class="sxs-lookup"><span data-stu-id="53de2-108">Members</span></span>
|<span data-ttu-id="53de2-109">成员</span><span class="sxs-lookup"><span data-stu-id="53de2-109">Member</span></span>|<span data-ttu-id="53de2-110">值</span><span class="sxs-lookup"><span data-stu-id="53de2-110">Value</span></span>|<span data-ttu-id="53de2-111">说明</span><span class="sxs-lookup"><span data-stu-id="53de2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53de2-112">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="53de2-112">lmAndNltm</span></span>|<span data-ttu-id="53de2-113">0</span><span class="sxs-lookup"><span data-stu-id="53de2-113">0</span></span>|<span data-ttu-id="53de2-114">发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="53de2-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="53de2-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="53de2-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="53de2-116">1</span><span class="sxs-lookup"><span data-stu-id="53de2-116">1</span></span>|<span data-ttu-id="53de2-117">如果协商，发送 LM & NTLM 使用 NTLMv2 会话安全</span><span class="sxs-lookup"><span data-stu-id="53de2-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="53de2-118">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="53de2-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="53de2-119">2</span><span class="sxs-lookup"><span data-stu-id="53de2-119">2</span></span>|<span data-ttu-id="53de2-120">发送 LM & 仅 NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="53de2-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="53de2-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="53de2-121">lmAndNtlmV2</span></span>|<span data-ttu-id="53de2-122">3</span><span class="sxs-lookup"><span data-stu-id="53de2-122">3</span></span>|<span data-ttu-id="53de2-123">发送 LM & 仅 NTLMv2 响应</span><span class="sxs-lookup"><span data-stu-id="53de2-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="53de2-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="53de2-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="53de2-125">4</span><span class="sxs-lookup"><span data-stu-id="53de2-125">4</span></span>|<span data-ttu-id="53de2-126">发送 LM & 仅 NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="53de2-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="53de2-127">拒绝 LM</span><span class="sxs-lookup"><span data-stu-id="53de2-127">Refuse LM</span></span>|
|<span data-ttu-id="53de2-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="53de2-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="53de2-129">5</span><span class="sxs-lookup"><span data-stu-id="53de2-129">5</span></span>|<span data-ttu-id="53de2-130">发送 LM & 仅 NTLMv2 响应。</span><span class="sxs-lookup"><span data-stu-id="53de2-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="53de2-131">拒绝 LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="53de2-131">Refuse LM & NTLM</span></span>|




