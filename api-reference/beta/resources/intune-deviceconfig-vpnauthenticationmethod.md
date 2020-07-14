---
title: vpnAuthenticationMethod 枚举类型
description: VPN 身份验证方法。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ef477b17b8ae7e8aedc3b95ce70b66115a3c8712
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123888"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="25e45-103">vpnAuthenticationMethod 枚举类型</span><span class="sxs-lookup"><span data-stu-id="25e45-103">vpnAuthenticationMethod enum type</span></span>

<span data-ttu-id="25e45-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25e45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25e45-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="25e45-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25e45-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="25e45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25e45-107">VPN 身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="25e45-107">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="25e45-108">成员</span><span class="sxs-lookup"><span data-stu-id="25e45-108">Members</span></span>
|<span data-ttu-id="25e45-109">成员</span><span class="sxs-lookup"><span data-stu-id="25e45-109">Member</span></span>|<span data-ttu-id="25e45-110">值</span><span class="sxs-lookup"><span data-stu-id="25e45-110">Value</span></span>|<span data-ttu-id="25e45-111">说明</span><span class="sxs-lookup"><span data-stu-id="25e45-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25e45-112">证书</span><span class="sxs-lookup"><span data-stu-id="25e45-112">certificate</span></span>|<span data-ttu-id="25e45-113">0</span><span class="sxs-lookup"><span data-stu-id="25e45-113">0</span></span>|<span data-ttu-id="25e45-114">使用证书进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="25e45-114">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="25e45-115">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="25e45-115">usernameAndPassword</span></span>|<span data-ttu-id="25e45-116">1 </span><span class="sxs-lookup"><span data-stu-id="25e45-116">1</span></span>|<span data-ttu-id="25e45-117">使用用户名和密码进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="25e45-117">Use username and password for authentication.</span></span>|
|<span data-ttu-id="25e45-118">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="25e45-118">sharedSecret</span></span>|<span data-ttu-id="25e45-119">2 </span><span class="sxs-lookup"><span data-stu-id="25e45-119">2</span></span>|<span data-ttu-id="25e45-120">使用共享密钥进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="25e45-120">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="25e45-121">仅对 iOS IKEv2 有效。</span><span class="sxs-lookup"><span data-stu-id="25e45-121">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="25e45-122">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="25e45-122">derivedCredential</span></span>|<span data-ttu-id="25e45-123">3 </span><span class="sxs-lookup"><span data-stu-id="25e45-123">3</span></span>|<span data-ttu-id="25e45-124">使用派生的凭据进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="25e45-124">Use Derived Credential for Authentication.</span></span>|
|<span data-ttu-id="25e45-125">azureAD</span><span class="sxs-lookup"><span data-stu-id="25e45-125">azureAD</span></span>|<span data-ttu-id="25e45-126">4 </span><span class="sxs-lookup"><span data-stu-id="25e45-126">4</span></span>|<span data-ttu-id="25e45-127">使用 Azure AD 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="25e45-127">Use Azure AD for authentication.</span></span>|



