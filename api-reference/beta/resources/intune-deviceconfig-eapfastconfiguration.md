---
title: eapFastConfiguration 枚举类型
description: EAP 快速配置的可用设置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 15232635cfcbe5064c5efe7beeb05e58c5e321ee
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701548"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="852a9-103">eapFastConfiguration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="852a9-103">eapFastConfiguration enum type</span></span>

<span data-ttu-id="852a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="852a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="852a9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="852a9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="852a9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="852a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="852a9-107">EAP 快速配置的可用设置。</span><span class="sxs-lookup"><span data-stu-id="852a9-107">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="852a9-108">成员</span><span class="sxs-lookup"><span data-stu-id="852a9-108">Members</span></span>
|<span data-ttu-id="852a9-109">成员</span><span class="sxs-lookup"><span data-stu-id="852a9-109">Member</span></span>|<span data-ttu-id="852a9-110">值</span><span class="sxs-lookup"><span data-stu-id="852a9-110">Value</span></span>|<span data-ttu-id="852a9-111">说明</span><span class="sxs-lookup"><span data-stu-id="852a9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="852a9-112">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="852a9-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="852a9-113">0</span><span class="sxs-lookup"><span data-stu-id="852a9-113">0</span></span>|<span data-ttu-id="852a9-114">使用 EAP-FAST) 的无保护性访问凭据 (PAC。</span><span class="sxs-lookup"><span data-stu-id="852a9-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="852a9-115">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="852a9-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="852a9-116">1</span><span class="sxs-lookup"><span data-stu-id="852a9-116">1</span></span>|<span data-ttu-id="852a9-117">使用受保护的访问凭据 (PAC) 。</span><span class="sxs-lookup"><span data-stu-id="852a9-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="852a9-118">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="852a9-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="852a9-119">双面</span><span class="sxs-lookup"><span data-stu-id="852a9-119">2</span></span>|<span data-ttu-id="852a9-120">使用受保护的访问凭据 (PAC) 和预配 PAC。</span><span class="sxs-lookup"><span data-stu-id="852a9-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="852a9-121">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="852a9-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="852a9-122">第三章</span><span class="sxs-lookup"><span data-stu-id="852a9-122">3</span></span>|<span data-ttu-id="852a9-123">使用受保护的访问凭据 (PAC) 、预配 PAC，并以匿名方式执行此操作。</span><span class="sxs-lookup"><span data-stu-id="852a9-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|





