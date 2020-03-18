---
title: localSecurityOptionsMinimumSessionSecurity 枚举类型
description: LocalSecurityOptionsMinimumSessionSecurity 的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: da31ca3cecc74e1c74270bd34bdad14df35cc1b1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790340"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="5dd53-103">localSecurityOptionsMinimumSessionSecurity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5dd53-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="5dd53-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5dd53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5dd53-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5dd53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5dd53-106">LocalSecurityOptionsMinimumSessionSecurity 的可能值</span><span class="sxs-lookup"><span data-stu-id="5dd53-106">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="5dd53-107">成员</span><span class="sxs-lookup"><span data-stu-id="5dd53-107">Members</span></span>
|<span data-ttu-id="5dd53-108">成员</span><span class="sxs-lookup"><span data-stu-id="5dd53-108">Member</span></span>|<span data-ttu-id="5dd53-109">值</span><span class="sxs-lookup"><span data-stu-id="5dd53-109">Value</span></span>|<span data-ttu-id="5dd53-110">说明</span><span class="sxs-lookup"><span data-stu-id="5dd53-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dd53-111">无</span><span class="sxs-lookup"><span data-stu-id="5dd53-111">none</span></span>|<span data-ttu-id="5dd53-112">0</span><span class="sxs-lookup"><span data-stu-id="5dd53-112">0</span></span>|<span data-ttu-id="5dd53-113">发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="5dd53-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="5dd53-114">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="5dd53-114">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="5dd53-115">1</span><span class="sxs-lookup"><span data-stu-id="5dd53-115">1</span></span>|<span data-ttu-id="5dd53-116">发送 LM & NTLM-如果协商，则使用 NTLMv2 会话安全性</span><span class="sxs-lookup"><span data-stu-id="5dd53-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="5dd53-117">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="5dd53-117">require128BitEncryption</span></span>|<span data-ttu-id="5dd53-118">双面</span><span class="sxs-lookup"><span data-stu-id="5dd53-118">2</span></span>|<span data-ttu-id="5dd53-119">仅发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="5dd53-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="5dd53-120">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="5dd53-120">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="5dd53-121">第三章</span><span class="sxs-lookup"><span data-stu-id="5dd53-121">3</span></span>|<span data-ttu-id="5dd53-122">仅发送 LM & NTLMv2 响应</span><span class="sxs-lookup"><span data-stu-id="5dd53-122">Send LM & NTLMv2 responses only</span></span>|



