---
title: localSecurityOptionsMinimumSessionSecurity 枚举类型
description: LocalSecurityOptionsMinimumSessionSecurity 的可能值
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f5d7e052d5b814bb10d3c0851683deccdf9f9f5f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439971"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="ed5bf-103">localSecurityOptionsMinimumSessionSecurity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ed5bf-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

<span data-ttu-id="ed5bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed5bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed5bf-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ed5bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed5bf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ed5bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed5bf-107">LocalSecurityOptionsMinimumSessionSecurity 的可能值</span><span class="sxs-lookup"><span data-stu-id="ed5bf-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="ed5bf-108">成员</span><span class="sxs-lookup"><span data-stu-id="ed5bf-108">Members</span></span>
|<span data-ttu-id="ed5bf-109">成员</span><span class="sxs-lookup"><span data-stu-id="ed5bf-109">Member</span></span>|<span data-ttu-id="ed5bf-110">值</span><span class="sxs-lookup"><span data-stu-id="ed5bf-110">Value</span></span>|<span data-ttu-id="ed5bf-111">说明</span><span class="sxs-lookup"><span data-stu-id="ed5bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed5bf-112">无</span><span class="sxs-lookup"><span data-stu-id="ed5bf-112">none</span></span>|<span data-ttu-id="ed5bf-113">0</span><span class="sxs-lookup"><span data-stu-id="ed5bf-113">0</span></span>|<span data-ttu-id="ed5bf-114">发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="ed5bf-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="ed5bf-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="ed5bf-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="ed5bf-116">1</span><span class="sxs-lookup"><span data-stu-id="ed5bf-116">1</span></span>|<span data-ttu-id="ed5bf-117">发送 LM & NTLM-如果协商，则使用 NTLMv2 会话安全性</span><span class="sxs-lookup"><span data-stu-id="ed5bf-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="ed5bf-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="ed5bf-118">require128BitEncryption</span></span>|<span data-ttu-id="ed5bf-119">双面</span><span class="sxs-lookup"><span data-stu-id="ed5bf-119">2</span></span>|<span data-ttu-id="ed5bf-120">仅发送 LM & NTLM 响应</span><span class="sxs-lookup"><span data-stu-id="ed5bf-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="ed5bf-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="ed5bf-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="ed5bf-122">第三章</span><span class="sxs-lookup"><span data-stu-id="ed5bf-122">3</span></span>|<span data-ttu-id="ed5bf-123">仅发送 LM & NTLMv2 响应</span><span class="sxs-lookup"><span data-stu-id="ed5bf-123">Send LM & NTLMv2 responses only</span></span>|



