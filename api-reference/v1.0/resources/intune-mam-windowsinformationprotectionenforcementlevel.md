---
title: windowsInformationProtectionEnforcementLevel 枚举类型
description: WIP 保护实施级别的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4661c80655defe85f27ac8259a961955552f7021
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964170"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="bd663-103">windowsInformationProtectionEnforcementLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="bd663-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="bd663-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bd663-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd663-105">WIP 保护实施级别的可能值</span><span class="sxs-lookup"><span data-stu-id="bd663-105">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="bd663-106">成员</span><span class="sxs-lookup"><span data-stu-id="bd663-106">Members</span></span>
|<span data-ttu-id="bd663-107">成员</span><span class="sxs-lookup"><span data-stu-id="bd663-107">Member</span></span>|<span data-ttu-id="bd663-108">值</span><span class="sxs-lookup"><span data-stu-id="bd663-108">Value</span></span>|<span data-ttu-id="bd663-109">Description</span><span class="sxs-lookup"><span data-stu-id="bd663-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd663-110">noProtection</span><span class="sxs-lookup"><span data-stu-id="bd663-110">noProtection</span></span>|<span data-ttu-id="bd663-111">0</span><span class="sxs-lookup"><span data-stu-id="bd663-111">0</span></span>|<span data-ttu-id="bd663-112">无保护强制</span><span class="sxs-lookup"><span data-stu-id="bd663-112">No protection enforcement</span></span>|
|<span data-ttu-id="bd663-113">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="bd663-113">encryptAndAuditOnly</span></span>|<span data-ttu-id="bd663-114">1</span><span class="sxs-lookup"><span data-stu-id="bd663-114">1</span></span>|<span data-ttu-id="bd663-115">加密和仅用于审核</span><span class="sxs-lookup"><span data-stu-id="bd663-115">Encrypt and Audit only</span></span>|
|<span data-ttu-id="bd663-116">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="bd663-116">encryptAuditAndPrompt</span></span>|<span data-ttu-id="bd663-117">2</span><span class="sxs-lookup"><span data-stu-id="bd663-117">2</span></span>|<span data-ttu-id="bd663-118">加密、 审核和提示</span><span class="sxs-lookup"><span data-stu-id="bd663-118">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="bd663-119">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="bd663-119">encryptAuditAndBlock</span></span>|<span data-ttu-id="bd663-120">3</span><span class="sxs-lookup"><span data-stu-id="bd663-120">3</span></span>|<span data-ttu-id="bd663-121">加密、 审核和阻止</span><span class="sxs-lookup"><span data-stu-id="bd663-121">Encrypt, Audit and Block</span></span>|



