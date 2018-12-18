---
title: windowsInformationProtectionEnforcementLevel 枚举类型
description: WIP 保护实施级别的可能值
author: tfitzmac
ms.openlocfilehash: 84f60f0e4f59206d420219e8547160c85202f9cf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313263"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="e8dd8-103">windowsInformationProtectionEnforcementLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e8dd8-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="e8dd8-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e8dd8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8dd8-105">WIP 保护实施级别的可能值</span><span class="sxs-lookup"><span data-stu-id="e8dd8-105">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="e8dd8-106">成员</span><span class="sxs-lookup"><span data-stu-id="e8dd8-106">Members</span></span>
|<span data-ttu-id="e8dd8-107">成员</span><span class="sxs-lookup"><span data-stu-id="e8dd8-107">Member</span></span>|<span data-ttu-id="e8dd8-108">值</span><span class="sxs-lookup"><span data-stu-id="e8dd8-108">Value</span></span>|<span data-ttu-id="e8dd8-109">说明</span><span class="sxs-lookup"><span data-stu-id="e8dd8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8dd8-110">noProtection</span><span class="sxs-lookup"><span data-stu-id="e8dd8-110">noProtection</span></span>|<span data-ttu-id="e8dd8-111">0</span><span class="sxs-lookup"><span data-stu-id="e8dd8-111">0</span></span>|<span data-ttu-id="e8dd8-112">无保护强制</span><span class="sxs-lookup"><span data-stu-id="e8dd8-112">No protection enforcement</span></span>|
|<span data-ttu-id="e8dd8-113">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="e8dd8-113">encryptAndAuditOnly</span></span>|<span data-ttu-id="e8dd8-114">1</span><span class="sxs-lookup"><span data-stu-id="e8dd8-114">1</span></span>|<span data-ttu-id="e8dd8-115">加密和仅用于审核</span><span class="sxs-lookup"><span data-stu-id="e8dd8-115">Encrypt and Audit only</span></span>|
|<span data-ttu-id="e8dd8-116">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="e8dd8-116">encryptAuditAndPrompt</span></span>|<span data-ttu-id="e8dd8-117">2</span><span class="sxs-lookup"><span data-stu-id="e8dd8-117">2</span></span>|<span data-ttu-id="e8dd8-118">加密、 审核和提示</span><span class="sxs-lookup"><span data-stu-id="e8dd8-118">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="e8dd8-119">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="e8dd8-119">encryptAuditAndBlock</span></span>|<span data-ttu-id="e8dd8-120">3</span><span class="sxs-lookup"><span data-stu-id="e8dd8-120">3</span></span>|<span data-ttu-id="e8dd8-121">加密、 审核和阻止</span><span class="sxs-lookup"><span data-stu-id="e8dd8-121">Encrypt, Audit and Block</span></span>|



