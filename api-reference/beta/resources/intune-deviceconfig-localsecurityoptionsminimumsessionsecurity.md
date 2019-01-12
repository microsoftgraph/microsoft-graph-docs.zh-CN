---
title: localSecurityOptionsMinimumSessionSecurity 枚举类型
description: LocalSecurityOptionsMinimumSessionSecurity 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 822c996d788fd5edb5c92f876c725b771b051c15
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952480"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="f5bc9-103">localSecurityOptionsMinimumSessionSecurity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f5bc9-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="f5bc9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f5bc9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5bc9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f5bc9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5bc9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f5bc9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5bc9-107">LocalSecurityOptionsMinimumSessionSecurity 的可能值</span><span class="sxs-lookup"><span data-stu-id="f5bc9-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>
## <a name="members"></a><span data-ttu-id="f5bc9-108">成员</span><span class="sxs-lookup"><span data-stu-id="f5bc9-108">Members</span></span>
|<span data-ttu-id="f5bc9-109">成员</span><span class="sxs-lookup"><span data-stu-id="f5bc9-109">Member</span></span>|<span data-ttu-id="f5bc9-110">值</span><span class="sxs-lookup"><span data-stu-id="f5bc9-110">Value</span></span>|<span data-ttu-id="f5bc9-111">Description</span><span class="sxs-lookup"><span data-stu-id="f5bc9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5bc9-112">无</span><span class="sxs-lookup"><span data-stu-id="f5bc9-112">none</span></span>|<span data-ttu-id="f5bc9-113">0</span><span class="sxs-lookup"><span data-stu-id="f5bc9-113">0</span></span>|<span data-ttu-id="f5bc9-114">发送 LM 和 NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="f5bc9-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="f5bc9-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="f5bc9-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="f5bc9-116">1</span><span class="sxs-lookup"><span data-stu-id="f5bc9-116">1</span></span>|<span data-ttu-id="f5bc9-117">如果协商，发送 LM 和 NTLM 使用 NTLMv2 会话安全</span><span class="sxs-lookup"><span data-stu-id="f5bc9-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="f5bc9-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="f5bc9-118">require128BitEncryption</span></span>|<span data-ttu-id="f5bc9-119">2</span><span class="sxs-lookup"><span data-stu-id="f5bc9-119">2</span></span>|<span data-ttu-id="f5bc9-120">发送 LM 和 NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="f5bc9-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="f5bc9-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="f5bc9-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="f5bc9-122">3</span><span class="sxs-lookup"><span data-stu-id="f5bc9-122">3</span></span>|<span data-ttu-id="f5bc9-123">发送 LM 和 NTLMv2 响应</span><span class="sxs-lookup"><span data-stu-id="f5bc9-123">Send LM & NTLMv2 responses only</span></span>|





