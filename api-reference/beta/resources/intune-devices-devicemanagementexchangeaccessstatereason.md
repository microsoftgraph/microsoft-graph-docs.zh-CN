---
title: deviceManagementExchangeAccessStateReason 枚举类型
description: 设备 Exchange 访问状态原因。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 695127717baa51f1888fd3b20d2bed4a42464e1b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299196"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="b1ba6-103">deviceManagementExchangeAccessStateReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b1ba6-103">deviceManagementExchangeAccessStateReason enum type</span></span>

<span data-ttu-id="b1ba6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1ba6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1ba6-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b1ba6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1ba6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1ba6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1ba6-107">设备 Exchange 访问状态原因。</span><span class="sxs-lookup"><span data-stu-id="b1ba6-107">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="b1ba6-108">成员</span><span class="sxs-lookup"><span data-stu-id="b1ba6-108">Members</span></span>
|<span data-ttu-id="b1ba6-109">成员</span><span class="sxs-lookup"><span data-stu-id="b1ba6-109">Member</span></span>|<span data-ttu-id="b1ba6-110">值</span><span class="sxs-lookup"><span data-stu-id="b1ba6-110">Value</span></span>|<span data-ttu-id="b1ba6-111">Description</span><span class="sxs-lookup"><span data-stu-id="b1ba6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1ba6-112">无</span><span class="sxs-lookup"><span data-stu-id="b1ba6-112">none</span></span>|<span data-ttu-id="b1ba6-113">0</span><span class="sxs-lookup"><span data-stu-id="b1ba6-113">0</span></span>|<span data-ttu-id="b1ba6-114">未发现来自 Exchange 的访问状态原因</span><span class="sxs-lookup"><span data-stu-id="b1ba6-114">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="b1ba6-115">unknown</span><span class="sxs-lookup"><span data-stu-id="b1ba6-115">unknown</span></span>|<span data-ttu-id="b1ba6-116">1</span><span class="sxs-lookup"><span data-stu-id="b1ba6-116">1</span></span>|<span data-ttu-id="b1ba6-117">未知访问状态原因</span><span class="sxs-lookup"><span data-stu-id="b1ba6-117">Unknown access state reason</span></span>|
|<span data-ttu-id="b1ba6-118">exchangeGlobalRule</span><span class="sxs-lookup"><span data-stu-id="b1ba6-118">exchangeGlobalRule</span></span>|<span data-ttu-id="b1ba6-119">双面</span><span class="sxs-lookup"><span data-stu-id="b1ba6-119">2</span></span>|<span data-ttu-id="b1ba6-120">由 Exchange 全局规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="b1ba6-120">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="b1ba6-121">exchangeIndividualRule</span><span class="sxs-lookup"><span data-stu-id="b1ba6-121">exchangeIndividualRule</span></span>|<span data-ttu-id="b1ba6-122">第三章</span><span class="sxs-lookup"><span data-stu-id="b1ba6-122">3</span></span>|<span data-ttu-id="b1ba6-123">由 Exchange 单个规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="b1ba6-123">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="b1ba6-124">exchangeDeviceRule</span><span class="sxs-lookup"><span data-stu-id="b1ba6-124">exchangeDeviceRule</span></span>|<span data-ttu-id="b1ba6-125">4 </span><span class="sxs-lookup"><span data-stu-id="b1ba6-125">4</span></span>|<span data-ttu-id="b1ba6-126">由 Exchange 设备规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="b1ba6-126">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="b1ba6-127">exchangeUpgrade</span><span class="sxs-lookup"><span data-stu-id="b1ba6-127">exchangeUpgrade</span></span>|<span data-ttu-id="b1ba6-128">5 </span><span class="sxs-lookup"><span data-stu-id="b1ba6-128">5</span></span>|<span data-ttu-id="b1ba6-129">Exchange 升级导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="b1ba6-129">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="b1ba6-130">exchangeMailboxPolicy</span><span class="sxs-lookup"><span data-stu-id="b1ba6-130">exchangeMailboxPolicy</span></span>|<span data-ttu-id="b1ba6-131">6 </span><span class="sxs-lookup"><span data-stu-id="b1ba6-131">6</span></span>|<span data-ttu-id="b1ba6-132">由 Exchange 邮箱策略确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="b1ba6-132">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="b1ba6-133">相互</span><span class="sxs-lookup"><span data-stu-id="b1ba6-133">other</span></span>|<span data-ttu-id="b1ba6-134">7 </span><span class="sxs-lookup"><span data-stu-id="b1ba6-134">7</span></span>|<span data-ttu-id="b1ba6-135">由 Exchange 确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="b1ba6-135">Access state determined by Exchange</span></span>|
|<span data-ttu-id="b1ba6-136">合格</span><span class="sxs-lookup"><span data-stu-id="b1ba6-136">compliant</span></span>|<span data-ttu-id="b1ba6-137">8 </span><span class="sxs-lookup"><span data-stu-id="b1ba6-137">8</span></span>|<span data-ttu-id="b1ba6-138">合规性挑战授予的访问状态</span><span class="sxs-lookup"><span data-stu-id="b1ba6-138">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="b1ba6-139">notCompliant</span><span class="sxs-lookup"><span data-stu-id="b1ba6-139">notCompliant</span></span>|<span data-ttu-id="b1ba6-140">9 </span><span class="sxs-lookup"><span data-stu-id="b1ba6-140">9</span></span>|<span data-ttu-id="b1ba6-141">由合规性挑战吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="b1ba6-141">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="b1ba6-142">notEnrolled</span><span class="sxs-lookup"><span data-stu-id="b1ba6-142">notEnrolled</span></span>|<span data-ttu-id="b1ba6-143">10  </span><span class="sxs-lookup"><span data-stu-id="b1ba6-143">10</span></span>|<span data-ttu-id="b1ba6-144">由管理质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="b1ba6-144">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="b1ba6-145">unknownLocation</span><span class="sxs-lookup"><span data-stu-id="b1ba6-145">unknownLocation</span></span>|<span data-ttu-id="b1ba6-146">12 </span><span class="sxs-lookup"><span data-stu-id="b1ba6-146">12</span></span>|<span data-ttu-id="b1ba6-147">由于未知位置导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="b1ba6-147">Access state due to unknown location</span></span>|
|<span data-ttu-id="b1ba6-148">mfaRequired</span><span class="sxs-lookup"><span data-stu-id="b1ba6-148">mfaRequired</span></span>|<span data-ttu-id="b1ba6-149">13 </span><span class="sxs-lookup"><span data-stu-id="b1ba6-149">13</span></span>|<span data-ttu-id="b1ba6-150">由于 MFA 质询而导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="b1ba6-150">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="b1ba6-151">azureADBlockDueToAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="b1ba6-151">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="b1ba6-152">14 </span><span class="sxs-lookup"><span data-stu-id="b1ba6-152">14</span></span>|<span data-ttu-id="b1ba6-153">由 AAD 访问策略吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="b1ba6-153">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="b1ba6-154">compromisedPassword</span><span class="sxs-lookup"><span data-stu-id="b1ba6-154">compromisedPassword</span></span>|<span data-ttu-id="b1ba6-155">15 </span><span class="sxs-lookup"><span data-stu-id="b1ba6-155">15</span></span>|<span data-ttu-id="b1ba6-156">通过密码被破解的密码吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="b1ba6-156">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="b1ba6-157">deviceNotKnownWithManagedApp</span><span class="sxs-lookup"><span data-stu-id="b1ba6-157">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="b1ba6-158">16 </span><span class="sxs-lookup"><span data-stu-id="b1ba6-158">16</span></span>|<span data-ttu-id="b1ba6-159">由托管应用程序质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="b1ba6-159">Access state revoked by managed application challenge</span></span>|




