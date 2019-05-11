---
title: localSecurityOptionsMinimumSessionSecurity 枚举类型
description: LocalSecurityOptionsMinimumSessionSecurity 的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7ab015e80b276870e663d47a3b8b18d17fed82a4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946166"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="25a87-103">localSecurityOptionsMinimumSessionSecurity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="25a87-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="25a87-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="25a87-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25a87-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="25a87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25a87-106">LocalSecurityOptionsMinimumSessionSecurity 的可能值</span><span class="sxs-lookup"><span data-stu-id="25a87-106">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="25a87-107">成员</span><span class="sxs-lookup"><span data-stu-id="25a87-107">Members</span></span>
|<span data-ttu-id="25a87-108">成员</span><span class="sxs-lookup"><span data-stu-id="25a87-108">Member</span></span>|<span data-ttu-id="25a87-109">值</span><span class="sxs-lookup"><span data-stu-id="25a87-109">Value</span></span>|<span data-ttu-id="25a87-110">说明</span><span class="sxs-lookup"><span data-stu-id="25a87-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25a87-111">无</span><span class="sxs-lookup"><span data-stu-id="25a87-111">none</span></span>|<span data-ttu-id="25a87-112">0</span><span class="sxs-lookup"><span data-stu-id="25a87-112">0</span></span>|<span data-ttu-id="25a87-113">发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="25a87-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="25a87-114">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="25a87-114">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="25a87-115">1</span><span class="sxs-lookup"><span data-stu-id="25a87-115">1</span></span>|<span data-ttu-id="25a87-116">发送 LM & NTLM-使用 NTLMv2 会话安全性 (如果协商)</span><span class="sxs-lookup"><span data-stu-id="25a87-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="25a87-117">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="25a87-117">require128BitEncryption</span></span>|<span data-ttu-id="25a87-118">双面</span><span class="sxs-lookup"><span data-stu-id="25a87-118">2</span></span>|<span data-ttu-id="25a87-119">仅发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="25a87-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="25a87-120">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="25a87-120">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="25a87-121">第三章</span><span class="sxs-lookup"><span data-stu-id="25a87-121">3</span></span>|<span data-ttu-id="25a87-122">仅发送 LM & NTLMv2 响应</span><span class="sxs-lookup"><span data-stu-id="25a87-122">Send LM & NTLMv2 responses only</span></span>|




