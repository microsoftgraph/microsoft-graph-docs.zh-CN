---
title: eapFastConfiguration 枚举类型
description: EAP 快速配置的可用设置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7857e5c2f7b2bd8fdb1f7e0754e587f4498c6d0e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332657"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="37262-103">eapFastConfiguration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="37262-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="37262-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="37262-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37262-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="37262-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37262-106">EAP 快速配置的可用设置。</span><span class="sxs-lookup"><span data-stu-id="37262-106">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="37262-107">成员</span><span class="sxs-lookup"><span data-stu-id="37262-107">Members</span></span>
|<span data-ttu-id="37262-108">成员</span><span class="sxs-lookup"><span data-stu-id="37262-108">Member</span></span>|<span data-ttu-id="37262-109">值</span><span class="sxs-lookup"><span data-stu-id="37262-109">Value</span></span>|<span data-ttu-id="37262-110">说明</span><span class="sxs-lookup"><span data-stu-id="37262-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37262-111">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="37262-111">noProtectedAccessCredential</span></span>|<span data-ttu-id="37262-112">0</span><span class="sxs-lookup"><span data-stu-id="37262-112">0</span></span>|<span data-ttu-id="37262-113">使用 EAP-FAST (无保护性访问凭据 (PAC))。</span><span class="sxs-lookup"><span data-stu-id="37262-113">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="37262-114">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="37262-114">useProtectedAccessCredential</span></span>|<span data-ttu-id="37262-115">1</span><span class="sxs-lookup"><span data-stu-id="37262-115">1</span></span>|<span data-ttu-id="37262-116">使用受保护的访问凭据 (PAC)。</span><span class="sxs-lookup"><span data-stu-id="37262-116">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="37262-117">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="37262-117">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="37262-118">双面</span><span class="sxs-lookup"><span data-stu-id="37262-118">2</span></span>|<span data-ttu-id="37262-119">使用保护性接入身分凭证 (PAC) 和预配 PAC。</span><span class="sxs-lookup"><span data-stu-id="37262-119">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="37262-120">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="37262-120">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="37262-121">第三章</span><span class="sxs-lookup"><span data-stu-id="37262-121">3</span></span>|<span data-ttu-id="37262-122">使用受保护的访问凭据 (PAC)、预配 PAC, 并以匿名方式执行此操作。</span><span class="sxs-lookup"><span data-stu-id="37262-122">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|



