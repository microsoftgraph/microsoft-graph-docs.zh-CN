---
title: windowsInformationProtectionEnforcementLevel 枚举类型
description: WIP 保护强制级别的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e6fb9528a3a4d87f13e1901c18885b7224291389
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42780624"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="1cb37-103">windowsInformationProtectionEnforcementLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1cb37-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="1cb37-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1cb37-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1cb37-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1cb37-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cb37-106">WIP 保护强制级别的可能值</span><span class="sxs-lookup"><span data-stu-id="1cb37-106">Possible values for WIP Protection enforcement levels</span></span>

## <a name="members"></a><span data-ttu-id="1cb37-107">成员</span><span class="sxs-lookup"><span data-stu-id="1cb37-107">Members</span></span>
|<span data-ttu-id="1cb37-108">成员</span><span class="sxs-lookup"><span data-stu-id="1cb37-108">Member</span></span>|<span data-ttu-id="1cb37-109">值</span><span class="sxs-lookup"><span data-stu-id="1cb37-109">Value</span></span>|<span data-ttu-id="1cb37-110">说明</span><span class="sxs-lookup"><span data-stu-id="1cb37-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cb37-111">noProtection</span><span class="sxs-lookup"><span data-stu-id="1cb37-111">noProtection</span></span>|<span data-ttu-id="1cb37-112">0</span><span class="sxs-lookup"><span data-stu-id="1cb37-112">0</span></span>|<span data-ttu-id="1cb37-113">无保护强制实施</span><span class="sxs-lookup"><span data-stu-id="1cb37-113">No protection enforcement</span></span>|
|<span data-ttu-id="1cb37-114">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="1cb37-114">encryptAndAuditOnly</span></span>|<span data-ttu-id="1cb37-115">1</span><span class="sxs-lookup"><span data-stu-id="1cb37-115">1</span></span>|<span data-ttu-id="1cb37-116">仅加密和审核</span><span class="sxs-lookup"><span data-stu-id="1cb37-116">Encrypt and Audit only</span></span>|
|<span data-ttu-id="1cb37-117">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="1cb37-117">encryptAuditAndPrompt</span></span>|<span data-ttu-id="1cb37-118">双面</span><span class="sxs-lookup"><span data-stu-id="1cb37-118">2</span></span>|<span data-ttu-id="1cb37-119">加密、审核和提示</span><span class="sxs-lookup"><span data-stu-id="1cb37-119">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="1cb37-120">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="1cb37-120">encryptAuditAndBlock</span></span>|<span data-ttu-id="1cb37-121">第三章</span><span class="sxs-lookup"><span data-stu-id="1cb37-121">3</span></span>|<span data-ttu-id="1cb37-122">加密、审核和阻止</span><span class="sxs-lookup"><span data-stu-id="1cb37-122">Encrypt, Audit and Block</span></span>|



