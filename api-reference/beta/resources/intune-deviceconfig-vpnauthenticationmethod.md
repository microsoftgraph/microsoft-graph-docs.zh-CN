---
title: vpnAuthenticationMethod 枚举类型
description: VPN 身份验证方法。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 58cb031abbcf520a8a970aa80bacd2390b860343
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367790"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="d772b-103">vpnAuthenticationMethod 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d772b-103">vpnAuthenticationMethod enum type</span></span>

> <span data-ttu-id="d772b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d772b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d772b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d772b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d772b-106">VPN 身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="d772b-106">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="d772b-107">成员</span><span class="sxs-lookup"><span data-stu-id="d772b-107">Members</span></span>
|<span data-ttu-id="d772b-108">成员</span><span class="sxs-lookup"><span data-stu-id="d772b-108">Member</span></span>|<span data-ttu-id="d772b-109">值</span><span class="sxs-lookup"><span data-stu-id="d772b-109">Value</span></span>|<span data-ttu-id="d772b-110">说明</span><span class="sxs-lookup"><span data-stu-id="d772b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d772b-111">证书</span><span class="sxs-lookup"><span data-stu-id="d772b-111">certificate</span></span>|<span data-ttu-id="d772b-112">0</span><span class="sxs-lookup"><span data-stu-id="d772b-112">0</span></span>|<span data-ttu-id="d772b-113">使用证书进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="d772b-113">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="d772b-114">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="d772b-114">usernameAndPassword</span></span>|<span data-ttu-id="d772b-115">1</span><span class="sxs-lookup"><span data-stu-id="d772b-115">1</span></span>|<span data-ttu-id="d772b-116">使用用户名和密码进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="d772b-116">Use username and password for authentication.</span></span>|
|<span data-ttu-id="d772b-117">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="d772b-117">sharedSecret</span></span>|<span data-ttu-id="d772b-118">双面</span><span class="sxs-lookup"><span data-stu-id="d772b-118">2</span></span>|<span data-ttu-id="d772b-119">使用共享密钥进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="d772b-119">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="d772b-120">仅对 iOS IKEv2 有效。</span><span class="sxs-lookup"><span data-stu-id="d772b-120">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="d772b-121">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="d772b-121">derivedCredential</span></span>|<span data-ttu-id="d772b-122">第三章</span><span class="sxs-lookup"><span data-stu-id="d772b-122">3</span></span>|<span data-ttu-id="d772b-123">使用派生的凭据进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="d772b-123">Use Derived Credential for Authentication.</span></span>  <span data-ttu-id="d772b-124">仅对 iOS 有效。</span><span class="sxs-lookup"><span data-stu-id="d772b-124">Only valid for iOS.</span></span>|



