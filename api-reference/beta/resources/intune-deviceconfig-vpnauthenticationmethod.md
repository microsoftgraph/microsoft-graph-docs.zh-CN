---
title: vpnAuthenticationMethod 枚举类型
description: VPN 身份验证方法。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dd3cc6887f5434df00a2ed9a817c0ca79c8c880e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43412449"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="e1b97-103">vpnAuthenticationMethod 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e1b97-103">vpnAuthenticationMethod enum type</span></span>

<span data-ttu-id="e1b97-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1b97-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1b97-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e1b97-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1b97-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e1b97-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1b97-107">VPN 身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="e1b97-107">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="e1b97-108">成员</span><span class="sxs-lookup"><span data-stu-id="e1b97-108">Members</span></span>
|<span data-ttu-id="e1b97-109">成员</span><span class="sxs-lookup"><span data-stu-id="e1b97-109">Member</span></span>|<span data-ttu-id="e1b97-110">值</span><span class="sxs-lookup"><span data-stu-id="e1b97-110">Value</span></span>|<span data-ttu-id="e1b97-111">说明</span><span class="sxs-lookup"><span data-stu-id="e1b97-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1b97-112">证书</span><span class="sxs-lookup"><span data-stu-id="e1b97-112">certificate</span></span>|<span data-ttu-id="e1b97-113">0</span><span class="sxs-lookup"><span data-stu-id="e1b97-113">0</span></span>|<span data-ttu-id="e1b97-114">使用证书进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="e1b97-114">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="e1b97-115">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="e1b97-115">usernameAndPassword</span></span>|<span data-ttu-id="e1b97-116">1</span><span class="sxs-lookup"><span data-stu-id="e1b97-116">1</span></span>|<span data-ttu-id="e1b97-117">使用用户名和密码进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="e1b97-117">Use username and password for authentication.</span></span>|
|<span data-ttu-id="e1b97-118">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="e1b97-118">sharedSecret</span></span>|<span data-ttu-id="e1b97-119">双面</span><span class="sxs-lookup"><span data-stu-id="e1b97-119">2</span></span>|<span data-ttu-id="e1b97-120">使用共享密钥进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="e1b97-120">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="e1b97-121">仅对 iOS IKEv2 有效。</span><span class="sxs-lookup"><span data-stu-id="e1b97-121">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="e1b97-122">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="e1b97-122">derivedCredential</span></span>|<span data-ttu-id="e1b97-123">第三章</span><span class="sxs-lookup"><span data-stu-id="e1b97-123">3</span></span>|<span data-ttu-id="e1b97-124">使用派生的凭据进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="e1b97-124">Use Derived Credential for Authentication.</span></span>|



