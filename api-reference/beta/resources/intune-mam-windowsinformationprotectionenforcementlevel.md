---
title: windowsInformationProtectionEnforcementLevel 枚举类型
description: WIP 保护实施级别的可能值
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 37ec9c781ea4a804260f7dff7b6586c042dcad48
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417670"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="b4348-103">windowsInformationProtectionEnforcementLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b4348-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="b4348-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b4348-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b4348-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b4348-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4348-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b4348-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4348-107">WIP 保护实施级别的可能值</span><span class="sxs-lookup"><span data-stu-id="b4348-107">Possible values for WIP Protection enforcement levels</span></span>

## <a name="members"></a><span data-ttu-id="b4348-108">成员</span><span class="sxs-lookup"><span data-stu-id="b4348-108">Members</span></span>
|<span data-ttu-id="b4348-109">成员</span><span class="sxs-lookup"><span data-stu-id="b4348-109">Member</span></span>|<span data-ttu-id="b4348-110">值</span><span class="sxs-lookup"><span data-stu-id="b4348-110">Value</span></span>|<span data-ttu-id="b4348-111">说明</span><span class="sxs-lookup"><span data-stu-id="b4348-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4348-112">noProtection</span><span class="sxs-lookup"><span data-stu-id="b4348-112">noProtection</span></span>|<span data-ttu-id="b4348-113">0</span><span class="sxs-lookup"><span data-stu-id="b4348-113">0</span></span>|<span data-ttu-id="b4348-114">无保护强制</span><span class="sxs-lookup"><span data-stu-id="b4348-114">No protection enforcement</span></span>|
|<span data-ttu-id="b4348-115">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="b4348-115">encryptAndAuditOnly</span></span>|<span data-ttu-id="b4348-116">1</span><span class="sxs-lookup"><span data-stu-id="b4348-116">1</span></span>|<span data-ttu-id="b4348-117">加密和仅用于审核</span><span class="sxs-lookup"><span data-stu-id="b4348-117">Encrypt and Audit only</span></span>|
|<span data-ttu-id="b4348-118">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="b4348-118">encryptAuditAndPrompt</span></span>|<span data-ttu-id="b4348-119">2</span><span class="sxs-lookup"><span data-stu-id="b4348-119">2</span></span>|<span data-ttu-id="b4348-120">加密、 审核和提示</span><span class="sxs-lookup"><span data-stu-id="b4348-120">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="b4348-121">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="b4348-121">encryptAuditAndBlock</span></span>|<span data-ttu-id="b4348-122">3</span><span class="sxs-lookup"><span data-stu-id="b4348-122">3</span></span>|<span data-ttu-id="b4348-123">加密、 审核和阻止</span><span class="sxs-lookup"><span data-stu-id="b4348-123">Encrypt, Audit and Block</span></span>|




