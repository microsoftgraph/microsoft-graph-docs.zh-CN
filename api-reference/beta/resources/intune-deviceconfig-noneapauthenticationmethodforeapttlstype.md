---
title: nonEapAuthenticationMethodForEapTtlsType 枚举类型
description: 身份验证的非 EAP 方法。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2f14c98118541e6eeb6cb48fd54ac3fb69a722b0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425594"
---
# <a name="noneapauthenticationmethodforeapttlstype-enum-type"></a><span data-ttu-id="b49b5-103">nonEapAuthenticationMethodForEapTtlsType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b49b5-103">nonEapAuthenticationMethodForEapTtlsType enum type</span></span>

> <span data-ttu-id="b49b5-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b49b5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b49b5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b49b5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b49b5-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b49b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b49b5-107">身份验证的非 EAP 方法。</span><span class="sxs-lookup"><span data-stu-id="b49b5-107">Non-EAP methods for authentication.</span></span>

## <a name="members"></a><span data-ttu-id="b49b5-108">成员</span><span class="sxs-lookup"><span data-stu-id="b49b5-108">Members</span></span>
|<span data-ttu-id="b49b5-109">成员</span><span class="sxs-lookup"><span data-stu-id="b49b5-109">Member</span></span>|<span data-ttu-id="b49b5-110">值</span><span class="sxs-lookup"><span data-stu-id="b49b5-110">Value</span></span>|<span data-ttu-id="b49b5-111">说明</span><span class="sxs-lookup"><span data-stu-id="b49b5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b49b5-112">unencryptedPassword</span><span class="sxs-lookup"><span data-stu-id="b49b5-112">unencryptedPassword</span></span>|<span data-ttu-id="b49b5-113">0</span><span class="sxs-lookup"><span data-stu-id="b49b5-113">0</span></span>|<span data-ttu-id="b49b5-114">未加密的密码 (PAP)。</span><span class="sxs-lookup"><span data-stu-id="b49b5-114">Unencrypted password (PAP).</span></span>|
|<span data-ttu-id="b49b5-115">challengeHandshakeAuthenticationProtocol</span><span class="sxs-lookup"><span data-stu-id="b49b5-115">challengeHandshakeAuthenticationProtocol</span></span>|<span data-ttu-id="b49b5-116">1</span><span class="sxs-lookup"><span data-stu-id="b49b5-116">1</span></span>|<span data-ttu-id="b49b5-117">质询握手身份验证协议 (CHAP)。</span><span class="sxs-lookup"><span data-stu-id="b49b5-117">Challenge Handshake Authentication Protocol (CHAP).</span></span>|
|<span data-ttu-id="b49b5-118">microsoftChap</span><span class="sxs-lookup"><span data-stu-id="b49b5-118">microsoftChap</span></span>|<span data-ttu-id="b49b5-119">2</span><span class="sxs-lookup"><span data-stu-id="b49b5-119">2</span></span>| <span data-ttu-id="b49b5-120">Microsoft CHAP (MS-CHAP)。</span><span class="sxs-lookup"><span data-stu-id="b49b5-120">Microsoft CHAP (MS-CHAP).</span></span>|
|<span data-ttu-id="b49b5-121">microsoftChapVersionTwo</span><span class="sxs-lookup"><span data-stu-id="b49b5-121">microsoftChapVersionTwo</span></span>|<span data-ttu-id="b49b5-122">3</span><span class="sxs-lookup"><span data-stu-id="b49b5-122">3</span></span>|<span data-ttu-id="b49b5-123">Microsoft CHAP 版本 2 (MS-CHAP v2)。</span><span class="sxs-lookup"><span data-stu-id="b49b5-123">Microsoft CHAP Version 2 (MS-CHAP v2).</span></span>|




