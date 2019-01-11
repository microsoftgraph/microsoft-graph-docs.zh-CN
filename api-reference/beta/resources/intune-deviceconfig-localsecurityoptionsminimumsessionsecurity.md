---
title: localSecurityOptionsMinimumSessionSecurity 枚举类型
description: LocalSecurityOptionsMinimumSessionSecurity 的可能值
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fb6912e7d3bba42364849165cceb28050ddacfae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833234"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="3cdc0-103">localSecurityOptionsMinimumSessionSecurity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3cdc0-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="3cdc0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3cdc0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3cdc0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3cdc0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3cdc0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3cdc0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3cdc0-107">LocalSecurityOptionsMinimumSessionSecurity 的可能值</span><span class="sxs-lookup"><span data-stu-id="3cdc0-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>
## <a name="members"></a><span data-ttu-id="3cdc0-108">成员</span><span class="sxs-lookup"><span data-stu-id="3cdc0-108">Members</span></span>
|<span data-ttu-id="3cdc0-109">成员</span><span class="sxs-lookup"><span data-stu-id="3cdc0-109">Member</span></span>|<span data-ttu-id="3cdc0-110">值</span><span class="sxs-lookup"><span data-stu-id="3cdc0-110">Value</span></span>|<span data-ttu-id="3cdc0-111">Description</span><span class="sxs-lookup"><span data-stu-id="3cdc0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cdc0-112">无</span><span class="sxs-lookup"><span data-stu-id="3cdc0-112">none</span></span>|<span data-ttu-id="3cdc0-113">0</span><span class="sxs-lookup"><span data-stu-id="3cdc0-113">0</span></span>|<span data-ttu-id="3cdc0-114">发送 LM 和 NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="3cdc0-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="3cdc0-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="3cdc0-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="3cdc0-116">1</span><span class="sxs-lookup"><span data-stu-id="3cdc0-116">1</span></span>|<span data-ttu-id="3cdc0-117">如果协商，发送 LM 和 NTLM 使用 NTLMv2 会话安全</span><span class="sxs-lookup"><span data-stu-id="3cdc0-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="3cdc0-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="3cdc0-118">require128BitEncryption</span></span>|<span data-ttu-id="3cdc0-119">2</span><span class="sxs-lookup"><span data-stu-id="3cdc0-119">2</span></span>|<span data-ttu-id="3cdc0-120">发送 LM 和 NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="3cdc0-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="3cdc0-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="3cdc0-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="3cdc0-122">3</span><span class="sxs-lookup"><span data-stu-id="3cdc0-122">3</span></span>|<span data-ttu-id="3cdc0-123">发送 LM 和 NTLMv2 响应</span><span class="sxs-lookup"><span data-stu-id="3cdc0-123">Send LM & NTLMv2 responses only</span></span>|





