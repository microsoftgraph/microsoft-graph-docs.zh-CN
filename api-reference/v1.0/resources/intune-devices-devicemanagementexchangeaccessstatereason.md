---
title: deviceManagementExchangeAccessStateReason 枚举类型
description: 设备 Exchange 访问状态原因。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b0e3d5190ae946bf101ab9955cbdf9d6a4592e97
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533284"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="56a25-103">deviceManagementExchangeAccessStateReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="56a25-103">deviceManagementExchangeAccessStateReason enum type</span></span>

<span data-ttu-id="56a25-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56a25-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56a25-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56a25-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56a25-106">设备 Exchange 访问状态原因。</span><span class="sxs-lookup"><span data-stu-id="56a25-106">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="56a25-107">成员</span><span class="sxs-lookup"><span data-stu-id="56a25-107">Members</span></span>
|<span data-ttu-id="56a25-108">成员</span><span class="sxs-lookup"><span data-stu-id="56a25-108">Member</span></span>|<span data-ttu-id="56a25-109">值</span><span class="sxs-lookup"><span data-stu-id="56a25-109">Value</span></span>|<span data-ttu-id="56a25-110">说明</span><span class="sxs-lookup"><span data-stu-id="56a25-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56a25-111">无</span><span class="sxs-lookup"><span data-stu-id="56a25-111">none</span></span>|<span data-ttu-id="56a25-112">0</span><span class="sxs-lookup"><span data-stu-id="56a25-112">0</span></span>|<span data-ttu-id="56a25-113">未发现来自 Exchange 的访问状态原因</span><span class="sxs-lookup"><span data-stu-id="56a25-113">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="56a25-114">unknown</span><span class="sxs-lookup"><span data-stu-id="56a25-114">unknown</span></span>|<span data-ttu-id="56a25-115">1 </span><span class="sxs-lookup"><span data-stu-id="56a25-115">1</span></span>|<span data-ttu-id="56a25-116">未知访问状态原因</span><span class="sxs-lookup"><span data-stu-id="56a25-116">Unknown access state reason</span></span>|
|<span data-ttu-id="56a25-117">exchangeGlobalRule</span><span class="sxs-lookup"><span data-stu-id="56a25-117">exchangeGlobalRule</span></span>|<span data-ttu-id="56a25-118">2 </span><span class="sxs-lookup"><span data-stu-id="56a25-118">2</span></span>|<span data-ttu-id="56a25-119">由 Exchange 全局规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="56a25-119">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="56a25-120">exchangeIndividualRule</span><span class="sxs-lookup"><span data-stu-id="56a25-120">exchangeIndividualRule</span></span>|<span data-ttu-id="56a25-121">3 </span><span class="sxs-lookup"><span data-stu-id="56a25-121">3</span></span>|<span data-ttu-id="56a25-122">由 Exchange 单个规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="56a25-122">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="56a25-123">exchangeDeviceRule</span><span class="sxs-lookup"><span data-stu-id="56a25-123">exchangeDeviceRule</span></span>|<span data-ttu-id="56a25-124">4 </span><span class="sxs-lookup"><span data-stu-id="56a25-124">4</span></span>|<span data-ttu-id="56a25-125">由 Exchange 设备规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="56a25-125">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="56a25-126">exchangeUpgrade</span><span class="sxs-lookup"><span data-stu-id="56a25-126">exchangeUpgrade</span></span>|<span data-ttu-id="56a25-127">5 </span><span class="sxs-lookup"><span data-stu-id="56a25-127">5</span></span>|<span data-ttu-id="56a25-128">Exchange 升级导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="56a25-128">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="56a25-129">exchangeMailboxPolicy</span><span class="sxs-lookup"><span data-stu-id="56a25-129">exchangeMailboxPolicy</span></span>|<span data-ttu-id="56a25-130">6 </span><span class="sxs-lookup"><span data-stu-id="56a25-130">6</span></span>|<span data-ttu-id="56a25-131">由 Exchange 邮箱策略确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="56a25-131">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="56a25-132">相互</span><span class="sxs-lookup"><span data-stu-id="56a25-132">other</span></span>|<span data-ttu-id="56a25-133">7 </span><span class="sxs-lookup"><span data-stu-id="56a25-133">7</span></span>|<span data-ttu-id="56a25-134">由 Exchange 确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="56a25-134">Access state determined by Exchange</span></span>|
|<span data-ttu-id="56a25-135">合格</span><span class="sxs-lookup"><span data-stu-id="56a25-135">compliant</span></span>|<span data-ttu-id="56a25-136">8 </span><span class="sxs-lookup"><span data-stu-id="56a25-136">8</span></span>|<span data-ttu-id="56a25-137">合规性挑战授予的访问状态</span><span class="sxs-lookup"><span data-stu-id="56a25-137">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="56a25-138">notCompliant</span><span class="sxs-lookup"><span data-stu-id="56a25-138">notCompliant</span></span>|<span data-ttu-id="56a25-139">9 </span><span class="sxs-lookup"><span data-stu-id="56a25-139">9</span></span>|<span data-ttu-id="56a25-140">由合规性挑战吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="56a25-140">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="56a25-141">notEnrolled</span><span class="sxs-lookup"><span data-stu-id="56a25-141">notEnrolled</span></span>|<span data-ttu-id="56a25-142">10 </span><span class="sxs-lookup"><span data-stu-id="56a25-142">10</span></span>|<span data-ttu-id="56a25-143">由管理质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="56a25-143">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="56a25-144">unknownLocation</span><span class="sxs-lookup"><span data-stu-id="56a25-144">unknownLocation</span></span>|<span data-ttu-id="56a25-145">12 </span><span class="sxs-lookup"><span data-stu-id="56a25-145">12</span></span>|<span data-ttu-id="56a25-146">由于未知位置导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="56a25-146">Access state due to unknown location</span></span>|
|<span data-ttu-id="56a25-147">mfaRequired</span><span class="sxs-lookup"><span data-stu-id="56a25-147">mfaRequired</span></span>|<span data-ttu-id="56a25-148">13 </span><span class="sxs-lookup"><span data-stu-id="56a25-148">13</span></span>|<span data-ttu-id="56a25-149">由于 MFA 质询而导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="56a25-149">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="56a25-150">azureADBlockDueToAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="56a25-150">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="56a25-151">14 </span><span class="sxs-lookup"><span data-stu-id="56a25-151">14</span></span>|<span data-ttu-id="56a25-152">由 AAD 访问策略吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="56a25-152">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="56a25-153">compromisedPassword</span><span class="sxs-lookup"><span data-stu-id="56a25-153">compromisedPassword</span></span>|<span data-ttu-id="56a25-154">15 </span><span class="sxs-lookup"><span data-stu-id="56a25-154">15</span></span>|<span data-ttu-id="56a25-155">通过密码被破解的密码吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="56a25-155">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="56a25-156">deviceNotKnownWithManagedApp</span><span class="sxs-lookup"><span data-stu-id="56a25-156">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="56a25-157">16 </span><span class="sxs-lookup"><span data-stu-id="56a25-157">16</span></span>|<span data-ttu-id="56a25-158">由托管应用程序质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="56a25-158">Access state revoked by managed application challenge</span></span>|




