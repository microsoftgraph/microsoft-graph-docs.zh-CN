---
title: vpnAuthenticationMethod 枚举类型
description: VPN 身份验证方法。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: dbb441bfc32e2de64f5950c033bdd24a3b05c59e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726375"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="23dc3-103">vpnAuthenticationMethod 枚举类型</span><span class="sxs-lookup"><span data-stu-id="23dc3-103">vpnAuthenticationMethod enum type</span></span>

<span data-ttu-id="23dc3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23dc3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23dc3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="23dc3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23dc3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="23dc3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23dc3-107">VPN 身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="23dc3-107">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="23dc3-108">成员</span><span class="sxs-lookup"><span data-stu-id="23dc3-108">Members</span></span>
|<span data-ttu-id="23dc3-109">成员</span><span class="sxs-lookup"><span data-stu-id="23dc3-109">Member</span></span>|<span data-ttu-id="23dc3-110">值</span><span class="sxs-lookup"><span data-stu-id="23dc3-110">Value</span></span>|<span data-ttu-id="23dc3-111">说明</span><span class="sxs-lookup"><span data-stu-id="23dc3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23dc3-112">证书</span><span class="sxs-lookup"><span data-stu-id="23dc3-112">certificate</span></span>|<span data-ttu-id="23dc3-113">0</span><span class="sxs-lookup"><span data-stu-id="23dc3-113">0</span></span>|<span data-ttu-id="23dc3-114">使用证书进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="23dc3-114">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="23dc3-115">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="23dc3-115">usernameAndPassword</span></span>|<span data-ttu-id="23dc3-116">1</span><span class="sxs-lookup"><span data-stu-id="23dc3-116">1</span></span>|<span data-ttu-id="23dc3-117">使用用户名和密码进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="23dc3-117">Use username and password for authentication.</span></span>|
|<span data-ttu-id="23dc3-118">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="23dc3-118">sharedSecret</span></span>|<span data-ttu-id="23dc3-119">双面</span><span class="sxs-lookup"><span data-stu-id="23dc3-119">2</span></span>|<span data-ttu-id="23dc3-120">使用共享密钥进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="23dc3-120">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="23dc3-121">仅对 iOS IKEv2 有效。</span><span class="sxs-lookup"><span data-stu-id="23dc3-121">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="23dc3-122">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="23dc3-122">derivedCredential</span></span>|<span data-ttu-id="23dc3-123">第三章</span><span class="sxs-lookup"><span data-stu-id="23dc3-123">3</span></span>|<span data-ttu-id="23dc3-124">使用派生的凭据进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="23dc3-124">Use Derived Credential for Authentication.</span></span>|
|<span data-ttu-id="23dc3-125">azureAD</span><span class="sxs-lookup"><span data-stu-id="23dc3-125">azureAD</span></span>|<span data-ttu-id="23dc3-126">4 </span><span class="sxs-lookup"><span data-stu-id="23dc3-126">4</span></span>|<span data-ttu-id="23dc3-127">使用 Azure AD 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="23dc3-127">Use Azure AD for authentication.</span></span>|





