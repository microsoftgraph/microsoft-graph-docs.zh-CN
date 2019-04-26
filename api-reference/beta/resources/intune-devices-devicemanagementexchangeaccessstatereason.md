---
title: deviceManagementExchangeAccessStateReason 枚举类型
description: 设备 Exchange 访问状态原因。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8dab2b0b39290568331a16473fd6eaf7286ce5df
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570045"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="e5a70-103">deviceManagementExchangeAccessStateReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e5a70-103">deviceManagementExchangeAccessStateReason enum type</span></span>

> <span data-ttu-id="e5a70-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e5a70-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5a70-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e5a70-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5a70-106">设备 Exchange 访问状态原因。</span><span class="sxs-lookup"><span data-stu-id="e5a70-106">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="e5a70-107">成员</span><span class="sxs-lookup"><span data-stu-id="e5a70-107">Members</span></span>
|<span data-ttu-id="e5a70-108">成员</span><span class="sxs-lookup"><span data-stu-id="e5a70-108">Member</span></span>|<span data-ttu-id="e5a70-109">值</span><span class="sxs-lookup"><span data-stu-id="e5a70-109">Value</span></span>|<span data-ttu-id="e5a70-110">说明</span><span class="sxs-lookup"><span data-stu-id="e5a70-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5a70-111">无</span><span class="sxs-lookup"><span data-stu-id="e5a70-111">none</span></span>|<span data-ttu-id="e5a70-112">0</span><span class="sxs-lookup"><span data-stu-id="e5a70-112">0</span></span>|<span data-ttu-id="e5a70-113">未发现来自 Exchange 的访问状态原因</span><span class="sxs-lookup"><span data-stu-id="e5a70-113">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="e5a70-114">unknown</span><span class="sxs-lookup"><span data-stu-id="e5a70-114">unknown</span></span>|<span data-ttu-id="e5a70-115">1</span><span class="sxs-lookup"><span data-stu-id="e5a70-115">1</span></span>|<span data-ttu-id="e5a70-116">未知访问状态原因</span><span class="sxs-lookup"><span data-stu-id="e5a70-116">Unknown access state reason</span></span>|
|<span data-ttu-id="e5a70-117">exchangeGlobalRule</span><span class="sxs-lookup"><span data-stu-id="e5a70-117">exchangeGlobalRule</span></span>|<span data-ttu-id="e5a70-118">2 </span><span class="sxs-lookup"><span data-stu-id="e5a70-118">2</span></span>|<span data-ttu-id="e5a70-119">由 Exchange 全局规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="e5a70-119">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="e5a70-120">exchangeIndividualRule</span><span class="sxs-lookup"><span data-stu-id="e5a70-120">exchangeIndividualRule</span></span>|<span data-ttu-id="e5a70-121">3 </span><span class="sxs-lookup"><span data-stu-id="e5a70-121">3</span></span>|<span data-ttu-id="e5a70-122">由 Exchange 单个规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="e5a70-122">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="e5a70-123">exchangeDeviceRule</span><span class="sxs-lookup"><span data-stu-id="e5a70-123">exchangeDeviceRule</span></span>|<span data-ttu-id="e5a70-124">4 </span><span class="sxs-lookup"><span data-stu-id="e5a70-124">4</span></span>|<span data-ttu-id="e5a70-125">由 Exchange 设备规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="e5a70-125">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="e5a70-126">exchangeUpgrade</span><span class="sxs-lookup"><span data-stu-id="e5a70-126">exchangeUpgrade</span></span>|<span data-ttu-id="e5a70-127">5 </span><span class="sxs-lookup"><span data-stu-id="e5a70-127">5</span></span>|<span data-ttu-id="e5a70-128">Exchange 升级导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="e5a70-128">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="e5a70-129">exchangeMailboxPolicy</span><span class="sxs-lookup"><span data-stu-id="e5a70-129">exchangeMailboxPolicy</span></span>|<span data-ttu-id="e5a70-130">6 </span><span class="sxs-lookup"><span data-stu-id="e5a70-130">6</span></span>|<span data-ttu-id="e5a70-131">由 Exchange 邮箱策略确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="e5a70-131">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="e5a70-132">相互</span><span class="sxs-lookup"><span data-stu-id="e5a70-132">other</span></span>|<span data-ttu-id="e5a70-133">7 </span><span class="sxs-lookup"><span data-stu-id="e5a70-133">7</span></span>|<span data-ttu-id="e5a70-134">由 Exchange 确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="e5a70-134">Access state determined by Exchange</span></span>|
|<span data-ttu-id="e5a70-135">合格</span><span class="sxs-lookup"><span data-stu-id="e5a70-135">compliant</span></span>|<span data-ttu-id="e5a70-136">8 </span><span class="sxs-lookup"><span data-stu-id="e5a70-136">8</span></span>|<span data-ttu-id="e5a70-137">合规性挑战授予的访问状态</span><span class="sxs-lookup"><span data-stu-id="e5a70-137">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="e5a70-138">notCompliant</span><span class="sxs-lookup"><span data-stu-id="e5a70-138">notCompliant</span></span>|<span data-ttu-id="e5a70-139">9 </span><span class="sxs-lookup"><span data-stu-id="e5a70-139">9</span></span>|<span data-ttu-id="e5a70-140">由合规性挑战吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="e5a70-140">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="e5a70-141">notEnrolled</span><span class="sxs-lookup"><span data-stu-id="e5a70-141">notEnrolled</span></span>|<span data-ttu-id="e5a70-142">10 </span><span class="sxs-lookup"><span data-stu-id="e5a70-142">10</span></span>|<span data-ttu-id="e5a70-143">由管理质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="e5a70-143">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="e5a70-144">unknownLocation</span><span class="sxs-lookup"><span data-stu-id="e5a70-144">unknownLocation</span></span>|<span data-ttu-id="e5a70-145">12 </span><span class="sxs-lookup"><span data-stu-id="e5a70-145">12</span></span>|<span data-ttu-id="e5a70-146">由于未知位置导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="e5a70-146">Access state due to unknown location</span></span>|
|<span data-ttu-id="e5a70-147">mfaRequired</span><span class="sxs-lookup"><span data-stu-id="e5a70-147">mfaRequired</span></span>|<span data-ttu-id="e5a70-148">13 </span><span class="sxs-lookup"><span data-stu-id="e5a70-148">13</span></span>|<span data-ttu-id="e5a70-149">由于 MFA 质询而导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="e5a70-149">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="e5a70-150">azureADBlockDueToAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="e5a70-150">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="e5a70-151">14 </span><span class="sxs-lookup"><span data-stu-id="e5a70-151">14</span></span>|<span data-ttu-id="e5a70-152">由 AAD 访问策略吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="e5a70-152">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="e5a70-153">compromisedPassword</span><span class="sxs-lookup"><span data-stu-id="e5a70-153">compromisedPassword</span></span>|<span data-ttu-id="e5a70-154">15 </span><span class="sxs-lookup"><span data-stu-id="e5a70-154">15</span></span>|<span data-ttu-id="e5a70-155">通过密码被破解的密码吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="e5a70-155">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="e5a70-156">deviceNotKnownWithManagedApp</span><span class="sxs-lookup"><span data-stu-id="e5a70-156">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="e5a70-157">16 </span><span class="sxs-lookup"><span data-stu-id="e5a70-157">16</span></span>|<span data-ttu-id="e5a70-158">由托管应用程序质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="e5a70-158">Access state revoked by managed application challenge</span></span>|





