---
title: groupPolicySettingType 枚举类型
description: 设置组策略的类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 411b19f05c626dce8898a75139b34cdd44647860
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528126"
---
# <a name="grouppolicysettingtype-enum-type"></a><span data-ttu-id="f6d3a-103">groupPolicySettingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f6d3a-103">groupPolicySettingType enum type</span></span>

<span data-ttu-id="f6d3a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f6d3a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6d3a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f6d3a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6d3a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f6d3a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6d3a-107">设置组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="f6d3a-107">Setting type of the group policy.</span></span>

## <a name="members"></a><span data-ttu-id="f6d3a-108">成员</span><span class="sxs-lookup"><span data-stu-id="f6d3a-108">Members</span></span>
|<span data-ttu-id="f6d3a-109">成员</span><span class="sxs-lookup"><span data-stu-id="f6d3a-109">Member</span></span>|<span data-ttu-id="f6d3a-110">值</span><span class="sxs-lookup"><span data-stu-id="f6d3a-110">Value</span></span>|<span data-ttu-id="f6d3a-111">说明</span><span class="sxs-lookup"><span data-stu-id="f6d3a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6d3a-112">unknown</span><span class="sxs-lookup"><span data-stu-id="f6d3a-112">unknown</span></span>|<span data-ttu-id="f6d3a-113">0</span><span class="sxs-lookup"><span data-stu-id="f6d3a-113">0</span></span>|<span data-ttu-id="f6d3a-114">GroupPolicySettingType 未知</span><span class="sxs-lookup"><span data-stu-id="f6d3a-114">GroupPolicySettingType unknown</span></span>|
|<span data-ttu-id="f6d3a-115">policy</span><span class="sxs-lookup"><span data-stu-id="f6d3a-115">policy</span></span>|<span data-ttu-id="f6d3a-116">1 </span><span class="sxs-lookup"><span data-stu-id="f6d3a-116">1</span></span>|<span data-ttu-id="f6d3a-117">策略设置类型</span><span class="sxs-lookup"><span data-stu-id="f6d3a-117">Policy setting type</span></span>|
|<span data-ttu-id="f6d3a-118">上级</span><span class="sxs-lookup"><span data-stu-id="f6d3a-118">account</span></span>|<span data-ttu-id="f6d3a-119">2 </span><span class="sxs-lookup"><span data-stu-id="f6d3a-119">2</span></span>|<span data-ttu-id="f6d3a-120">帐户设置类型</span><span class="sxs-lookup"><span data-stu-id="f6d3a-120">Account setting type</span></span>|
|<span data-ttu-id="f6d3a-121">securityOptions</span><span class="sxs-lookup"><span data-stu-id="f6d3a-121">securityOptions</span></span>|<span data-ttu-id="f6d3a-122">3 </span><span class="sxs-lookup"><span data-stu-id="f6d3a-122">3</span></span>|<span data-ttu-id="f6d3a-123">SecurityOptions 设置类型</span><span class="sxs-lookup"><span data-stu-id="f6d3a-123">SecurityOptions setting type</span></span>|
|<span data-ttu-id="f6d3a-124">userRightsAssignment</span><span class="sxs-lookup"><span data-stu-id="f6d3a-124">userRightsAssignment</span></span>|<span data-ttu-id="f6d3a-125">4 </span><span class="sxs-lookup"><span data-stu-id="f6d3a-125">4</span></span>|<span data-ttu-id="f6d3a-126">UserRightsAssignment 设置类型</span><span class="sxs-lookup"><span data-stu-id="f6d3a-126">UserRightsAssignment setting type</span></span>|
|<span data-ttu-id="f6d3a-127">auditSetting</span><span class="sxs-lookup"><span data-stu-id="f6d3a-127">auditSetting</span></span>|<span data-ttu-id="f6d3a-128">5 </span><span class="sxs-lookup"><span data-stu-id="f6d3a-128">5</span></span>|<span data-ttu-id="f6d3a-129">AuditSetting 设置类型</span><span class="sxs-lookup"><span data-stu-id="f6d3a-129">AuditSetting setting type</span></span>|
|<span data-ttu-id="f6d3a-130">windowsFirewallSettings</span><span class="sxs-lookup"><span data-stu-id="f6d3a-130">windowsFirewallSettings</span></span>|<span data-ttu-id="f6d3a-131">6 </span><span class="sxs-lookup"><span data-stu-id="f6d3a-131">6</span></span>|<span data-ttu-id="f6d3a-132">WindowsFirewallSettings 设置类型</span><span class="sxs-lookup"><span data-stu-id="f6d3a-132">WindowsFirewallSettings setting type</span></span>|



