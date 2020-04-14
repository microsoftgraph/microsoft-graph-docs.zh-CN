---
title: eapFastConfiguration 枚举类型
description: EAP 快速配置的可用设置。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f0d045252c058b2557fd9bb4448e0275953e0b09
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469130"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="18ef7-103">eapFastConfiguration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="18ef7-103">eapFastConfiguration enum type</span></span>

<span data-ttu-id="18ef7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18ef7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18ef7-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="18ef7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18ef7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="18ef7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18ef7-107">EAP 快速配置的可用设置。</span><span class="sxs-lookup"><span data-stu-id="18ef7-107">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="18ef7-108">成员</span><span class="sxs-lookup"><span data-stu-id="18ef7-108">Members</span></span>
|<span data-ttu-id="18ef7-109">成员</span><span class="sxs-lookup"><span data-stu-id="18ef7-109">Member</span></span>|<span data-ttu-id="18ef7-110">值</span><span class="sxs-lookup"><span data-stu-id="18ef7-110">Value</span></span>|<span data-ttu-id="18ef7-111">说明</span><span class="sxs-lookup"><span data-stu-id="18ef7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18ef7-112">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="18ef7-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="18ef7-113">0</span><span class="sxs-lookup"><span data-stu-id="18ef7-113">0</span></span>|<span data-ttu-id="18ef7-114">使用 EAP-FAST （无保护性访问凭据（PAC））。</span><span class="sxs-lookup"><span data-stu-id="18ef7-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="18ef7-115">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="18ef7-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="18ef7-116">1</span><span class="sxs-lookup"><span data-stu-id="18ef7-116">1</span></span>|<span data-ttu-id="18ef7-117">使用受保护的访问凭据（PAC）。</span><span class="sxs-lookup"><span data-stu-id="18ef7-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="18ef7-118">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="18ef7-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="18ef7-119">双面</span><span class="sxs-lookup"><span data-stu-id="18ef7-119">2</span></span>|<span data-ttu-id="18ef7-120">使用保护性接入身分凭证（PAC）和预配 PAC。</span><span class="sxs-lookup"><span data-stu-id="18ef7-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="18ef7-121">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="18ef7-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="18ef7-122">第三章</span><span class="sxs-lookup"><span data-stu-id="18ef7-122">3</span></span>|<span data-ttu-id="18ef7-123">使用受保护的访问凭据（PAC）、预配 PAC，并以匿名方式执行此操作。</span><span class="sxs-lookup"><span data-stu-id="18ef7-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|



