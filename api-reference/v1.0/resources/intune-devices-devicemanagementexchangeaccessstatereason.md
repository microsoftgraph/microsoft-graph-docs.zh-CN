---
title: deviceManagementExchangeAccessStateReason 枚举类型
description: 设备 Exchange 访问状态原因。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3c598b06d51ef6852086cadd011fe9145f61dc1f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356932"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="0c7c6-103">deviceManagementExchangeAccessStateReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0c7c6-103">deviceManagementExchangeAccessStateReason enum type</span></span>

> <span data-ttu-id="0c7c6-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0c7c6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c7c6-105">设备 Exchange 访问状态原因。</span><span class="sxs-lookup"><span data-stu-id="0c7c6-105">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="0c7c6-106">成员</span><span class="sxs-lookup"><span data-stu-id="0c7c6-106">Members</span></span>
|<span data-ttu-id="0c7c6-107">成员</span><span class="sxs-lookup"><span data-stu-id="0c7c6-107">Member</span></span>|<span data-ttu-id="0c7c6-108">值</span><span class="sxs-lookup"><span data-stu-id="0c7c6-108">Value</span></span>|<span data-ttu-id="0c7c6-109">说明</span><span class="sxs-lookup"><span data-stu-id="0c7c6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c7c6-110">无</span><span class="sxs-lookup"><span data-stu-id="0c7c6-110">none</span></span>|<span data-ttu-id="0c7c6-111">0</span><span class="sxs-lookup"><span data-stu-id="0c7c6-111">0</span></span>|<span data-ttu-id="0c7c6-112">未发现来自 Exchange 的访问状态原因</span><span class="sxs-lookup"><span data-stu-id="0c7c6-112">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="0c7c6-113">unknown</span><span class="sxs-lookup"><span data-stu-id="0c7c6-113">unknown</span></span>|<span data-ttu-id="0c7c6-114">1</span><span class="sxs-lookup"><span data-stu-id="0c7c6-114">1</span></span>|<span data-ttu-id="0c7c6-115">未知访问状态原因</span><span class="sxs-lookup"><span data-stu-id="0c7c6-115">Unknown access state reason</span></span>|
|<span data-ttu-id="0c7c6-116">exchangeGlobalRule</span><span class="sxs-lookup"><span data-stu-id="0c7c6-116">exchangeGlobalRule</span></span>|<span data-ttu-id="0c7c6-117">双面</span><span class="sxs-lookup"><span data-stu-id="0c7c6-117">2</span></span>|<span data-ttu-id="0c7c6-118">由 Exchange 全局规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="0c7c6-118">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="0c7c6-119">exchangeIndividualRule</span><span class="sxs-lookup"><span data-stu-id="0c7c6-119">exchangeIndividualRule</span></span>|<span data-ttu-id="0c7c6-120">第三章</span><span class="sxs-lookup"><span data-stu-id="0c7c6-120">3</span></span>|<span data-ttu-id="0c7c6-121">由 Exchange 单个规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="0c7c6-121">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="0c7c6-122">exchangeDeviceRule</span><span class="sxs-lookup"><span data-stu-id="0c7c6-122">exchangeDeviceRule</span></span>|<span data-ttu-id="0c7c6-123">4</span><span class="sxs-lookup"><span data-stu-id="0c7c6-123">4</span></span>|<span data-ttu-id="0c7c6-124">由 Exchange 设备规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="0c7c6-124">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="0c7c6-125">exchangeUpgrade</span><span class="sxs-lookup"><span data-stu-id="0c7c6-125">exchangeUpgrade</span></span>|<span data-ttu-id="0c7c6-126">5</span><span class="sxs-lookup"><span data-stu-id="0c7c6-126">5</span></span>|<span data-ttu-id="0c7c6-127">Exchange 升级导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="0c7c6-127">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="0c7c6-128">exchangeMailboxPolicy</span><span class="sxs-lookup"><span data-stu-id="0c7c6-128">exchangeMailboxPolicy</span></span>|<span data-ttu-id="0c7c6-129">型</span><span class="sxs-lookup"><span data-stu-id="0c7c6-129">6</span></span>|<span data-ttu-id="0c7c6-130">由 Exchange 邮箱策略确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="0c7c6-130">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="0c7c6-131">相互</span><span class="sxs-lookup"><span data-stu-id="0c7c6-131">other</span></span>|<span data-ttu-id="0c7c6-132">步</span><span class="sxs-lookup"><span data-stu-id="0c7c6-132">7</span></span>|<span data-ttu-id="0c7c6-133">由 Exchange 确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="0c7c6-133">Access state determined by Exchange</span></span>|
|<span data-ttu-id="0c7c6-134">合格</span><span class="sxs-lookup"><span data-stu-id="0c7c6-134">compliant</span></span>|<span data-ttu-id="0c7c6-135">utf-8</span><span class="sxs-lookup"><span data-stu-id="0c7c6-135">8</span></span>|<span data-ttu-id="0c7c6-136">合规性挑战授予的访问状态</span><span class="sxs-lookup"><span data-stu-id="0c7c6-136">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="0c7c6-137">notCompliant</span><span class="sxs-lookup"><span data-stu-id="0c7c6-137">notCompliant</span></span>|<span data-ttu-id="0c7c6-138">第</span><span class="sxs-lookup"><span data-stu-id="0c7c6-138">9</span></span>|<span data-ttu-id="0c7c6-139">由合规性挑战吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="0c7c6-139">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="0c7c6-140">notEnrolled</span><span class="sxs-lookup"><span data-stu-id="0c7c6-140">notEnrolled</span></span>|<span data-ttu-id="0c7c6-141">10 </span><span class="sxs-lookup"><span data-stu-id="0c7c6-141">10</span></span>|<span data-ttu-id="0c7c6-142">由管理质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="0c7c6-142">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="0c7c6-143">unknownLocation</span><span class="sxs-lookup"><span data-stu-id="0c7c6-143">unknownLocation</span></span>|<span data-ttu-id="0c7c6-144">12</span><span class="sxs-lookup"><span data-stu-id="0c7c6-144">12</span></span>|<span data-ttu-id="0c7c6-145">由于未知位置导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="0c7c6-145">Access state due to unknown location</span></span>|
|<span data-ttu-id="0c7c6-146">mfaRequired</span><span class="sxs-lookup"><span data-stu-id="0c7c6-146">mfaRequired</span></span>|<span data-ttu-id="0c7c6-147">13</span><span class="sxs-lookup"><span data-stu-id="0c7c6-147">13</span></span>|<span data-ttu-id="0c7c6-148">由于 MFA 质询而导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="0c7c6-148">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="0c7c6-149">azureADBlockDueToAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="0c7c6-149">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="0c7c6-150">日</span><span class="sxs-lookup"><span data-stu-id="0c7c6-150">14</span></span>|<span data-ttu-id="0c7c6-151">由 AAD 访问策略吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="0c7c6-151">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="0c7c6-152">compromisedPassword</span><span class="sxs-lookup"><span data-stu-id="0c7c6-152">compromisedPassword</span></span>|<span data-ttu-id="0c7c6-153">个</span><span class="sxs-lookup"><span data-stu-id="0c7c6-153">15</span></span>|<span data-ttu-id="0c7c6-154">通过密码被破解的密码吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="0c7c6-154">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="0c7c6-155">deviceNotKnownWithManagedApp</span><span class="sxs-lookup"><span data-stu-id="0c7c6-155">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="0c7c6-156">位</span><span class="sxs-lookup"><span data-stu-id="0c7c6-156">16</span></span>|<span data-ttu-id="0c7c6-157">由托管应用程序质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="0c7c6-157">Access state revoked by managed application challenge</span></span>|




