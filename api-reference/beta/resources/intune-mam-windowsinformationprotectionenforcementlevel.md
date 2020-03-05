---
title: windowsInformationProtectionEnforcementLevel 枚举类型
description: WIP 保护强制级别的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 46488043220297617dfc4eb807d94ef2a9c0ba19
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527835"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="6be09-103">windowsInformationProtectionEnforcementLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6be09-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

<span data-ttu-id="6be09-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6be09-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6be09-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6be09-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6be09-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6be09-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6be09-107">WIP 保护强制级别的可能值</span><span class="sxs-lookup"><span data-stu-id="6be09-107">Possible values for WIP Protection enforcement levels</span></span>

## <a name="members"></a><span data-ttu-id="6be09-108">成员</span><span class="sxs-lookup"><span data-stu-id="6be09-108">Members</span></span>
|<span data-ttu-id="6be09-109">成员</span><span class="sxs-lookup"><span data-stu-id="6be09-109">Member</span></span>|<span data-ttu-id="6be09-110">值</span><span class="sxs-lookup"><span data-stu-id="6be09-110">Value</span></span>|<span data-ttu-id="6be09-111">说明</span><span class="sxs-lookup"><span data-stu-id="6be09-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6be09-112">noProtection</span><span class="sxs-lookup"><span data-stu-id="6be09-112">noProtection</span></span>|<span data-ttu-id="6be09-113">0</span><span class="sxs-lookup"><span data-stu-id="6be09-113">0</span></span>|<span data-ttu-id="6be09-114">无保护强制实施</span><span class="sxs-lookup"><span data-stu-id="6be09-114">No protection enforcement</span></span>|
|<span data-ttu-id="6be09-115">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="6be09-115">encryptAndAuditOnly</span></span>|<span data-ttu-id="6be09-116">1 </span><span class="sxs-lookup"><span data-stu-id="6be09-116">1</span></span>|<span data-ttu-id="6be09-117">仅加密和审核</span><span class="sxs-lookup"><span data-stu-id="6be09-117">Encrypt and Audit only</span></span>|
|<span data-ttu-id="6be09-118">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="6be09-118">encryptAuditAndPrompt</span></span>|<span data-ttu-id="6be09-119">2 </span><span class="sxs-lookup"><span data-stu-id="6be09-119">2</span></span>|<span data-ttu-id="6be09-120">加密、审核和提示</span><span class="sxs-lookup"><span data-stu-id="6be09-120">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="6be09-121">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="6be09-121">encryptAuditAndBlock</span></span>|<span data-ttu-id="6be09-122">3 </span><span class="sxs-lookup"><span data-stu-id="6be09-122">3</span></span>|<span data-ttu-id="6be09-123">加密、审核和阻止</span><span class="sxs-lookup"><span data-stu-id="6be09-123">Encrypt, Audit and Block</span></span>|



