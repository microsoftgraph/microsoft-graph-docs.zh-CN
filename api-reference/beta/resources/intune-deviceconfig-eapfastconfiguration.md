---
title: eapFastConfiguration 枚举类型
description: EAP 快速配置的可用设置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca19e48f07d7bdb2859af9924cd391a9dbdfdf3f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989887"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="822bd-103">eapFastConfiguration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="822bd-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="822bd-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="822bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="822bd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="822bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="822bd-106">EAP 快速配置的可用设置。</span><span class="sxs-lookup"><span data-stu-id="822bd-106">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="822bd-107">成员</span><span class="sxs-lookup"><span data-stu-id="822bd-107">Members</span></span>
|<span data-ttu-id="822bd-108">成员</span><span class="sxs-lookup"><span data-stu-id="822bd-108">Member</span></span>|<span data-ttu-id="822bd-109">值</span><span class="sxs-lookup"><span data-stu-id="822bd-109">Value</span></span>|<span data-ttu-id="822bd-110">说明</span><span class="sxs-lookup"><span data-stu-id="822bd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="822bd-111">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="822bd-111">noProtectedAccessCredential</span></span>|<span data-ttu-id="822bd-112">0</span><span class="sxs-lookup"><span data-stu-id="822bd-112">0</span></span>|<span data-ttu-id="822bd-113">使用 EAP-FAST (无保护性访问凭据 (PAC))。</span><span class="sxs-lookup"><span data-stu-id="822bd-113">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="822bd-114">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="822bd-114">useProtectedAccessCredential</span></span>|<span data-ttu-id="822bd-115">1</span><span class="sxs-lookup"><span data-stu-id="822bd-115">1</span></span>|<span data-ttu-id="822bd-116">使用受保护的访问凭据 (PAC)。</span><span class="sxs-lookup"><span data-stu-id="822bd-116">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="822bd-117">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="822bd-117">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="822bd-118">双面</span><span class="sxs-lookup"><span data-stu-id="822bd-118">2</span></span>|<span data-ttu-id="822bd-119">使用保护性接入身分凭证 (PAC) 和预配 PAC。</span><span class="sxs-lookup"><span data-stu-id="822bd-119">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="822bd-120">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="822bd-120">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="822bd-121">第三章</span><span class="sxs-lookup"><span data-stu-id="822bd-121">3</span></span>|<span data-ttu-id="822bd-122">使用受保护的访问凭据 (PAC)、预配 PAC, 并以匿名方式执行此操作。</span><span class="sxs-lookup"><span data-stu-id="822bd-122">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|





