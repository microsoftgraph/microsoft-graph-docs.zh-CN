---
title: windowsInformationProtectionEnforcementLevel 枚举类型
description: WIP 保护实施级别的可能值
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5097682172281ece366a8f0389c314e2fb630190
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868367"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="9038f-103">windowsInformationProtectionEnforcementLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9038f-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="9038f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9038f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9038f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9038f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9038f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9038f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9038f-107">WIP 保护实施级别的可能值</span><span class="sxs-lookup"><span data-stu-id="9038f-107">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="9038f-108">成员</span><span class="sxs-lookup"><span data-stu-id="9038f-108">Members</span></span>
|<span data-ttu-id="9038f-109">成员</span><span class="sxs-lookup"><span data-stu-id="9038f-109">Member</span></span>|<span data-ttu-id="9038f-110">值</span><span class="sxs-lookup"><span data-stu-id="9038f-110">Value</span></span>|<span data-ttu-id="9038f-111">Description</span><span class="sxs-lookup"><span data-stu-id="9038f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9038f-112">noProtection</span><span class="sxs-lookup"><span data-stu-id="9038f-112">noProtection</span></span>|<span data-ttu-id="9038f-113">0</span><span class="sxs-lookup"><span data-stu-id="9038f-113">0</span></span>|<span data-ttu-id="9038f-114">无保护强制</span><span class="sxs-lookup"><span data-stu-id="9038f-114">No protection enforcement</span></span>|
|<span data-ttu-id="9038f-115">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="9038f-115">encryptAndAuditOnly</span></span>|<span data-ttu-id="9038f-116">1</span><span class="sxs-lookup"><span data-stu-id="9038f-116">1</span></span>|<span data-ttu-id="9038f-117">加密和仅用于审核</span><span class="sxs-lookup"><span data-stu-id="9038f-117">Encrypt and Audit only</span></span>|
|<span data-ttu-id="9038f-118">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="9038f-118">encryptAuditAndPrompt</span></span>|<span data-ttu-id="9038f-119">2</span><span class="sxs-lookup"><span data-stu-id="9038f-119">2</span></span>|<span data-ttu-id="9038f-120">加密、 审核和提示</span><span class="sxs-lookup"><span data-stu-id="9038f-120">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="9038f-121">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="9038f-121">encryptAuditAndBlock</span></span>|<span data-ttu-id="9038f-122">3</span><span class="sxs-lookup"><span data-stu-id="9038f-122">3</span></span>|<span data-ttu-id="9038f-123">加密、 审核和阻止</span><span class="sxs-lookup"><span data-stu-id="9038f-123">Encrypt, Audit and Block</span></span>|





