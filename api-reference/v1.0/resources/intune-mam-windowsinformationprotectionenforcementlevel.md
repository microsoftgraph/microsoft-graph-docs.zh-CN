---
title: windowsInformationProtectionEnforcementLevel 枚举类型
description: WIP 保护实施级别的可能值
ms.openlocfilehash: 5d27923c53dbae0aaeebc6bd664f0cd7f6bd9e8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011579"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="ef223-103">windowsInformationProtectionEnforcementLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ef223-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="ef223-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ef223-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef223-105">WIP 保护实施级别的可能值</span><span class="sxs-lookup"><span data-stu-id="ef223-105">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="ef223-106">成员</span><span class="sxs-lookup"><span data-stu-id="ef223-106">Members</span></span>
|<span data-ttu-id="ef223-107">成员</span><span class="sxs-lookup"><span data-stu-id="ef223-107">Member</span></span>|<span data-ttu-id="ef223-108">值</span><span class="sxs-lookup"><span data-stu-id="ef223-108">Value</span></span>|<span data-ttu-id="ef223-109">说明</span><span class="sxs-lookup"><span data-stu-id="ef223-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef223-110">noProtection</span><span class="sxs-lookup"><span data-stu-id="ef223-110">noProtection</span></span>|<span data-ttu-id="ef223-111">0</span><span class="sxs-lookup"><span data-stu-id="ef223-111">0</span></span>|<span data-ttu-id="ef223-112">无保护强制</span><span class="sxs-lookup"><span data-stu-id="ef223-112">No protection enforcement</span></span>|
|<span data-ttu-id="ef223-113">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="ef223-113">encryptAndAuditOnly</span></span>|<span data-ttu-id="ef223-114">1</span><span class="sxs-lookup"><span data-stu-id="ef223-114">1</span></span>|<span data-ttu-id="ef223-115">加密和仅用于审核</span><span class="sxs-lookup"><span data-stu-id="ef223-115">Encrypt and Audit only</span></span>|
|<span data-ttu-id="ef223-116">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="ef223-116">encryptAuditAndPrompt</span></span>|<span data-ttu-id="ef223-117">2</span><span class="sxs-lookup"><span data-stu-id="ef223-117">2</span></span>|<span data-ttu-id="ef223-118">加密、 审核和提示</span><span class="sxs-lookup"><span data-stu-id="ef223-118">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="ef223-119">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="ef223-119">encryptAuditAndBlock</span></span>|<span data-ttu-id="ef223-120">3</span><span class="sxs-lookup"><span data-stu-id="ef223-120">3</span></span>|<span data-ttu-id="ef223-121">加密、 审核和阻止</span><span class="sxs-lookup"><span data-stu-id="ef223-121">Encrypt, Audit and Block</span></span>|



