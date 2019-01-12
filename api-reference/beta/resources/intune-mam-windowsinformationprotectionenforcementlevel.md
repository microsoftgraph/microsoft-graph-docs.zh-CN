---
title: windowsInformationProtectionEnforcementLevel 枚举类型
description: WIP 保护实施级别的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ed087465d05ba91bcdc1f8cff7fec0aba567420a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913406"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="abddb-103">windowsInformationProtectionEnforcementLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="abddb-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="abddb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="abddb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abddb-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="abddb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="abddb-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="abddb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abddb-107">WIP 保护实施级别的可能值</span><span class="sxs-lookup"><span data-stu-id="abddb-107">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="abddb-108">成员</span><span class="sxs-lookup"><span data-stu-id="abddb-108">Members</span></span>
|<span data-ttu-id="abddb-109">成员</span><span class="sxs-lookup"><span data-stu-id="abddb-109">Member</span></span>|<span data-ttu-id="abddb-110">值</span><span class="sxs-lookup"><span data-stu-id="abddb-110">Value</span></span>|<span data-ttu-id="abddb-111">Description</span><span class="sxs-lookup"><span data-stu-id="abddb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abddb-112">noProtection</span><span class="sxs-lookup"><span data-stu-id="abddb-112">noProtection</span></span>|<span data-ttu-id="abddb-113">0</span><span class="sxs-lookup"><span data-stu-id="abddb-113">0</span></span>|<span data-ttu-id="abddb-114">无保护强制</span><span class="sxs-lookup"><span data-stu-id="abddb-114">No protection enforcement</span></span>|
|<span data-ttu-id="abddb-115">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="abddb-115">encryptAndAuditOnly</span></span>|<span data-ttu-id="abddb-116">1</span><span class="sxs-lookup"><span data-stu-id="abddb-116">1</span></span>|<span data-ttu-id="abddb-117">加密和仅用于审核</span><span class="sxs-lookup"><span data-stu-id="abddb-117">Encrypt and Audit only</span></span>|
|<span data-ttu-id="abddb-118">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="abddb-118">encryptAuditAndPrompt</span></span>|<span data-ttu-id="abddb-119">2</span><span class="sxs-lookup"><span data-stu-id="abddb-119">2</span></span>|<span data-ttu-id="abddb-120">加密、 审核和提示</span><span class="sxs-lookup"><span data-stu-id="abddb-120">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="abddb-121">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="abddb-121">encryptAuditAndBlock</span></span>|<span data-ttu-id="abddb-122">3</span><span class="sxs-lookup"><span data-stu-id="abddb-122">3</span></span>|<span data-ttu-id="abddb-123">加密、 审核和阻止</span><span class="sxs-lookup"><span data-stu-id="abddb-123">Encrypt, Audit and Block</span></span>|





