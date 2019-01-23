---
title: eapFastConfiguration 枚举类型
description: EAP FAST 配置的可用设置。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1fa2c3c3a4cf0bc245ea7c9fbc4294d69215deee
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399386"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="763bd-103">eapFastConfiguration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="763bd-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="763bd-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="763bd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="763bd-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="763bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="763bd-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="763bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="763bd-107">EAP FAST 配置的可用设置。</span><span class="sxs-lookup"><span data-stu-id="763bd-107">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="763bd-108">成员</span><span class="sxs-lookup"><span data-stu-id="763bd-108">Members</span></span>
|<span data-ttu-id="763bd-109">成员</span><span class="sxs-lookup"><span data-stu-id="763bd-109">Member</span></span>|<span data-ttu-id="763bd-110">值</span><span class="sxs-lookup"><span data-stu-id="763bd-110">Value</span></span>|<span data-ttu-id="763bd-111">说明</span><span class="sxs-lookup"><span data-stu-id="763bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="763bd-112">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="763bd-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="763bd-113">0</span><span class="sxs-lookup"><span data-stu-id="763bd-113">0</span></span>|<span data-ttu-id="763bd-114">使用 EAP-FAST 不受保护的访问凭据 (PAC)。</span><span class="sxs-lookup"><span data-stu-id="763bd-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="763bd-115">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="763bd-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="763bd-116">1</span><span class="sxs-lookup"><span data-stu-id="763bd-116">1</span></span>|<span data-ttu-id="763bd-117">使用受保护访问凭据 (PAC)。</span><span class="sxs-lookup"><span data-stu-id="763bd-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="763bd-118">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="763bd-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="763bd-119">2</span><span class="sxs-lookup"><span data-stu-id="763bd-119">2</span></span>|<span data-ttu-id="763bd-120">使用受保护的访问凭据 (PAC) 和设置 pac。</span><span class="sxs-lookup"><span data-stu-id="763bd-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="763bd-121">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="763bd-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="763bd-122">3</span><span class="sxs-lookup"><span data-stu-id="763bd-122">3</span></span>|<span data-ttu-id="763bd-123">使用受保护访问凭据 (PAC)，设置 PAC，并以匿名方式这样。</span><span class="sxs-lookup"><span data-stu-id="763bd-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|




