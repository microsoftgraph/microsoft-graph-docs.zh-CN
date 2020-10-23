---
title: deviceManagementExchangeAccessStateReason 枚举类型
description: 设备 Exchange 访问状态原因。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: cca75743a7ab4e32f4ec3d4b065756f0bae19bd6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727412"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="eabd0-103">deviceManagementExchangeAccessStateReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="eabd0-103">deviceManagementExchangeAccessStateReason enum type</span></span>

<span data-ttu-id="eabd0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eabd0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eabd0-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eabd0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eabd0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eabd0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eabd0-107">设备 Exchange 访问状态原因。</span><span class="sxs-lookup"><span data-stu-id="eabd0-107">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="eabd0-108">成员</span><span class="sxs-lookup"><span data-stu-id="eabd0-108">Members</span></span>
|<span data-ttu-id="eabd0-109">成员</span><span class="sxs-lookup"><span data-stu-id="eabd0-109">Member</span></span>|<span data-ttu-id="eabd0-110">值</span><span class="sxs-lookup"><span data-stu-id="eabd0-110">Value</span></span>|<span data-ttu-id="eabd0-111">说明</span><span class="sxs-lookup"><span data-stu-id="eabd0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eabd0-112">无</span><span class="sxs-lookup"><span data-stu-id="eabd0-112">none</span></span>|<span data-ttu-id="eabd0-113">0</span><span class="sxs-lookup"><span data-stu-id="eabd0-113">0</span></span>|<span data-ttu-id="eabd0-114">未发现来自 Exchange 的访问状态原因</span><span class="sxs-lookup"><span data-stu-id="eabd0-114">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="eabd0-115">unknown</span><span class="sxs-lookup"><span data-stu-id="eabd0-115">unknown</span></span>|<span data-ttu-id="eabd0-116">1</span><span class="sxs-lookup"><span data-stu-id="eabd0-116">1</span></span>|<span data-ttu-id="eabd0-117">未知访问状态原因</span><span class="sxs-lookup"><span data-stu-id="eabd0-117">Unknown access state reason</span></span>|
|<span data-ttu-id="eabd0-118">exchangeGlobalRule</span><span class="sxs-lookup"><span data-stu-id="eabd0-118">exchangeGlobalRule</span></span>|<span data-ttu-id="eabd0-119">双面</span><span class="sxs-lookup"><span data-stu-id="eabd0-119">2</span></span>|<span data-ttu-id="eabd0-120">由 Exchange 全局规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="eabd0-120">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="eabd0-121">exchangeIndividualRule</span><span class="sxs-lookup"><span data-stu-id="eabd0-121">exchangeIndividualRule</span></span>|<span data-ttu-id="eabd0-122">第三章</span><span class="sxs-lookup"><span data-stu-id="eabd0-122">3</span></span>|<span data-ttu-id="eabd0-123">由 Exchange 单个规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="eabd0-123">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="eabd0-124">exchangeDeviceRule</span><span class="sxs-lookup"><span data-stu-id="eabd0-124">exchangeDeviceRule</span></span>|<span data-ttu-id="eabd0-125">4 </span><span class="sxs-lookup"><span data-stu-id="eabd0-125">4</span></span>|<span data-ttu-id="eabd0-126">由 Exchange 设备规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="eabd0-126">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="eabd0-127">exchangeUpgrade</span><span class="sxs-lookup"><span data-stu-id="eabd0-127">exchangeUpgrade</span></span>|<span data-ttu-id="eabd0-128">5 </span><span class="sxs-lookup"><span data-stu-id="eabd0-128">5</span></span>|<span data-ttu-id="eabd0-129">Exchange 升级导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="eabd0-129">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="eabd0-130">exchangeMailboxPolicy</span><span class="sxs-lookup"><span data-stu-id="eabd0-130">exchangeMailboxPolicy</span></span>|<span data-ttu-id="eabd0-131">6 </span><span class="sxs-lookup"><span data-stu-id="eabd0-131">6</span></span>|<span data-ttu-id="eabd0-132">由 Exchange 邮箱策略确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="eabd0-132">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="eabd0-133">相互</span><span class="sxs-lookup"><span data-stu-id="eabd0-133">other</span></span>|<span data-ttu-id="eabd0-134">7 </span><span class="sxs-lookup"><span data-stu-id="eabd0-134">7</span></span>|<span data-ttu-id="eabd0-135">由 Exchange 确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="eabd0-135">Access state determined by Exchange</span></span>|
|<span data-ttu-id="eabd0-136">合格</span><span class="sxs-lookup"><span data-stu-id="eabd0-136">compliant</span></span>|<span data-ttu-id="eabd0-137">8 </span><span class="sxs-lookup"><span data-stu-id="eabd0-137">8</span></span>|<span data-ttu-id="eabd0-138">合规性挑战授予的访问状态</span><span class="sxs-lookup"><span data-stu-id="eabd0-138">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="eabd0-139">notCompliant</span><span class="sxs-lookup"><span data-stu-id="eabd0-139">notCompliant</span></span>|<span data-ttu-id="eabd0-140">9 </span><span class="sxs-lookup"><span data-stu-id="eabd0-140">9</span></span>|<span data-ttu-id="eabd0-141">由合规性挑战吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="eabd0-141">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="eabd0-142">notEnrolled</span><span class="sxs-lookup"><span data-stu-id="eabd0-142">notEnrolled</span></span>|<span data-ttu-id="eabd0-143">10  </span><span class="sxs-lookup"><span data-stu-id="eabd0-143">10</span></span>|<span data-ttu-id="eabd0-144">由管理质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="eabd0-144">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="eabd0-145">unknownLocation</span><span class="sxs-lookup"><span data-stu-id="eabd0-145">unknownLocation</span></span>|<span data-ttu-id="eabd0-146">12 </span><span class="sxs-lookup"><span data-stu-id="eabd0-146">12</span></span>|<span data-ttu-id="eabd0-147">由于未知位置导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="eabd0-147">Access state due to unknown location</span></span>|
|<span data-ttu-id="eabd0-148">mfaRequired</span><span class="sxs-lookup"><span data-stu-id="eabd0-148">mfaRequired</span></span>|<span data-ttu-id="eabd0-149">13 </span><span class="sxs-lookup"><span data-stu-id="eabd0-149">13</span></span>|<span data-ttu-id="eabd0-150">由于 MFA 质询而导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="eabd0-150">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="eabd0-151">azureADBlockDueToAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="eabd0-151">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="eabd0-152">14 </span><span class="sxs-lookup"><span data-stu-id="eabd0-152">14</span></span>|<span data-ttu-id="eabd0-153">由 AAD 访问策略吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="eabd0-153">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="eabd0-154">compromisedPassword</span><span class="sxs-lookup"><span data-stu-id="eabd0-154">compromisedPassword</span></span>|<span data-ttu-id="eabd0-155">15 </span><span class="sxs-lookup"><span data-stu-id="eabd0-155">15</span></span>|<span data-ttu-id="eabd0-156">通过密码被破解的密码吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="eabd0-156">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="eabd0-157">deviceNotKnownWithManagedApp</span><span class="sxs-lookup"><span data-stu-id="eabd0-157">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="eabd0-158">16 </span><span class="sxs-lookup"><span data-stu-id="eabd0-158">16</span></span>|<span data-ttu-id="eabd0-159">由托管应用程序质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="eabd0-159">Access state revoked by managed application challenge</span></span>|





