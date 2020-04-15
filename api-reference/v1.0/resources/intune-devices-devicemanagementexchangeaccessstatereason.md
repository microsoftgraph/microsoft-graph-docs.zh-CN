---
title: deviceManagementExchangeAccessStateReason 枚举类型
description: 设备 Exchange 访问状态原因。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bf3b6d3200ab461877b90dda2226437c863b4d0c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453988"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="85972-103">deviceManagementExchangeAccessStateReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="85972-103">deviceManagementExchangeAccessStateReason enum type</span></span>

<span data-ttu-id="85972-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85972-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85972-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85972-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85972-106">设备 Exchange 访问状态原因。</span><span class="sxs-lookup"><span data-stu-id="85972-106">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="85972-107">成员</span><span class="sxs-lookup"><span data-stu-id="85972-107">Members</span></span>
|<span data-ttu-id="85972-108">成员</span><span class="sxs-lookup"><span data-stu-id="85972-108">Member</span></span>|<span data-ttu-id="85972-109">值</span><span class="sxs-lookup"><span data-stu-id="85972-109">Value</span></span>|<span data-ttu-id="85972-110">说明</span><span class="sxs-lookup"><span data-stu-id="85972-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85972-111">无</span><span class="sxs-lookup"><span data-stu-id="85972-111">none</span></span>|<span data-ttu-id="85972-112">0</span><span class="sxs-lookup"><span data-stu-id="85972-112">0</span></span>|<span data-ttu-id="85972-113">未发现来自 Exchange 的访问状态原因</span><span class="sxs-lookup"><span data-stu-id="85972-113">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="85972-114">unknown</span><span class="sxs-lookup"><span data-stu-id="85972-114">unknown</span></span>|<span data-ttu-id="85972-115">1</span><span class="sxs-lookup"><span data-stu-id="85972-115">1</span></span>|<span data-ttu-id="85972-116">未知访问状态原因</span><span class="sxs-lookup"><span data-stu-id="85972-116">Unknown access state reason</span></span>|
|<span data-ttu-id="85972-117">exchangeGlobalRule</span><span class="sxs-lookup"><span data-stu-id="85972-117">exchangeGlobalRule</span></span>|<span data-ttu-id="85972-118">双面</span><span class="sxs-lookup"><span data-stu-id="85972-118">2</span></span>|<span data-ttu-id="85972-119">由 Exchange 全局规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="85972-119">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="85972-120">exchangeIndividualRule</span><span class="sxs-lookup"><span data-stu-id="85972-120">exchangeIndividualRule</span></span>|<span data-ttu-id="85972-121">第三章</span><span class="sxs-lookup"><span data-stu-id="85972-121">3</span></span>|<span data-ttu-id="85972-122">由 Exchange 单个规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="85972-122">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="85972-123">exchangeDeviceRule</span><span class="sxs-lookup"><span data-stu-id="85972-123">exchangeDeviceRule</span></span>|<span data-ttu-id="85972-124">4 </span><span class="sxs-lookup"><span data-stu-id="85972-124">4</span></span>|<span data-ttu-id="85972-125">由 Exchange 设备规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="85972-125">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="85972-126">exchangeUpgrade</span><span class="sxs-lookup"><span data-stu-id="85972-126">exchangeUpgrade</span></span>|<span data-ttu-id="85972-127">5 </span><span class="sxs-lookup"><span data-stu-id="85972-127">5</span></span>|<span data-ttu-id="85972-128">Exchange 升级导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="85972-128">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="85972-129">exchangeMailboxPolicy</span><span class="sxs-lookup"><span data-stu-id="85972-129">exchangeMailboxPolicy</span></span>|<span data-ttu-id="85972-130">6 </span><span class="sxs-lookup"><span data-stu-id="85972-130">6</span></span>|<span data-ttu-id="85972-131">由 Exchange 邮箱策略确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="85972-131">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="85972-132">相互</span><span class="sxs-lookup"><span data-stu-id="85972-132">other</span></span>|<span data-ttu-id="85972-133">7 </span><span class="sxs-lookup"><span data-stu-id="85972-133">7</span></span>|<span data-ttu-id="85972-134">由 Exchange 确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="85972-134">Access state determined by Exchange</span></span>|
|<span data-ttu-id="85972-135">合格</span><span class="sxs-lookup"><span data-stu-id="85972-135">compliant</span></span>|<span data-ttu-id="85972-136">8 </span><span class="sxs-lookup"><span data-stu-id="85972-136">8</span></span>|<span data-ttu-id="85972-137">合规性挑战授予的访问状态</span><span class="sxs-lookup"><span data-stu-id="85972-137">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="85972-138">notCompliant</span><span class="sxs-lookup"><span data-stu-id="85972-138">notCompliant</span></span>|<span data-ttu-id="85972-139">9 </span><span class="sxs-lookup"><span data-stu-id="85972-139">9</span></span>|<span data-ttu-id="85972-140">由合规性挑战吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="85972-140">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="85972-141">notEnrolled</span><span class="sxs-lookup"><span data-stu-id="85972-141">notEnrolled</span></span>|<span data-ttu-id="85972-142">10 </span><span class="sxs-lookup"><span data-stu-id="85972-142">10</span></span>|<span data-ttu-id="85972-143">由管理质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="85972-143">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="85972-144">unknownLocation</span><span class="sxs-lookup"><span data-stu-id="85972-144">unknownLocation</span></span>|<span data-ttu-id="85972-145">12 </span><span class="sxs-lookup"><span data-stu-id="85972-145">12</span></span>|<span data-ttu-id="85972-146">由于未知位置导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="85972-146">Access state due to unknown location</span></span>|
|<span data-ttu-id="85972-147">mfaRequired</span><span class="sxs-lookup"><span data-stu-id="85972-147">mfaRequired</span></span>|<span data-ttu-id="85972-148">13</span><span class="sxs-lookup"><span data-stu-id="85972-148">13</span></span>|<span data-ttu-id="85972-149">由于 MFA 质询而导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="85972-149">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="85972-150">azureADBlockDueToAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="85972-150">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="85972-151">14 </span><span class="sxs-lookup"><span data-stu-id="85972-151">14</span></span>|<span data-ttu-id="85972-152">由 AAD 访问策略吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="85972-152">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="85972-153">compromisedPassword</span><span class="sxs-lookup"><span data-stu-id="85972-153">compromisedPassword</span></span>|<span data-ttu-id="85972-154">15 </span><span class="sxs-lookup"><span data-stu-id="85972-154">15</span></span>|<span data-ttu-id="85972-155">通过密码被破解的密码吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="85972-155">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="85972-156">deviceNotKnownWithManagedApp</span><span class="sxs-lookup"><span data-stu-id="85972-156">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="85972-157">16 </span><span class="sxs-lookup"><span data-stu-id="85972-157">16</span></span>|<span data-ttu-id="85972-158">由托管应用程序质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="85972-158">Access state revoked by managed application challenge</span></span>|







