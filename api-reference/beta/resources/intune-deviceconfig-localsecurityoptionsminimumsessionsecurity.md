---
title: localSecurityOptionsMinimumSessionSecurity 枚举类型
description: LocalSecurityOptionsMinimumSessionSecurity 的可能值
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c39f2bb6d0bab2aff09fc05bb0492e81102e1b7c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396082"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="600c3-103">localSecurityOptionsMinimumSessionSecurity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="600c3-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="600c3-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="600c3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="600c3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="600c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="600c3-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="600c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="600c3-107">LocalSecurityOptionsMinimumSessionSecurity 的可能值</span><span class="sxs-lookup"><span data-stu-id="600c3-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="600c3-108">成员</span><span class="sxs-lookup"><span data-stu-id="600c3-108">Members</span></span>
|<span data-ttu-id="600c3-109">成员</span><span class="sxs-lookup"><span data-stu-id="600c3-109">Member</span></span>|<span data-ttu-id="600c3-110">值</span><span class="sxs-lookup"><span data-stu-id="600c3-110">Value</span></span>|<span data-ttu-id="600c3-111">说明</span><span class="sxs-lookup"><span data-stu-id="600c3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="600c3-112">无</span><span class="sxs-lookup"><span data-stu-id="600c3-112">none</span></span>|<span data-ttu-id="600c3-113">0</span><span class="sxs-lookup"><span data-stu-id="600c3-113">0</span></span>|<span data-ttu-id="600c3-114">发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="600c3-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="600c3-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="600c3-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="600c3-116">1</span><span class="sxs-lookup"><span data-stu-id="600c3-116">1</span></span>|<span data-ttu-id="600c3-117">如果协商，发送 LM & NTLM 使用 NTLMv2 会话安全</span><span class="sxs-lookup"><span data-stu-id="600c3-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="600c3-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="600c3-118">require128BitEncryption</span></span>|<span data-ttu-id="600c3-119">2</span><span class="sxs-lookup"><span data-stu-id="600c3-119">2</span></span>|<span data-ttu-id="600c3-120">发送 LM & 仅 NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="600c3-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="600c3-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="600c3-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="600c3-122">3</span><span class="sxs-lookup"><span data-stu-id="600c3-122">3</span></span>|<span data-ttu-id="600c3-123">发送 LM & 仅 NTLMv2 响应</span><span class="sxs-lookup"><span data-stu-id="600c3-123">Send LM & NTLMv2 responses only</span></span>|




