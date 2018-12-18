---
title: eapFastConfiguration 枚举类型
description: EAP FAST 配置的可用设置。
author: tfitzmac
ms.openlocfilehash: ba84adb86e9910df47bd236fd2bd348cbc9c8e6f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326360"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="a326d-103">eapFastConfiguration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a326d-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="a326d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a326d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a326d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a326d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a326d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a326d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a326d-107">EAP FAST 配置的可用设置。</span><span class="sxs-lookup"><span data-stu-id="a326d-107">Available settings for EAP-FAST Configuration.</span></span>
## <a name="members"></a><span data-ttu-id="a326d-108">成员</span><span class="sxs-lookup"><span data-stu-id="a326d-108">Members</span></span>
|<span data-ttu-id="a326d-109">成员</span><span class="sxs-lookup"><span data-stu-id="a326d-109">Member</span></span>|<span data-ttu-id="a326d-110">值</span><span class="sxs-lookup"><span data-stu-id="a326d-110">Value</span></span>|<span data-ttu-id="a326d-111">说明</span><span class="sxs-lookup"><span data-stu-id="a326d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a326d-112">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="a326d-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="a326d-113">0</span><span class="sxs-lookup"><span data-stu-id="a326d-113">0</span></span>|<span data-ttu-id="a326d-114">使用 EAP-FAST 不受保护的访问凭据 (PAC)。</span><span class="sxs-lookup"><span data-stu-id="a326d-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="a326d-115">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="a326d-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="a326d-116">1</span><span class="sxs-lookup"><span data-stu-id="a326d-116">1</span></span>|<span data-ttu-id="a326d-117">使用受保护访问凭据 (PAC)。</span><span class="sxs-lookup"><span data-stu-id="a326d-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="a326d-118">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="a326d-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="a326d-119">2</span><span class="sxs-lookup"><span data-stu-id="a326d-119">2</span></span>|<span data-ttu-id="a326d-120">使用受保护的访问凭据 (PAC) 和设置 pac。</span><span class="sxs-lookup"><span data-stu-id="a326d-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="a326d-121">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="a326d-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="a326d-122">3</span><span class="sxs-lookup"><span data-stu-id="a326d-122">3</span></span>|<span data-ttu-id="a326d-123">使用受保护访问凭据 (PAC)，设置 PAC，并以匿名方式这样。</span><span class="sxs-lookup"><span data-stu-id="a326d-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|





