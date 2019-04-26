---
title: nonEapAuthenticationMethodForEapTtlsType 枚举类型
description: 用于身份验证的非 EAP 方法。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a69ea80f23b2671dfd58fee87573d6e2614b360
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554413"
---
# <a name="noneapauthenticationmethodforeapttlstype-enum-type"></a><span data-ttu-id="ee302-103">nonEapAuthenticationMethodForEapTtlsType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ee302-103">nonEapAuthenticationMethodForEapTtlsType enum type</span></span>

> <span data-ttu-id="ee302-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ee302-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee302-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ee302-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee302-106">用于身份验证的非 EAP 方法。</span><span class="sxs-lookup"><span data-stu-id="ee302-106">Non-EAP methods for authentication.</span></span>

## <a name="members"></a><span data-ttu-id="ee302-107">成员</span><span class="sxs-lookup"><span data-stu-id="ee302-107">Members</span></span>
|<span data-ttu-id="ee302-108">成员</span><span class="sxs-lookup"><span data-stu-id="ee302-108">Member</span></span>|<span data-ttu-id="ee302-109">值</span><span class="sxs-lookup"><span data-stu-id="ee302-109">Value</span></span>|<span data-ttu-id="ee302-110">说明</span><span class="sxs-lookup"><span data-stu-id="ee302-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee302-111">unencryptedPassword</span><span class="sxs-lookup"><span data-stu-id="ee302-111">unencryptedPassword</span></span>|<span data-ttu-id="ee302-112">0</span><span class="sxs-lookup"><span data-stu-id="ee302-112">0</span></span>|<span data-ttu-id="ee302-113">未加密的密码 (PAP)。</span><span class="sxs-lookup"><span data-stu-id="ee302-113">Unencrypted password (PAP).</span></span>|
|<span data-ttu-id="ee302-114">challengeHandshakeAuthenticationProtocol</span><span class="sxs-lookup"><span data-stu-id="ee302-114">challengeHandshakeAuthenticationProtocol</span></span>|<span data-ttu-id="ee302-115">1</span><span class="sxs-lookup"><span data-stu-id="ee302-115">1</span></span>|<span data-ttu-id="ee302-116">质询握手身份验证协议 (CHAP)。</span><span class="sxs-lookup"><span data-stu-id="ee302-116">Challenge Handshake Authentication Protocol (CHAP).</span></span>|
|<span data-ttu-id="ee302-117">microsoftChap</span><span class="sxs-lookup"><span data-stu-id="ee302-117">microsoftChap</span></span>|<span data-ttu-id="ee302-118">2 </span><span class="sxs-lookup"><span data-stu-id="ee302-118">2</span></span>| <span data-ttu-id="ee302-119">Microsoft chap (毫秒-chap)。</span><span class="sxs-lookup"><span data-stu-id="ee302-119">Microsoft CHAP (MS-CHAP).</span></span>|
|<span data-ttu-id="ee302-120">microsoftChapVersionTwo</span><span class="sxs-lookup"><span data-stu-id="ee302-120">microsoftChapVersionTwo</span></span>|<span data-ttu-id="ee302-121">3 </span><span class="sxs-lookup"><span data-stu-id="ee302-121">3</span></span>|<span data-ttu-id="ee302-122">Microsoft CHAP 版本 2 (毫秒-CHAP v2)。</span><span class="sxs-lookup"><span data-stu-id="ee302-122">Microsoft CHAP Version 2 (MS-CHAP v2).</span></span>|





