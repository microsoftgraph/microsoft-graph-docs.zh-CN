---
title: deviceManagementExchangeAccessStateReason 枚举类型
description: 设备 Exchange 访问状态原因。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 37ce7d40ef2f8ea6cc729b25bcfc9b66480fdf6a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091171"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="45f36-103">deviceManagementExchangeAccessStateReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="45f36-103">deviceManagementExchangeAccessStateReason enum type</span></span>

<span data-ttu-id="45f36-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45f36-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45f36-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="45f36-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45f36-106">设备 Exchange 访问状态原因。</span><span class="sxs-lookup"><span data-stu-id="45f36-106">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="45f36-107">成员</span><span class="sxs-lookup"><span data-stu-id="45f36-107">Members</span></span>
|<span data-ttu-id="45f36-108">成员</span><span class="sxs-lookup"><span data-stu-id="45f36-108">Member</span></span>|<span data-ttu-id="45f36-109">值</span><span class="sxs-lookup"><span data-stu-id="45f36-109">Value</span></span>|<span data-ttu-id="45f36-110">说明</span><span class="sxs-lookup"><span data-stu-id="45f36-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45f36-111">无</span><span class="sxs-lookup"><span data-stu-id="45f36-111">none</span></span>|<span data-ttu-id="45f36-112">0</span><span class="sxs-lookup"><span data-stu-id="45f36-112">0</span></span>|<span data-ttu-id="45f36-113">未发现来自 Exchange 的访问状态原因</span><span class="sxs-lookup"><span data-stu-id="45f36-113">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="45f36-114">unknown</span><span class="sxs-lookup"><span data-stu-id="45f36-114">unknown</span></span>|<span data-ttu-id="45f36-115">1 </span><span class="sxs-lookup"><span data-stu-id="45f36-115">1</span></span>|<span data-ttu-id="45f36-116">未知访问状态原因</span><span class="sxs-lookup"><span data-stu-id="45f36-116">Unknown access state reason</span></span>|
|<span data-ttu-id="45f36-117">exchangeGlobalRule</span><span class="sxs-lookup"><span data-stu-id="45f36-117">exchangeGlobalRule</span></span>|<span data-ttu-id="45f36-118">2 </span><span class="sxs-lookup"><span data-stu-id="45f36-118">2</span></span>|<span data-ttu-id="45f36-119">由 Exchange 全局规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="45f36-119">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="45f36-120">exchangeIndividualRule</span><span class="sxs-lookup"><span data-stu-id="45f36-120">exchangeIndividualRule</span></span>|<span data-ttu-id="45f36-121">第三章</span><span class="sxs-lookup"><span data-stu-id="45f36-121">3</span></span>|<span data-ttu-id="45f36-122">由 Exchange 单个规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="45f36-122">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="45f36-123">exchangeDeviceRule</span><span class="sxs-lookup"><span data-stu-id="45f36-123">exchangeDeviceRule</span></span>|<span data-ttu-id="45f36-124">4 </span><span class="sxs-lookup"><span data-stu-id="45f36-124">4</span></span>|<span data-ttu-id="45f36-125">由 Exchange 设备规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="45f36-125">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="45f36-126">exchangeUpgrade</span><span class="sxs-lookup"><span data-stu-id="45f36-126">exchangeUpgrade</span></span>|<span data-ttu-id="45f36-127">5 </span><span class="sxs-lookup"><span data-stu-id="45f36-127">5</span></span>|<span data-ttu-id="45f36-128">Exchange 升级导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="45f36-128">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="45f36-129">exchangeMailboxPolicy</span><span class="sxs-lookup"><span data-stu-id="45f36-129">exchangeMailboxPolicy</span></span>|<span data-ttu-id="45f36-130">6 </span><span class="sxs-lookup"><span data-stu-id="45f36-130">6</span></span>|<span data-ttu-id="45f36-131">由 Exchange 邮箱策略确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="45f36-131">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="45f36-132">相互</span><span class="sxs-lookup"><span data-stu-id="45f36-132">other</span></span>|<span data-ttu-id="45f36-133">7 </span><span class="sxs-lookup"><span data-stu-id="45f36-133">7</span></span>|<span data-ttu-id="45f36-134">由 Exchange 确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="45f36-134">Access state determined by Exchange</span></span>|
|<span data-ttu-id="45f36-135">合格</span><span class="sxs-lookup"><span data-stu-id="45f36-135">compliant</span></span>|<span data-ttu-id="45f36-136">8 </span><span class="sxs-lookup"><span data-stu-id="45f36-136">8</span></span>|<span data-ttu-id="45f36-137">合规性挑战授予的访问状态</span><span class="sxs-lookup"><span data-stu-id="45f36-137">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="45f36-138">notCompliant</span><span class="sxs-lookup"><span data-stu-id="45f36-138">notCompliant</span></span>|<span data-ttu-id="45f36-139">9 </span><span class="sxs-lookup"><span data-stu-id="45f36-139">9</span></span>|<span data-ttu-id="45f36-140">由合规性挑战吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="45f36-140">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="45f36-141">notEnrolled</span><span class="sxs-lookup"><span data-stu-id="45f36-141">notEnrolled</span></span>|<span data-ttu-id="45f36-142">10 </span><span class="sxs-lookup"><span data-stu-id="45f36-142">10</span></span>|<span data-ttu-id="45f36-143">由管理质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="45f36-143">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="45f36-144">unknownLocation</span><span class="sxs-lookup"><span data-stu-id="45f36-144">unknownLocation</span></span>|<span data-ttu-id="45f36-145">12 </span><span class="sxs-lookup"><span data-stu-id="45f36-145">12</span></span>|<span data-ttu-id="45f36-146">由于未知位置导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="45f36-146">Access state due to unknown location</span></span>|
|<span data-ttu-id="45f36-147">mfaRequired</span><span class="sxs-lookup"><span data-stu-id="45f36-147">mfaRequired</span></span>|<span data-ttu-id="45f36-148">13 </span><span class="sxs-lookup"><span data-stu-id="45f36-148">13</span></span>|<span data-ttu-id="45f36-149">由于 MFA 质询而导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="45f36-149">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="45f36-150">azureADBlockDueToAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="45f36-150">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="45f36-151">14 </span><span class="sxs-lookup"><span data-stu-id="45f36-151">14</span></span>|<span data-ttu-id="45f36-152">由 AAD 访问策略吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="45f36-152">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="45f36-153">compromisedPassword</span><span class="sxs-lookup"><span data-stu-id="45f36-153">compromisedPassword</span></span>|<span data-ttu-id="45f36-154">15 </span><span class="sxs-lookup"><span data-stu-id="45f36-154">15</span></span>|<span data-ttu-id="45f36-155">通过密码被破解的密码吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="45f36-155">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="45f36-156">deviceNotKnownWithManagedApp</span><span class="sxs-lookup"><span data-stu-id="45f36-156">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="45f36-157">16 </span><span class="sxs-lookup"><span data-stu-id="45f36-157">16</span></span>|<span data-ttu-id="45f36-158">由托管应用程序质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="45f36-158">Access state revoked by managed application challenge</span></span>|









