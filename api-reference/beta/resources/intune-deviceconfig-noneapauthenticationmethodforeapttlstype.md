---
title: nonEapAuthenticationMethodForEapTtlsType 枚举类型
description: 用于身份验证的非 EAP 方法。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 262cae1f72d52ec31ee98107e5f52e36eb403962
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43402113"
---
# <a name="noneapauthenticationmethodforeapttlstype-enum-type"></a><span data-ttu-id="cdc62-103">nonEapAuthenticationMethodForEapTtlsType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cdc62-103">nonEapAuthenticationMethodForEapTtlsType enum type</span></span>

<span data-ttu-id="cdc62-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdc62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cdc62-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cdc62-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdc62-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cdc62-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdc62-107">用于身份验证的非 EAP 方法。</span><span class="sxs-lookup"><span data-stu-id="cdc62-107">Non-EAP methods for authentication.</span></span>

## <a name="members"></a><span data-ttu-id="cdc62-108">成员</span><span class="sxs-lookup"><span data-stu-id="cdc62-108">Members</span></span>
|<span data-ttu-id="cdc62-109">成员</span><span class="sxs-lookup"><span data-stu-id="cdc62-109">Member</span></span>|<span data-ttu-id="cdc62-110">值</span><span class="sxs-lookup"><span data-stu-id="cdc62-110">Value</span></span>|<span data-ttu-id="cdc62-111">说明</span><span class="sxs-lookup"><span data-stu-id="cdc62-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdc62-112">unencryptedPassword</span><span class="sxs-lookup"><span data-stu-id="cdc62-112">unencryptedPassword</span></span>|<span data-ttu-id="cdc62-113">0</span><span class="sxs-lookup"><span data-stu-id="cdc62-113">0</span></span>|<span data-ttu-id="cdc62-114">未加密的密码（PAP）。</span><span class="sxs-lookup"><span data-stu-id="cdc62-114">Unencrypted password (PAP).</span></span>|
|<span data-ttu-id="cdc62-115">challengeHandshakeAuthenticationProtocol</span><span class="sxs-lookup"><span data-stu-id="cdc62-115">challengeHandshakeAuthenticationProtocol</span></span>|<span data-ttu-id="cdc62-116">1</span><span class="sxs-lookup"><span data-stu-id="cdc62-116">1</span></span>|<span data-ttu-id="cdc62-117">质询握手身份验证协议（CHAP）。</span><span class="sxs-lookup"><span data-stu-id="cdc62-117">Challenge Handshake Authentication Protocol (CHAP).</span></span>|
|<span data-ttu-id="cdc62-118">microsoftChap</span><span class="sxs-lookup"><span data-stu-id="cdc62-118">microsoftChap</span></span>|<span data-ttu-id="cdc62-119">双面</span><span class="sxs-lookup"><span data-stu-id="cdc62-119">2</span></span>| <span data-ttu-id="cdc62-120">Microsoft CHAP （毫秒-CHAP）。</span><span class="sxs-lookup"><span data-stu-id="cdc62-120">Microsoft CHAP (MS-CHAP).</span></span>|
|<span data-ttu-id="cdc62-121">microsoftChapVersionTwo</span><span class="sxs-lookup"><span data-stu-id="cdc62-121">microsoftChapVersionTwo</span></span>|<span data-ttu-id="cdc62-122">第三章</span><span class="sxs-lookup"><span data-stu-id="cdc62-122">3</span></span>|<span data-ttu-id="cdc62-123">Microsoft CHAP 版本2（毫秒-CHAP v2）。</span><span class="sxs-lookup"><span data-stu-id="cdc62-123">Microsoft CHAP Version 2 (MS-CHAP v2).</span></span>|



