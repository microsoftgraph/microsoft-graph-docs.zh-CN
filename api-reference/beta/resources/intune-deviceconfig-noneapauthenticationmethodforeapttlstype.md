---
title: nonEapAuthenticationMethodForEapTtlsType 枚举类型
description: 用于身份验证的非 EAP 方法。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 08c8240f28b015939a10a41bfd437c8f62fd4003
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958814"
---
# <a name="noneapauthenticationmethodforeapttlstype-enum-type"></a><span data-ttu-id="98815-103">nonEapAuthenticationMethodForEapTtlsType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="98815-103">nonEapAuthenticationMethodForEapTtlsType enum type</span></span>

> <span data-ttu-id="98815-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="98815-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98815-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="98815-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98815-106">用于身份验证的非 EAP 方法。</span><span class="sxs-lookup"><span data-stu-id="98815-106">Non-EAP methods for authentication.</span></span>

## <a name="members"></a><span data-ttu-id="98815-107">成员</span><span class="sxs-lookup"><span data-stu-id="98815-107">Members</span></span>
|<span data-ttu-id="98815-108">成员</span><span class="sxs-lookup"><span data-stu-id="98815-108">Member</span></span>|<span data-ttu-id="98815-109">值</span><span class="sxs-lookup"><span data-stu-id="98815-109">Value</span></span>|<span data-ttu-id="98815-110">说明</span><span class="sxs-lookup"><span data-stu-id="98815-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98815-111">unencryptedPassword</span><span class="sxs-lookup"><span data-stu-id="98815-111">unencryptedPassword</span></span>|<span data-ttu-id="98815-112">0</span><span class="sxs-lookup"><span data-stu-id="98815-112">0</span></span>|<span data-ttu-id="98815-113">未加密的密码 (PAP)。</span><span class="sxs-lookup"><span data-stu-id="98815-113">Unencrypted password (PAP).</span></span>|
|<span data-ttu-id="98815-114">challengeHandshakeAuthenticationProtocol</span><span class="sxs-lookup"><span data-stu-id="98815-114">challengeHandshakeAuthenticationProtocol</span></span>|<span data-ttu-id="98815-115">1</span><span class="sxs-lookup"><span data-stu-id="98815-115">1</span></span>|<span data-ttu-id="98815-116">质询握手身份验证协议 (CHAP)。</span><span class="sxs-lookup"><span data-stu-id="98815-116">Challenge Handshake Authentication Protocol (CHAP).</span></span>|
|<span data-ttu-id="98815-117">microsoftChap</span><span class="sxs-lookup"><span data-stu-id="98815-117">microsoftChap</span></span>|<span data-ttu-id="98815-118">双面</span><span class="sxs-lookup"><span data-stu-id="98815-118">2</span></span>| <span data-ttu-id="98815-119">Microsoft CHAP (毫秒-CHAP)。</span><span class="sxs-lookup"><span data-stu-id="98815-119">Microsoft CHAP (MS-CHAP).</span></span>|
|<span data-ttu-id="98815-120">microsoftChapVersionTwo</span><span class="sxs-lookup"><span data-stu-id="98815-120">microsoftChapVersionTwo</span></span>|<span data-ttu-id="98815-121">第三章</span><span class="sxs-lookup"><span data-stu-id="98815-121">3</span></span>|<span data-ttu-id="98815-122">Microsoft CHAP 版本 2 (毫秒-CHAP v2)。</span><span class="sxs-lookup"><span data-stu-id="98815-122">Microsoft CHAP Version 2 (MS-CHAP v2).</span></span>|





