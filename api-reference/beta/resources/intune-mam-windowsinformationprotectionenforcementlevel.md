---
title: windowsInformationProtectionEnforcementLevel 枚举类型
description: WIP 保护强制级别的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ac5a360bebfc60dbaf4315be5e4e189f91c1f2b8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522137"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="a5bf8-103">windowsInformationProtectionEnforcementLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a5bf8-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="a5bf8-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a5bf8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5bf8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a5bf8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5bf8-106">WIP 保护强制级别的可能值</span><span class="sxs-lookup"><span data-stu-id="a5bf8-106">Possible values for WIP Protection enforcement levels</span></span>

## <a name="members"></a><span data-ttu-id="a5bf8-107">成员</span><span class="sxs-lookup"><span data-stu-id="a5bf8-107">Members</span></span>
|<span data-ttu-id="a5bf8-108">成员</span><span class="sxs-lookup"><span data-stu-id="a5bf8-108">Member</span></span>|<span data-ttu-id="a5bf8-109">值</span><span class="sxs-lookup"><span data-stu-id="a5bf8-109">Value</span></span>|<span data-ttu-id="a5bf8-110">说明</span><span class="sxs-lookup"><span data-stu-id="a5bf8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5bf8-111">noProtection</span><span class="sxs-lookup"><span data-stu-id="a5bf8-111">noProtection</span></span>|<span data-ttu-id="a5bf8-112">0</span><span class="sxs-lookup"><span data-stu-id="a5bf8-112">0</span></span>|<span data-ttu-id="a5bf8-113">无保护强制实施</span><span class="sxs-lookup"><span data-stu-id="a5bf8-113">No protection enforcement</span></span>|
|<span data-ttu-id="a5bf8-114">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="a5bf8-114">encryptAndAuditOnly</span></span>|<span data-ttu-id="a5bf8-115">1</span><span class="sxs-lookup"><span data-stu-id="a5bf8-115">1</span></span>|<span data-ttu-id="a5bf8-116">仅加密和审核</span><span class="sxs-lookup"><span data-stu-id="a5bf8-116">Encrypt and Audit only</span></span>|
|<span data-ttu-id="a5bf8-117">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="a5bf8-117">encryptAuditAndPrompt</span></span>|<span data-ttu-id="a5bf8-118">2 </span><span class="sxs-lookup"><span data-stu-id="a5bf8-118">2</span></span>|<span data-ttu-id="a5bf8-119">加密、审核和提示</span><span class="sxs-lookup"><span data-stu-id="a5bf8-119">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="a5bf8-120">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="a5bf8-120">encryptAuditAndBlock</span></span>|<span data-ttu-id="a5bf8-121">3 </span><span class="sxs-lookup"><span data-stu-id="a5bf8-121">3</span></span>|<span data-ttu-id="a5bf8-122">加密、审核和阻止</span><span class="sxs-lookup"><span data-stu-id="a5bf8-122">Encrypt, Audit and Block</span></span>|





