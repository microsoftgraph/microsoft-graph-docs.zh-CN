---
title: windowsInformationProtectionEnforcementLevel 枚举类型
description: WIP 保护强制级别的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ac5a360bebfc60dbaf4315be5e4e189f91c1f2b8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801615"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="da176-103">windowsInformationProtectionEnforcementLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="da176-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="da176-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="da176-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da176-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da176-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da176-106">WIP 保护强制级别的可能值</span><span class="sxs-lookup"><span data-stu-id="da176-106">Possible values for WIP Protection enforcement levels</span></span>

## <a name="members"></a><span data-ttu-id="da176-107">成员</span><span class="sxs-lookup"><span data-stu-id="da176-107">Members</span></span>
|<span data-ttu-id="da176-108">成员</span><span class="sxs-lookup"><span data-stu-id="da176-108">Member</span></span>|<span data-ttu-id="da176-109">值</span><span class="sxs-lookup"><span data-stu-id="da176-109">Value</span></span>|<span data-ttu-id="da176-110">说明</span><span class="sxs-lookup"><span data-stu-id="da176-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da176-111">noProtection</span><span class="sxs-lookup"><span data-stu-id="da176-111">noProtection</span></span>|<span data-ttu-id="da176-112">0</span><span class="sxs-lookup"><span data-stu-id="da176-112">0</span></span>|<span data-ttu-id="da176-113">无保护强制实施</span><span class="sxs-lookup"><span data-stu-id="da176-113">No protection enforcement</span></span>|
|<span data-ttu-id="da176-114">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="da176-114">encryptAndAuditOnly</span></span>|<span data-ttu-id="da176-115">1</span><span class="sxs-lookup"><span data-stu-id="da176-115">1</span></span>|<span data-ttu-id="da176-116">仅加密和审核</span><span class="sxs-lookup"><span data-stu-id="da176-116">Encrypt and Audit only</span></span>|
|<span data-ttu-id="da176-117">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="da176-117">encryptAuditAndPrompt</span></span>|<span data-ttu-id="da176-118">双面</span><span class="sxs-lookup"><span data-stu-id="da176-118">2</span></span>|<span data-ttu-id="da176-119">加密、审核和提示</span><span class="sxs-lookup"><span data-stu-id="da176-119">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="da176-120">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="da176-120">encryptAuditAndBlock</span></span>|<span data-ttu-id="da176-121">第三章</span><span class="sxs-lookup"><span data-stu-id="da176-121">3</span></span>|<span data-ttu-id="da176-122">加密、审核和阻止</span><span class="sxs-lookup"><span data-stu-id="da176-122">Encrypt, Audit and Block</span></span>|





