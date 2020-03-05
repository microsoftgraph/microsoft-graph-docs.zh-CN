---
title: eapFastConfiguration 枚举类型
description: EAP 快速配置的可用设置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: db3f39eaeb375705c974e907ae4b0a177bd6c4ac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526544"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="c5aa3-103">eapFastConfiguration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c5aa3-103">eapFastConfiguration enum type</span></span>

<span data-ttu-id="c5aa3-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c5aa3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5aa3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c5aa3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5aa3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c5aa3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5aa3-107">EAP 快速配置的可用设置。</span><span class="sxs-lookup"><span data-stu-id="c5aa3-107">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="c5aa3-108">成员</span><span class="sxs-lookup"><span data-stu-id="c5aa3-108">Members</span></span>
|<span data-ttu-id="c5aa3-109">成员</span><span class="sxs-lookup"><span data-stu-id="c5aa3-109">Member</span></span>|<span data-ttu-id="c5aa3-110">值</span><span class="sxs-lookup"><span data-stu-id="c5aa3-110">Value</span></span>|<span data-ttu-id="c5aa3-111">说明</span><span class="sxs-lookup"><span data-stu-id="c5aa3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5aa3-112">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="c5aa3-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="c5aa3-113">0</span><span class="sxs-lookup"><span data-stu-id="c5aa3-113">0</span></span>|<span data-ttu-id="c5aa3-114">使用 EAP-FAST （无保护性访问凭据（PAC））。</span><span class="sxs-lookup"><span data-stu-id="c5aa3-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="c5aa3-115">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="c5aa3-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="c5aa3-116">1 </span><span class="sxs-lookup"><span data-stu-id="c5aa3-116">1</span></span>|<span data-ttu-id="c5aa3-117">使用受保护的访问凭据（PAC）。</span><span class="sxs-lookup"><span data-stu-id="c5aa3-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="c5aa3-118">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="c5aa3-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="c5aa3-119">2 </span><span class="sxs-lookup"><span data-stu-id="c5aa3-119">2</span></span>|<span data-ttu-id="c5aa3-120">使用保护性接入身分凭证（PAC）和预配 PAC。</span><span class="sxs-lookup"><span data-stu-id="c5aa3-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="c5aa3-121">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="c5aa3-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="c5aa3-122">3 </span><span class="sxs-lookup"><span data-stu-id="c5aa3-122">3</span></span>|<span data-ttu-id="c5aa3-123">使用受保护的访问凭据（PAC）、预配 PAC，并以匿名方式执行此操作。</span><span class="sxs-lookup"><span data-stu-id="c5aa3-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|



