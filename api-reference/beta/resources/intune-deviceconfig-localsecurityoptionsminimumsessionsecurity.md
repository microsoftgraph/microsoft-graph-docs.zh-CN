---
title: localSecurityOptionsMinimumSessionSecurity 枚举类型
description: LocalSecurityOptionsMinimumSessionSecurity 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe6007747aed1037a4dc3d5264bb432182a28c00
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145344"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="c7858-103">localSecurityOptionsMinimumSessionSecurity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c7858-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="c7858-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c7858-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7858-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7858-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7858-106">LocalSecurityOptionsMinimumSessionSecurity 的可能值</span><span class="sxs-lookup"><span data-stu-id="c7858-106">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="c7858-107">成员</span><span class="sxs-lookup"><span data-stu-id="c7858-107">Members</span></span>
|<span data-ttu-id="c7858-108">成员</span><span class="sxs-lookup"><span data-stu-id="c7858-108">Member</span></span>|<span data-ttu-id="c7858-109">值</span><span class="sxs-lookup"><span data-stu-id="c7858-109">Value</span></span>|<span data-ttu-id="c7858-110">说明</span><span class="sxs-lookup"><span data-stu-id="c7858-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7858-111">无</span><span class="sxs-lookup"><span data-stu-id="c7858-111">none</span></span>|<span data-ttu-id="c7858-112">0</span><span class="sxs-lookup"><span data-stu-id="c7858-112">0</span></span>|<span data-ttu-id="c7858-113">发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="c7858-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="c7858-114">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="c7858-114">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="c7858-115">1</span><span class="sxs-lookup"><span data-stu-id="c7858-115">1</span></span>|<span data-ttu-id="c7858-116">发送 LM & NTLM-使用 NTLMv2 会话安全性 (如果协商)</span><span class="sxs-lookup"><span data-stu-id="c7858-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="c7858-117">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="c7858-117">require128BitEncryption</span></span>|<span data-ttu-id="c7858-118">双面</span><span class="sxs-lookup"><span data-stu-id="c7858-118">2</span></span>|<span data-ttu-id="c7858-119">仅发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="c7858-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="c7858-120">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="c7858-120">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="c7858-121">第三章</span><span class="sxs-lookup"><span data-stu-id="c7858-121">3</span></span>|<span data-ttu-id="c7858-122">仅发送 LM & NTLMv2 响应</span><span class="sxs-lookup"><span data-stu-id="c7858-122">Send LM & NTLMv2 responses only</span></span>|




