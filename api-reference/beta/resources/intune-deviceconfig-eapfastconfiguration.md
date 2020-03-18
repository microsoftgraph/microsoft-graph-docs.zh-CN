---
title: eapFastConfiguration 枚举类型
description: EAP 快速配置的可用设置。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b70e2688473f9af93dcd3b0f0d4d05b77d81446f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791952"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="edb48-103">eapFastConfiguration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="edb48-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="edb48-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="edb48-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edb48-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="edb48-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edb48-106">EAP 快速配置的可用设置。</span><span class="sxs-lookup"><span data-stu-id="edb48-106">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="edb48-107">成员</span><span class="sxs-lookup"><span data-stu-id="edb48-107">Members</span></span>
|<span data-ttu-id="edb48-108">成员</span><span class="sxs-lookup"><span data-stu-id="edb48-108">Member</span></span>|<span data-ttu-id="edb48-109">值</span><span class="sxs-lookup"><span data-stu-id="edb48-109">Value</span></span>|<span data-ttu-id="edb48-110">说明</span><span class="sxs-lookup"><span data-stu-id="edb48-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edb48-111">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="edb48-111">noProtectedAccessCredential</span></span>|<span data-ttu-id="edb48-112">0</span><span class="sxs-lookup"><span data-stu-id="edb48-112">0</span></span>|<span data-ttu-id="edb48-113">使用 EAP-FAST （无保护性访问凭据（PAC））。</span><span class="sxs-lookup"><span data-stu-id="edb48-113">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="edb48-114">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="edb48-114">useProtectedAccessCredential</span></span>|<span data-ttu-id="edb48-115">1</span><span class="sxs-lookup"><span data-stu-id="edb48-115">1</span></span>|<span data-ttu-id="edb48-116">使用受保护的访问凭据（PAC）。</span><span class="sxs-lookup"><span data-stu-id="edb48-116">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="edb48-117">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="edb48-117">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="edb48-118">双面</span><span class="sxs-lookup"><span data-stu-id="edb48-118">2</span></span>|<span data-ttu-id="edb48-119">使用保护性接入身分凭证（PAC）和预配 PAC。</span><span class="sxs-lookup"><span data-stu-id="edb48-119">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="edb48-120">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="edb48-120">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="edb48-121">第三章</span><span class="sxs-lookup"><span data-stu-id="edb48-121">3</span></span>|<span data-ttu-id="edb48-122">使用受保护的访问凭据（PAC）、预配 PAC，并以匿名方式执行此操作。</span><span class="sxs-lookup"><span data-stu-id="edb48-122">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|



