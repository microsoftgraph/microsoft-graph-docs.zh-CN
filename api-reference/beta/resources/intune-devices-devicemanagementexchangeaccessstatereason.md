---
title: deviceManagementExchangeAccessStateReason 枚举类型
description: 设备 Exchange 访问状态原因。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d6761af448b51c9c434472c4ad43978d34b1b1b6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968458"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="d0264-103">deviceManagementExchangeAccessStateReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d0264-103">deviceManagementExchangeAccessStateReason enum type</span></span>

> <span data-ttu-id="d0264-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d0264-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0264-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d0264-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0264-106">设备 Exchange 访问状态原因。</span><span class="sxs-lookup"><span data-stu-id="d0264-106">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="d0264-107">成员</span><span class="sxs-lookup"><span data-stu-id="d0264-107">Members</span></span>
|<span data-ttu-id="d0264-108">成员</span><span class="sxs-lookup"><span data-stu-id="d0264-108">Member</span></span>|<span data-ttu-id="d0264-109">值</span><span class="sxs-lookup"><span data-stu-id="d0264-109">Value</span></span>|<span data-ttu-id="d0264-110">说明</span><span class="sxs-lookup"><span data-stu-id="d0264-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0264-111">无</span><span class="sxs-lookup"><span data-stu-id="d0264-111">none</span></span>|<span data-ttu-id="d0264-112">0</span><span class="sxs-lookup"><span data-stu-id="d0264-112">0</span></span>|<span data-ttu-id="d0264-113">未发现来自 Exchange 的访问状态原因</span><span class="sxs-lookup"><span data-stu-id="d0264-113">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="d0264-114">unknown</span><span class="sxs-lookup"><span data-stu-id="d0264-114">unknown</span></span>|<span data-ttu-id="d0264-115">1</span><span class="sxs-lookup"><span data-stu-id="d0264-115">1</span></span>|<span data-ttu-id="d0264-116">未知访问状态原因</span><span class="sxs-lookup"><span data-stu-id="d0264-116">Unknown access state reason</span></span>|
|<span data-ttu-id="d0264-117">exchangeGlobalRule</span><span class="sxs-lookup"><span data-stu-id="d0264-117">exchangeGlobalRule</span></span>|<span data-ttu-id="d0264-118">双面</span><span class="sxs-lookup"><span data-stu-id="d0264-118">2</span></span>|<span data-ttu-id="d0264-119">由 Exchange 全局规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="d0264-119">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="d0264-120">exchangeIndividualRule</span><span class="sxs-lookup"><span data-stu-id="d0264-120">exchangeIndividualRule</span></span>|<span data-ttu-id="d0264-121">第三章</span><span class="sxs-lookup"><span data-stu-id="d0264-121">3</span></span>|<span data-ttu-id="d0264-122">由 Exchange 单个规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="d0264-122">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="d0264-123">exchangeDeviceRule</span><span class="sxs-lookup"><span data-stu-id="d0264-123">exchangeDeviceRule</span></span>|<span data-ttu-id="d0264-124">4</span><span class="sxs-lookup"><span data-stu-id="d0264-124">4</span></span>|<span data-ttu-id="d0264-125">由 Exchange 设备规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="d0264-125">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="d0264-126">exchangeUpgrade</span><span class="sxs-lookup"><span data-stu-id="d0264-126">exchangeUpgrade</span></span>|<span data-ttu-id="d0264-127">5</span><span class="sxs-lookup"><span data-stu-id="d0264-127">5</span></span>|<span data-ttu-id="d0264-128">Exchange 升级导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="d0264-128">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="d0264-129">exchangeMailboxPolicy</span><span class="sxs-lookup"><span data-stu-id="d0264-129">exchangeMailboxPolicy</span></span>|<span data-ttu-id="d0264-130">型</span><span class="sxs-lookup"><span data-stu-id="d0264-130">6</span></span>|<span data-ttu-id="d0264-131">由 Exchange 邮箱策略确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="d0264-131">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="d0264-132">相互</span><span class="sxs-lookup"><span data-stu-id="d0264-132">other</span></span>|<span data-ttu-id="d0264-133">步</span><span class="sxs-lookup"><span data-stu-id="d0264-133">7</span></span>|<span data-ttu-id="d0264-134">由 Exchange 确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="d0264-134">Access state determined by Exchange</span></span>|
|<span data-ttu-id="d0264-135">合格</span><span class="sxs-lookup"><span data-stu-id="d0264-135">compliant</span></span>|<span data-ttu-id="d0264-136">utf-8</span><span class="sxs-lookup"><span data-stu-id="d0264-136">8</span></span>|<span data-ttu-id="d0264-137">合规性挑战授予的访问状态</span><span class="sxs-lookup"><span data-stu-id="d0264-137">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="d0264-138">notCompliant</span><span class="sxs-lookup"><span data-stu-id="d0264-138">notCompliant</span></span>|<span data-ttu-id="d0264-139">第</span><span class="sxs-lookup"><span data-stu-id="d0264-139">9</span></span>|<span data-ttu-id="d0264-140">由合规性挑战吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="d0264-140">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="d0264-141">notEnrolled</span><span class="sxs-lookup"><span data-stu-id="d0264-141">notEnrolled</span></span>|<span data-ttu-id="d0264-142">10 </span><span class="sxs-lookup"><span data-stu-id="d0264-142">10</span></span>|<span data-ttu-id="d0264-143">由管理质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="d0264-143">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="d0264-144">unknownLocation</span><span class="sxs-lookup"><span data-stu-id="d0264-144">unknownLocation</span></span>|<span data-ttu-id="d0264-145">12</span><span class="sxs-lookup"><span data-stu-id="d0264-145">12</span></span>|<span data-ttu-id="d0264-146">由于未知位置导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="d0264-146">Access state due to unknown location</span></span>|
|<span data-ttu-id="d0264-147">mfaRequired</span><span class="sxs-lookup"><span data-stu-id="d0264-147">mfaRequired</span></span>|<span data-ttu-id="d0264-148">13</span><span class="sxs-lookup"><span data-stu-id="d0264-148">13</span></span>|<span data-ttu-id="d0264-149">由于 MFA 质询而导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="d0264-149">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="d0264-150">azureADBlockDueToAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="d0264-150">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="d0264-151">日</span><span class="sxs-lookup"><span data-stu-id="d0264-151">14</span></span>|<span data-ttu-id="d0264-152">由 AAD 访问策略吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="d0264-152">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="d0264-153">compromisedPassword</span><span class="sxs-lookup"><span data-stu-id="d0264-153">compromisedPassword</span></span>|<span data-ttu-id="d0264-154">个</span><span class="sxs-lookup"><span data-stu-id="d0264-154">15</span></span>|<span data-ttu-id="d0264-155">通过密码被破解的密码吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="d0264-155">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="d0264-156">deviceNotKnownWithManagedApp</span><span class="sxs-lookup"><span data-stu-id="d0264-156">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="d0264-157">位</span><span class="sxs-lookup"><span data-stu-id="d0264-157">16</span></span>|<span data-ttu-id="d0264-158">由托管应用程序质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="d0264-158">Access state revoked by managed application challenge</span></span>|





