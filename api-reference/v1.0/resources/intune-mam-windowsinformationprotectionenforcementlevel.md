---
title: windowsInformationProtectionEnforcementLevel 枚举类型
description: WIP 保护强制级别的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ba8e8cded8ac4a245a556de78fc2ab99443eab3e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448240"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="32481-103">windowsInformationProtectionEnforcementLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="32481-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

<span data-ttu-id="32481-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="32481-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32481-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="32481-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32481-106">WIP 保护强制级别的可能值</span><span class="sxs-lookup"><span data-stu-id="32481-106">Possible values for WIP Protection enforcement levels</span></span>

## <a name="members"></a><span data-ttu-id="32481-107">成员</span><span class="sxs-lookup"><span data-stu-id="32481-107">Members</span></span>
|<span data-ttu-id="32481-108">成员</span><span class="sxs-lookup"><span data-stu-id="32481-108">Member</span></span>|<span data-ttu-id="32481-109">值</span><span class="sxs-lookup"><span data-stu-id="32481-109">Value</span></span>|<span data-ttu-id="32481-110">说明</span><span class="sxs-lookup"><span data-stu-id="32481-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32481-111">noProtection</span><span class="sxs-lookup"><span data-stu-id="32481-111">noProtection</span></span>|<span data-ttu-id="32481-112">0</span><span class="sxs-lookup"><span data-stu-id="32481-112">0</span></span>|<span data-ttu-id="32481-113">无保护强制实施</span><span class="sxs-lookup"><span data-stu-id="32481-113">No protection enforcement</span></span>|
|<span data-ttu-id="32481-114">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="32481-114">encryptAndAuditOnly</span></span>|<span data-ttu-id="32481-115">1 </span><span class="sxs-lookup"><span data-stu-id="32481-115">1</span></span>|<span data-ttu-id="32481-116">仅加密和审核</span><span class="sxs-lookup"><span data-stu-id="32481-116">Encrypt and Audit only</span></span>|
|<span data-ttu-id="32481-117">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="32481-117">encryptAuditAndPrompt</span></span>|<span data-ttu-id="32481-118">2 </span><span class="sxs-lookup"><span data-stu-id="32481-118">2</span></span>|<span data-ttu-id="32481-119">加密、审核和提示</span><span class="sxs-lookup"><span data-stu-id="32481-119">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="32481-120">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="32481-120">encryptAuditAndBlock</span></span>|<span data-ttu-id="32481-121">3 </span><span class="sxs-lookup"><span data-stu-id="32481-121">3</span></span>|<span data-ttu-id="32481-122">加密、审核和阻止</span><span class="sxs-lookup"><span data-stu-id="32481-122">Encrypt, Audit and Block</span></span>|




