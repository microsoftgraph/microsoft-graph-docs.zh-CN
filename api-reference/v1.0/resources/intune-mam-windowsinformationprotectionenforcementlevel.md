---
title: windowsInformationProtectionEnforcementLevel 枚举类型
description: WIP 保护强制级别的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4a1b9a985753e54fcd36d9bcf568c10a9821fad9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752313"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="f7fa0-103">windowsInformationProtectionEnforcementLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f7fa0-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

<span data-ttu-id="f7fa0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7fa0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7fa0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7fa0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7fa0-106">WIP 保护强制级别的可能值</span><span class="sxs-lookup"><span data-stu-id="f7fa0-106">Possible values for WIP Protection enforcement levels</span></span>

## <a name="members"></a><span data-ttu-id="f7fa0-107">成员</span><span class="sxs-lookup"><span data-stu-id="f7fa0-107">Members</span></span>
|<span data-ttu-id="f7fa0-108">成员</span><span class="sxs-lookup"><span data-stu-id="f7fa0-108">Member</span></span>|<span data-ttu-id="f7fa0-109">值</span><span class="sxs-lookup"><span data-stu-id="f7fa0-109">Value</span></span>|<span data-ttu-id="f7fa0-110">Description</span><span class="sxs-lookup"><span data-stu-id="f7fa0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7fa0-111">noProtection</span><span class="sxs-lookup"><span data-stu-id="f7fa0-111">noProtection</span></span>|<span data-ttu-id="f7fa0-112">0</span><span class="sxs-lookup"><span data-stu-id="f7fa0-112">0</span></span>|<span data-ttu-id="f7fa0-113">不强制执行保护</span><span class="sxs-lookup"><span data-stu-id="f7fa0-113">No protection enforcement</span></span>|
|<span data-ttu-id="f7fa0-114">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="f7fa0-114">encryptAndAuditOnly</span></span>|<span data-ttu-id="f7fa0-115">1</span><span class="sxs-lookup"><span data-stu-id="f7fa0-115">1</span></span>|<span data-ttu-id="f7fa0-116">仅加密和审核</span><span class="sxs-lookup"><span data-stu-id="f7fa0-116">Encrypt and Audit only</span></span>|
|<span data-ttu-id="f7fa0-117">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="f7fa0-117">encryptAuditAndPrompt</span></span>|<span data-ttu-id="f7fa0-118">2</span><span class="sxs-lookup"><span data-stu-id="f7fa0-118">2</span></span>|<span data-ttu-id="f7fa0-119">加密、审核和提示</span><span class="sxs-lookup"><span data-stu-id="f7fa0-119">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="f7fa0-120">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="f7fa0-120">encryptAuditAndBlock</span></span>|<span data-ttu-id="f7fa0-121">3</span><span class="sxs-lookup"><span data-stu-id="f7fa0-121">3</span></span>|<span data-ttu-id="f7fa0-122">加密、审核和阻止</span><span class="sxs-lookup"><span data-stu-id="f7fa0-122">Encrypt, Audit and Block</span></span>|




