---
title: deviceManagementExchangeAccessStateReason 枚举类型
description: 设备 Exchange 访问状态原因。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ecd0e44a03a894ef21dfd35a97ac4f1bc272705
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942099"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="04f2e-103">deviceManagementExchangeAccessStateReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="04f2e-103">deviceManagementExchangeAccessStateReason enum type</span></span>

> <span data-ttu-id="04f2e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="04f2e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04f2e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="04f2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04f2e-106">设备 Exchange 访问状态原因。</span><span class="sxs-lookup"><span data-stu-id="04f2e-106">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="04f2e-107">成员</span><span class="sxs-lookup"><span data-stu-id="04f2e-107">Members</span></span>
|<span data-ttu-id="04f2e-108">成员</span><span class="sxs-lookup"><span data-stu-id="04f2e-108">Member</span></span>|<span data-ttu-id="04f2e-109">值</span><span class="sxs-lookup"><span data-stu-id="04f2e-109">Value</span></span>|<span data-ttu-id="04f2e-110">说明</span><span class="sxs-lookup"><span data-stu-id="04f2e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04f2e-111">无</span><span class="sxs-lookup"><span data-stu-id="04f2e-111">none</span></span>|<span data-ttu-id="04f2e-112">0</span><span class="sxs-lookup"><span data-stu-id="04f2e-112">0</span></span>|<span data-ttu-id="04f2e-113">未发现来自 Exchange 的访问状态原因</span><span class="sxs-lookup"><span data-stu-id="04f2e-113">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="04f2e-114">unknown</span><span class="sxs-lookup"><span data-stu-id="04f2e-114">unknown</span></span>|<span data-ttu-id="04f2e-115">1</span><span class="sxs-lookup"><span data-stu-id="04f2e-115">1</span></span>|<span data-ttu-id="04f2e-116">未知访问状态原因</span><span class="sxs-lookup"><span data-stu-id="04f2e-116">Unknown access state reason</span></span>|
|<span data-ttu-id="04f2e-117">exchangeGlobalRule</span><span class="sxs-lookup"><span data-stu-id="04f2e-117">exchangeGlobalRule</span></span>|<span data-ttu-id="04f2e-118">双面</span><span class="sxs-lookup"><span data-stu-id="04f2e-118">2</span></span>|<span data-ttu-id="04f2e-119">由 Exchange 全局规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="04f2e-119">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="04f2e-120">exchangeIndividualRule</span><span class="sxs-lookup"><span data-stu-id="04f2e-120">exchangeIndividualRule</span></span>|<span data-ttu-id="04f2e-121">第三章</span><span class="sxs-lookup"><span data-stu-id="04f2e-121">3</span></span>|<span data-ttu-id="04f2e-122">由 Exchange 单个规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="04f2e-122">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="04f2e-123">exchangeDeviceRule</span><span class="sxs-lookup"><span data-stu-id="04f2e-123">exchangeDeviceRule</span></span>|<span data-ttu-id="04f2e-124">4</span><span class="sxs-lookup"><span data-stu-id="04f2e-124">4</span></span>|<span data-ttu-id="04f2e-125">由 Exchange 设备规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="04f2e-125">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="04f2e-126">exchangeUpgrade</span><span class="sxs-lookup"><span data-stu-id="04f2e-126">exchangeUpgrade</span></span>|<span data-ttu-id="04f2e-127">5</span><span class="sxs-lookup"><span data-stu-id="04f2e-127">5</span></span>|<span data-ttu-id="04f2e-128">Exchange 升级导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="04f2e-128">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="04f2e-129">exchangeMailboxPolicy</span><span class="sxs-lookup"><span data-stu-id="04f2e-129">exchangeMailboxPolicy</span></span>|<span data-ttu-id="04f2e-130">型</span><span class="sxs-lookup"><span data-stu-id="04f2e-130">6</span></span>|<span data-ttu-id="04f2e-131">由 Exchange 邮箱策略确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="04f2e-131">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="04f2e-132">相互</span><span class="sxs-lookup"><span data-stu-id="04f2e-132">other</span></span>|<span data-ttu-id="04f2e-133">步</span><span class="sxs-lookup"><span data-stu-id="04f2e-133">7</span></span>|<span data-ttu-id="04f2e-134">由 Exchange 确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="04f2e-134">Access state determined by Exchange</span></span>|
|<span data-ttu-id="04f2e-135">合格</span><span class="sxs-lookup"><span data-stu-id="04f2e-135">compliant</span></span>|<span data-ttu-id="04f2e-136">utf-8</span><span class="sxs-lookup"><span data-stu-id="04f2e-136">8</span></span>|<span data-ttu-id="04f2e-137">合规性挑战授予的访问状态</span><span class="sxs-lookup"><span data-stu-id="04f2e-137">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="04f2e-138">notCompliant</span><span class="sxs-lookup"><span data-stu-id="04f2e-138">notCompliant</span></span>|<span data-ttu-id="04f2e-139">第</span><span class="sxs-lookup"><span data-stu-id="04f2e-139">9</span></span>|<span data-ttu-id="04f2e-140">由合规性挑战吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="04f2e-140">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="04f2e-141">notEnrolled</span><span class="sxs-lookup"><span data-stu-id="04f2e-141">notEnrolled</span></span>|<span data-ttu-id="04f2e-142">10 </span><span class="sxs-lookup"><span data-stu-id="04f2e-142">10</span></span>|<span data-ttu-id="04f2e-143">由管理质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="04f2e-143">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="04f2e-144">unknownLocation</span><span class="sxs-lookup"><span data-stu-id="04f2e-144">unknownLocation</span></span>|<span data-ttu-id="04f2e-145">12</span><span class="sxs-lookup"><span data-stu-id="04f2e-145">12</span></span>|<span data-ttu-id="04f2e-146">由于未知位置导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="04f2e-146">Access state due to unknown location</span></span>|
|<span data-ttu-id="04f2e-147">mfaRequired</span><span class="sxs-lookup"><span data-stu-id="04f2e-147">mfaRequired</span></span>|<span data-ttu-id="04f2e-148">13</span><span class="sxs-lookup"><span data-stu-id="04f2e-148">13</span></span>|<span data-ttu-id="04f2e-149">由于 MFA 质询而导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="04f2e-149">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="04f2e-150">azureADBlockDueToAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="04f2e-150">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="04f2e-151">日</span><span class="sxs-lookup"><span data-stu-id="04f2e-151">14</span></span>|<span data-ttu-id="04f2e-152">由 AAD 访问策略吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="04f2e-152">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="04f2e-153">compromisedPassword</span><span class="sxs-lookup"><span data-stu-id="04f2e-153">compromisedPassword</span></span>|<span data-ttu-id="04f2e-154">个</span><span class="sxs-lookup"><span data-stu-id="04f2e-154">15</span></span>|<span data-ttu-id="04f2e-155">通过密码被破解的密码吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="04f2e-155">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="04f2e-156">deviceNotKnownWithManagedApp</span><span class="sxs-lookup"><span data-stu-id="04f2e-156">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="04f2e-157">位</span><span class="sxs-lookup"><span data-stu-id="04f2e-157">16</span></span>|<span data-ttu-id="04f2e-158">由托管应用程序质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="04f2e-158">Access state revoked by managed application challenge</span></span>|




