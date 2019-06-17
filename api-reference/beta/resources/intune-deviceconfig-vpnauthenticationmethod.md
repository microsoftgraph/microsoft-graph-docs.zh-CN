---
title: vpnAuthenticationMethod 枚举类型
description: VPN 身份验证方法。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 343b8e3809a3f61926521a43d873161b2d5eee5f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994312"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="6071d-103">vpnAuthenticationMethod 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6071d-103">vpnAuthenticationMethod enum type</span></span>

> <span data-ttu-id="6071d-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6071d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6071d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6071d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6071d-106">VPN 身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="6071d-106">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="6071d-107">成员</span><span class="sxs-lookup"><span data-stu-id="6071d-107">Members</span></span>
|<span data-ttu-id="6071d-108">成员</span><span class="sxs-lookup"><span data-stu-id="6071d-108">Member</span></span>|<span data-ttu-id="6071d-109">值</span><span class="sxs-lookup"><span data-stu-id="6071d-109">Value</span></span>|<span data-ttu-id="6071d-110">说明</span><span class="sxs-lookup"><span data-stu-id="6071d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6071d-111">证书</span><span class="sxs-lookup"><span data-stu-id="6071d-111">certificate</span></span>|<span data-ttu-id="6071d-112">0</span><span class="sxs-lookup"><span data-stu-id="6071d-112">0</span></span>|<span data-ttu-id="6071d-113">使用证书进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="6071d-113">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="6071d-114">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="6071d-114">usernameAndPassword</span></span>|<span data-ttu-id="6071d-115">1</span><span class="sxs-lookup"><span data-stu-id="6071d-115">1</span></span>|<span data-ttu-id="6071d-116">使用用户名和密码进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="6071d-116">Use username and password for authentication.</span></span>|
|<span data-ttu-id="6071d-117">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="6071d-117">sharedSecret</span></span>|<span data-ttu-id="6071d-118">双面</span><span class="sxs-lookup"><span data-stu-id="6071d-118">2</span></span>|<span data-ttu-id="6071d-119">使用共享密钥进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="6071d-119">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="6071d-120">仅对 iOS IKEv2 有效。</span><span class="sxs-lookup"><span data-stu-id="6071d-120">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="6071d-121">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="6071d-121">derivedCredential</span></span>|<span data-ttu-id="6071d-122">第三章</span><span class="sxs-lookup"><span data-stu-id="6071d-122">3</span></span>|<span data-ttu-id="6071d-123">使用派生的凭据进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="6071d-123">Use Derived Credential for Authentication.</span></span>  <span data-ttu-id="6071d-124">仅对 iOS 有效。</span><span class="sxs-lookup"><span data-stu-id="6071d-124">Only valid for iOS.</span></span>|





