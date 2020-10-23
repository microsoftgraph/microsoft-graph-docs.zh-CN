---
title: groupPolicySettingType 枚举类型
description: 设置组策略的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a6bd8424d4142271bb8e364fb64f1bf0c23557b4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697453"
---
# <a name="grouppolicysettingtype-enum-type"></a><span data-ttu-id="6ec2f-103">groupPolicySettingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6ec2f-103">groupPolicySettingType enum type</span></span>

<span data-ttu-id="6ec2f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ec2f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ec2f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6ec2f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ec2f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6ec2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ec2f-107">设置组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="6ec2f-107">Setting type of the group policy.</span></span>

## <a name="members"></a><span data-ttu-id="6ec2f-108">成员</span><span class="sxs-lookup"><span data-stu-id="6ec2f-108">Members</span></span>
|<span data-ttu-id="6ec2f-109">成员</span><span class="sxs-lookup"><span data-stu-id="6ec2f-109">Member</span></span>|<span data-ttu-id="6ec2f-110">值</span><span class="sxs-lookup"><span data-stu-id="6ec2f-110">Value</span></span>|<span data-ttu-id="6ec2f-111">说明</span><span class="sxs-lookup"><span data-stu-id="6ec2f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ec2f-112">unknown</span><span class="sxs-lookup"><span data-stu-id="6ec2f-112">unknown</span></span>|<span data-ttu-id="6ec2f-113">0</span><span class="sxs-lookup"><span data-stu-id="6ec2f-113">0</span></span>|<span data-ttu-id="6ec2f-114">GroupPolicySettingType 未知</span><span class="sxs-lookup"><span data-stu-id="6ec2f-114">GroupPolicySettingType unknown</span></span>|
|<span data-ttu-id="6ec2f-115">策略</span><span class="sxs-lookup"><span data-stu-id="6ec2f-115">policy</span></span>|<span data-ttu-id="6ec2f-116">1</span><span class="sxs-lookup"><span data-stu-id="6ec2f-116">1</span></span>|<span data-ttu-id="6ec2f-117">策略设置类型</span><span class="sxs-lookup"><span data-stu-id="6ec2f-117">Policy setting type</span></span>|
|<span data-ttu-id="6ec2f-118">上级</span><span class="sxs-lookup"><span data-stu-id="6ec2f-118">account</span></span>|<span data-ttu-id="6ec2f-119">双面</span><span class="sxs-lookup"><span data-stu-id="6ec2f-119">2</span></span>|<span data-ttu-id="6ec2f-120">帐户设置类型</span><span class="sxs-lookup"><span data-stu-id="6ec2f-120">Account setting type</span></span>|
|<span data-ttu-id="6ec2f-121">securityOptions</span><span class="sxs-lookup"><span data-stu-id="6ec2f-121">securityOptions</span></span>|<span data-ttu-id="6ec2f-122">第三章</span><span class="sxs-lookup"><span data-stu-id="6ec2f-122">3</span></span>|<span data-ttu-id="6ec2f-123">SecurityOptions 设置类型</span><span class="sxs-lookup"><span data-stu-id="6ec2f-123">SecurityOptions setting type</span></span>|
|<span data-ttu-id="6ec2f-124">userRightsAssignment</span><span class="sxs-lookup"><span data-stu-id="6ec2f-124">userRightsAssignment</span></span>|<span data-ttu-id="6ec2f-125">4 </span><span class="sxs-lookup"><span data-stu-id="6ec2f-125">4</span></span>|<span data-ttu-id="6ec2f-126">UserRightsAssignment 设置类型</span><span class="sxs-lookup"><span data-stu-id="6ec2f-126">UserRightsAssignment setting type</span></span>|
|<span data-ttu-id="6ec2f-127">auditSetting</span><span class="sxs-lookup"><span data-stu-id="6ec2f-127">auditSetting</span></span>|<span data-ttu-id="6ec2f-128">5 </span><span class="sxs-lookup"><span data-stu-id="6ec2f-128">5</span></span>|<span data-ttu-id="6ec2f-129">AuditSetting 设置类型</span><span class="sxs-lookup"><span data-stu-id="6ec2f-129">AuditSetting setting type</span></span>|
|<span data-ttu-id="6ec2f-130">windowsFirewallSettings</span><span class="sxs-lookup"><span data-stu-id="6ec2f-130">windowsFirewallSettings</span></span>|<span data-ttu-id="6ec2f-131">6 </span><span class="sxs-lookup"><span data-stu-id="6ec2f-131">6</span></span>|<span data-ttu-id="6ec2f-132">WindowsFirewallSettings 设置类型</span><span class="sxs-lookup"><span data-stu-id="6ec2f-132">WindowsFirewallSettings setting type</span></span>|





