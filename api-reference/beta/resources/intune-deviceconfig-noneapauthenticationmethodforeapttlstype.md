---
title: nonEapAuthenticationMethodForEapTtlsType 枚举类型
description: 身份验证的非 EAP 方法。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 27673d4245f9bea1ef24c25034497b4d5bf7aebd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884180"
---
# <a name="noneapauthenticationmethodforeapttlstype-enum-type"></a><span data-ttu-id="b0b43-103">nonEapAuthenticationMethodForEapTtlsType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b0b43-103">nonEapAuthenticationMethodForEapTtlsType enum type</span></span>

> <span data-ttu-id="b0b43-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b0b43-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0b43-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b0b43-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0b43-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b0b43-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0b43-107">身份验证的非 EAP 方法。</span><span class="sxs-lookup"><span data-stu-id="b0b43-107">Non-EAP methods for authentication.</span></span>
## <a name="members"></a><span data-ttu-id="b0b43-108">成员</span><span class="sxs-lookup"><span data-stu-id="b0b43-108">Members</span></span>
|<span data-ttu-id="b0b43-109">成员</span><span class="sxs-lookup"><span data-stu-id="b0b43-109">Member</span></span>|<span data-ttu-id="b0b43-110">值</span><span class="sxs-lookup"><span data-stu-id="b0b43-110">Value</span></span>|<span data-ttu-id="b0b43-111">Description</span><span class="sxs-lookup"><span data-stu-id="b0b43-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0b43-112">unencryptedPassword</span><span class="sxs-lookup"><span data-stu-id="b0b43-112">unencryptedPassword</span></span>|<span data-ttu-id="b0b43-113">0</span><span class="sxs-lookup"><span data-stu-id="b0b43-113">0</span></span>|<span data-ttu-id="b0b43-114">未加密的密码 (PAP)。</span><span class="sxs-lookup"><span data-stu-id="b0b43-114">Unencrypted password (PAP).</span></span>|
|<span data-ttu-id="b0b43-115">challengeHandshakeAuthenticationProtocol</span><span class="sxs-lookup"><span data-stu-id="b0b43-115">challengeHandshakeAuthenticationProtocol</span></span>|<span data-ttu-id="b0b43-116">1</span><span class="sxs-lookup"><span data-stu-id="b0b43-116">1</span></span>|<span data-ttu-id="b0b43-117">质询握手身份验证协议 (CHAP)。</span><span class="sxs-lookup"><span data-stu-id="b0b43-117">Challenge Handshake Authentication Protocol (CHAP).</span></span>|
|<span data-ttu-id="b0b43-118">microsoftChap</span><span class="sxs-lookup"><span data-stu-id="b0b43-118">microsoftChap</span></span>|<span data-ttu-id="b0b43-119">2</span><span class="sxs-lookup"><span data-stu-id="b0b43-119">2</span></span>| <span data-ttu-id="b0b43-120">Microsoft CHAP (MS-CHAP)。</span><span class="sxs-lookup"><span data-stu-id="b0b43-120">Microsoft CHAP (MS-CHAP).</span></span>|
|<span data-ttu-id="b0b43-121">microsoftChapVersionTwo</span><span class="sxs-lookup"><span data-stu-id="b0b43-121">microsoftChapVersionTwo</span></span>|<span data-ttu-id="b0b43-122">3</span><span class="sxs-lookup"><span data-stu-id="b0b43-122">3</span></span>|<span data-ttu-id="b0b43-123">Microsoft CHAP 版本 2 (MS-CHAP v2)。</span><span class="sxs-lookup"><span data-stu-id="b0b43-123">Microsoft CHAP Version 2 (MS-CHAP v2).</span></span>|





