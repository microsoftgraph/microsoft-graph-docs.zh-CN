---
title: windowsInformationProtectionEnforcementLevel 枚举类型
description: WIP 保护实施级别的可能值
author: tfitzmac
ms.openlocfilehash: cb30ffb58b129fc302d7896c148072a54b98c0a2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315160"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="2b692-103">windowsInformationProtectionEnforcementLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2b692-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="2b692-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2b692-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b692-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2b692-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b692-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2b692-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b692-107">WIP 保护实施级别的可能值</span><span class="sxs-lookup"><span data-stu-id="2b692-107">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="2b692-108">成员</span><span class="sxs-lookup"><span data-stu-id="2b692-108">Members</span></span>
|<span data-ttu-id="2b692-109">成员</span><span class="sxs-lookup"><span data-stu-id="2b692-109">Member</span></span>|<span data-ttu-id="2b692-110">值</span><span class="sxs-lookup"><span data-stu-id="2b692-110">Value</span></span>|<span data-ttu-id="2b692-111">说明</span><span class="sxs-lookup"><span data-stu-id="2b692-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b692-112">noProtection</span><span class="sxs-lookup"><span data-stu-id="2b692-112">noProtection</span></span>|<span data-ttu-id="2b692-113">0</span><span class="sxs-lookup"><span data-stu-id="2b692-113">0</span></span>|<span data-ttu-id="2b692-114">无保护强制</span><span class="sxs-lookup"><span data-stu-id="2b692-114">No protection enforcement</span></span>|
|<span data-ttu-id="2b692-115">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="2b692-115">encryptAndAuditOnly</span></span>|<span data-ttu-id="2b692-116">1</span><span class="sxs-lookup"><span data-stu-id="2b692-116">1</span></span>|<span data-ttu-id="2b692-117">加密和仅用于审核</span><span class="sxs-lookup"><span data-stu-id="2b692-117">Encrypt and Audit only</span></span>|
|<span data-ttu-id="2b692-118">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="2b692-118">encryptAuditAndPrompt</span></span>|<span data-ttu-id="2b692-119">2</span><span class="sxs-lookup"><span data-stu-id="2b692-119">2</span></span>|<span data-ttu-id="2b692-120">加密、 审核和提示</span><span class="sxs-lookup"><span data-stu-id="2b692-120">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="2b692-121">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="2b692-121">encryptAuditAndBlock</span></span>|<span data-ttu-id="2b692-122">3</span><span class="sxs-lookup"><span data-stu-id="2b692-122">3</span></span>|<span data-ttu-id="2b692-123">加密、 审核和阻止</span><span class="sxs-lookup"><span data-stu-id="2b692-123">Encrypt, Audit and Block</span></span>|





