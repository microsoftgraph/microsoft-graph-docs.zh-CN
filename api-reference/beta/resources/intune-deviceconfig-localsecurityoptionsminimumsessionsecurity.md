---
title: localSecurityOptionsMinimumSessionSecurity 枚举类型
description: LocalSecurityOptionsMinimumSessionSecurity 的可能值
ms.openlocfilehash: 969c7d6576c613f5214bfc3b8a5a1ad36722f0df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047330"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="71126-103">localSecurityOptionsMinimumSessionSecurity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="71126-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="71126-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="71126-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71126-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="71126-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71126-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="71126-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71126-107">LocalSecurityOptionsMinimumSessionSecurity 的可能值</span><span class="sxs-lookup"><span data-stu-id="71126-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>
## <a name="members"></a><span data-ttu-id="71126-108">成员</span><span class="sxs-lookup"><span data-stu-id="71126-108">Members</span></span>
|<span data-ttu-id="71126-109">成员</span><span class="sxs-lookup"><span data-stu-id="71126-109">Member</span></span>|<span data-ttu-id="71126-110">值</span><span class="sxs-lookup"><span data-stu-id="71126-110">Value</span></span>|<span data-ttu-id="71126-111">说明</span><span class="sxs-lookup"><span data-stu-id="71126-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71126-112">无</span><span class="sxs-lookup"><span data-stu-id="71126-112">none</span></span>|<span data-ttu-id="71126-113">0</span><span class="sxs-lookup"><span data-stu-id="71126-113">0</span></span>|<span data-ttu-id="71126-114">发送 LM 和 NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="71126-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="71126-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="71126-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="71126-116">1</span><span class="sxs-lookup"><span data-stu-id="71126-116">1</span></span>|<span data-ttu-id="71126-117">如果协商，发送 LM 和 NTLM 使用 NTLMv2 会话安全</span><span class="sxs-lookup"><span data-stu-id="71126-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="71126-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="71126-118">require128BitEncryption</span></span>|<span data-ttu-id="71126-119">2</span><span class="sxs-lookup"><span data-stu-id="71126-119">2</span></span>|<span data-ttu-id="71126-120">发送 LM 和 NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="71126-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="71126-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="71126-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="71126-122">3</span><span class="sxs-lookup"><span data-stu-id="71126-122">3</span></span>|<span data-ttu-id="71126-123">发送 LM 和 NTLMv2 响应</span><span class="sxs-lookup"><span data-stu-id="71126-123">Send LM & NTLMv2 responses only</span></span>|





