---
title: windowsInformationProtectionEnforcementLevel 枚举类型
description: WIP 保护强制级别的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c5d5846ad8025b040fb853b8ba6f1dc402e0f15f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373579"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="dd00a-103">windowsInformationProtectionEnforcementLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="dd00a-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="dd00a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dd00a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd00a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dd00a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd00a-106">WIP 保护强制级别的可能值</span><span class="sxs-lookup"><span data-stu-id="dd00a-106">Possible values for WIP Protection enforcement levels</span></span>

## <a name="members"></a><span data-ttu-id="dd00a-107">成员</span><span class="sxs-lookup"><span data-stu-id="dd00a-107">Members</span></span>
|<span data-ttu-id="dd00a-108">成员</span><span class="sxs-lookup"><span data-stu-id="dd00a-108">Member</span></span>|<span data-ttu-id="dd00a-109">值</span><span class="sxs-lookup"><span data-stu-id="dd00a-109">Value</span></span>|<span data-ttu-id="dd00a-110">说明</span><span class="sxs-lookup"><span data-stu-id="dd00a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd00a-111">noProtection</span><span class="sxs-lookup"><span data-stu-id="dd00a-111">noProtection</span></span>|<span data-ttu-id="dd00a-112">0</span><span class="sxs-lookup"><span data-stu-id="dd00a-112">0</span></span>|<span data-ttu-id="dd00a-113">无保护强制实施</span><span class="sxs-lookup"><span data-stu-id="dd00a-113">No protection enforcement</span></span>|
|<span data-ttu-id="dd00a-114">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="dd00a-114">encryptAndAuditOnly</span></span>|<span data-ttu-id="dd00a-115">1</span><span class="sxs-lookup"><span data-stu-id="dd00a-115">1</span></span>|<span data-ttu-id="dd00a-116">仅加密和审核</span><span class="sxs-lookup"><span data-stu-id="dd00a-116">Encrypt and Audit only</span></span>|
|<span data-ttu-id="dd00a-117">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="dd00a-117">encryptAuditAndPrompt</span></span>|<span data-ttu-id="dd00a-118">双面</span><span class="sxs-lookup"><span data-stu-id="dd00a-118">2</span></span>|<span data-ttu-id="dd00a-119">加密、审核和提示</span><span class="sxs-lookup"><span data-stu-id="dd00a-119">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="dd00a-120">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="dd00a-120">encryptAuditAndBlock</span></span>|<span data-ttu-id="dd00a-121">第三章</span><span class="sxs-lookup"><span data-stu-id="dd00a-121">3</span></span>|<span data-ttu-id="dd00a-122">加密、审核和阻止</span><span class="sxs-lookup"><span data-stu-id="dd00a-122">Encrypt, Audit and Block</span></span>|



