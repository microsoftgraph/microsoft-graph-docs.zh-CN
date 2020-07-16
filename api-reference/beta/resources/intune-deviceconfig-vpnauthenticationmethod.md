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
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="72a93-103">vpnAuthenticationMethod 枚举类型</span><span class="sxs-lookup"><span data-stu-id="72a93-103">vpnAuthenticationMethod enum type</span></span>

<span data-ttu-id="72a93-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72a93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72a93-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="72a93-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72a93-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="72a93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72a93-107">VPN 身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="72a93-107">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="72a93-108">成员</span><span class="sxs-lookup"><span data-stu-id="72a93-108">Members</span></span>
|<span data-ttu-id="72a93-109">成员</span><span class="sxs-lookup"><span data-stu-id="72a93-109">Member</span></span>|<span data-ttu-id="72a93-110">值</span><span class="sxs-lookup"><span data-stu-id="72a93-110">Value</span></span>|<span data-ttu-id="72a93-111">说明</span><span class="sxs-lookup"><span data-stu-id="72a93-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72a93-112">证书</span><span class="sxs-lookup"><span data-stu-id="72a93-112">certificate</span></span>|<span data-ttu-id="72a93-113">0</span><span class="sxs-lookup"><span data-stu-id="72a93-113">0</span></span>|<span data-ttu-id="72a93-114">使用证书进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="72a93-114">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="72a93-115">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="72a93-115">usernameAndPassword</span></span>|<span data-ttu-id="72a93-116">1 </span><span class="sxs-lookup"><span data-stu-id="72a93-116">1</span></span>|<span data-ttu-id="72a93-117">使用用户名和密码进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="72a93-117">Use username and password for authentication.</span></span>|
|<span data-ttu-id="72a93-118">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="72a93-118">sharedSecret</span></span>|<span data-ttu-id="72a93-119">2 </span><span class="sxs-lookup"><span data-stu-id="72a93-119">2</span></span>|<span data-ttu-id="72a93-120">使用共享密钥进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="72a93-120">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="72a93-121">仅对 iOS IKEv2 有效。</span><span class="sxs-lookup"><span data-stu-id="72a93-121">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="72a93-122">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="72a93-122">derivedCredential</span></span>|<span data-ttu-id="72a93-123">3 </span><span class="sxs-lookup"><span data-stu-id="72a93-123">3</span></span>|<span data-ttu-id="72a93-124">使用派生的凭据进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="72a93-124">Use Derived Credential for Authentication.</span></span>|
|<span data-ttu-id="72a93-125">azureAD</span><span class="sxs-lookup"><span data-stu-id="72a93-125">azureAD</span></span>|<span data-ttu-id="72a93-126">4 </span><span class="sxs-lookup"><span data-stu-id="72a93-126">4</span></span>|<span data-ttu-id="72a93-127">使用 Azure AD 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="72a93-127">Use Azure AD for authentication.</span></span>|



