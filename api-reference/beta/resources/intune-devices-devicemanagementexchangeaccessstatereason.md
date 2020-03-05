---
title: deviceManagementExchangeAccessStateReason 枚举类型
description: 设备 Exchange 访问状态原因。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: db63de7180ae6716263f958ef43a7cb2e3f299e2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525066"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="fded1-103">deviceManagementExchangeAccessStateReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fded1-103">deviceManagementExchangeAccessStateReason enum type</span></span>

<span data-ttu-id="fded1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="fded1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fded1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fded1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fded1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fded1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fded1-107">设备 Exchange 访问状态原因。</span><span class="sxs-lookup"><span data-stu-id="fded1-107">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="fded1-108">成员</span><span class="sxs-lookup"><span data-stu-id="fded1-108">Members</span></span>
|<span data-ttu-id="fded1-109">成员</span><span class="sxs-lookup"><span data-stu-id="fded1-109">Member</span></span>|<span data-ttu-id="fded1-110">值</span><span class="sxs-lookup"><span data-stu-id="fded1-110">Value</span></span>|<span data-ttu-id="fded1-111">说明</span><span class="sxs-lookup"><span data-stu-id="fded1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fded1-112">无</span><span class="sxs-lookup"><span data-stu-id="fded1-112">none</span></span>|<span data-ttu-id="fded1-113">0</span><span class="sxs-lookup"><span data-stu-id="fded1-113">0</span></span>|<span data-ttu-id="fded1-114">未发现来自 Exchange 的访问状态原因</span><span class="sxs-lookup"><span data-stu-id="fded1-114">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="fded1-115">unknown</span><span class="sxs-lookup"><span data-stu-id="fded1-115">unknown</span></span>|<span data-ttu-id="fded1-116">1 </span><span class="sxs-lookup"><span data-stu-id="fded1-116">1</span></span>|<span data-ttu-id="fded1-117">未知访问状态原因</span><span class="sxs-lookup"><span data-stu-id="fded1-117">Unknown access state reason</span></span>|
|<span data-ttu-id="fded1-118">exchangeGlobalRule</span><span class="sxs-lookup"><span data-stu-id="fded1-118">exchangeGlobalRule</span></span>|<span data-ttu-id="fded1-119">2 </span><span class="sxs-lookup"><span data-stu-id="fded1-119">2</span></span>|<span data-ttu-id="fded1-120">由 Exchange 全局规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="fded1-120">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="fded1-121">exchangeIndividualRule</span><span class="sxs-lookup"><span data-stu-id="fded1-121">exchangeIndividualRule</span></span>|<span data-ttu-id="fded1-122">3 </span><span class="sxs-lookup"><span data-stu-id="fded1-122">3</span></span>|<span data-ttu-id="fded1-123">由 Exchange 单个规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="fded1-123">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="fded1-124">exchangeDeviceRule</span><span class="sxs-lookup"><span data-stu-id="fded1-124">exchangeDeviceRule</span></span>|<span data-ttu-id="fded1-125">4 </span><span class="sxs-lookup"><span data-stu-id="fded1-125">4</span></span>|<span data-ttu-id="fded1-126">由 Exchange 设备规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="fded1-126">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="fded1-127">exchangeUpgrade</span><span class="sxs-lookup"><span data-stu-id="fded1-127">exchangeUpgrade</span></span>|<span data-ttu-id="fded1-128">5 </span><span class="sxs-lookup"><span data-stu-id="fded1-128">5</span></span>|<span data-ttu-id="fded1-129">Exchange 升级导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="fded1-129">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="fded1-130">exchangeMailboxPolicy</span><span class="sxs-lookup"><span data-stu-id="fded1-130">exchangeMailboxPolicy</span></span>|<span data-ttu-id="fded1-131">6 </span><span class="sxs-lookup"><span data-stu-id="fded1-131">6</span></span>|<span data-ttu-id="fded1-132">由 Exchange 邮箱策略确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="fded1-132">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="fded1-133">相互</span><span class="sxs-lookup"><span data-stu-id="fded1-133">other</span></span>|<span data-ttu-id="fded1-134">7 </span><span class="sxs-lookup"><span data-stu-id="fded1-134">7</span></span>|<span data-ttu-id="fded1-135">由 Exchange 确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="fded1-135">Access state determined by Exchange</span></span>|
|<span data-ttu-id="fded1-136">合格</span><span class="sxs-lookup"><span data-stu-id="fded1-136">compliant</span></span>|<span data-ttu-id="fded1-137">8 </span><span class="sxs-lookup"><span data-stu-id="fded1-137">8</span></span>|<span data-ttu-id="fded1-138">合规性挑战授予的访问状态</span><span class="sxs-lookup"><span data-stu-id="fded1-138">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="fded1-139">notCompliant</span><span class="sxs-lookup"><span data-stu-id="fded1-139">notCompliant</span></span>|<span data-ttu-id="fded1-140">9 </span><span class="sxs-lookup"><span data-stu-id="fded1-140">9</span></span>|<span data-ttu-id="fded1-141">由合规性挑战吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="fded1-141">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="fded1-142">notEnrolled</span><span class="sxs-lookup"><span data-stu-id="fded1-142">notEnrolled</span></span>|<span data-ttu-id="fded1-143">10 </span><span class="sxs-lookup"><span data-stu-id="fded1-143">10</span></span>|<span data-ttu-id="fded1-144">由管理质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="fded1-144">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="fded1-145">unknownLocation</span><span class="sxs-lookup"><span data-stu-id="fded1-145">unknownLocation</span></span>|<span data-ttu-id="fded1-146">12 </span><span class="sxs-lookup"><span data-stu-id="fded1-146">12</span></span>|<span data-ttu-id="fded1-147">由于未知位置导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="fded1-147">Access state due to unknown location</span></span>|
|<span data-ttu-id="fded1-148">mfaRequired</span><span class="sxs-lookup"><span data-stu-id="fded1-148">mfaRequired</span></span>|<span data-ttu-id="fded1-149">13 </span><span class="sxs-lookup"><span data-stu-id="fded1-149">13</span></span>|<span data-ttu-id="fded1-150">由于 MFA 质询而导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="fded1-150">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="fded1-151">azureADBlockDueToAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="fded1-151">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="fded1-152">14 </span><span class="sxs-lookup"><span data-stu-id="fded1-152">14</span></span>|<span data-ttu-id="fded1-153">由 AAD 访问策略吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="fded1-153">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="fded1-154">compromisedPassword</span><span class="sxs-lookup"><span data-stu-id="fded1-154">compromisedPassword</span></span>|<span data-ttu-id="fded1-155">15 </span><span class="sxs-lookup"><span data-stu-id="fded1-155">15</span></span>|<span data-ttu-id="fded1-156">通过密码被破解的密码吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="fded1-156">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="fded1-157">deviceNotKnownWithManagedApp</span><span class="sxs-lookup"><span data-stu-id="fded1-157">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="fded1-158">16 </span><span class="sxs-lookup"><span data-stu-id="fded1-158">16</span></span>|<span data-ttu-id="fded1-159">由托管应用程序质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="fded1-159">Access state revoked by managed application challenge</span></span>|



