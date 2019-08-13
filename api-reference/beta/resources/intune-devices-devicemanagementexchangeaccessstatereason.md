---
title: deviceManagementExchangeAccessStateReason 枚举类型
description: 设备 Exchange 访问状态原因。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 525f994b19cff11b06109726e7efbc2033cad69a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370079"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="58a0b-103">deviceManagementExchangeAccessStateReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="58a0b-103">deviceManagementExchangeAccessStateReason enum type</span></span>

> <span data-ttu-id="58a0b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="58a0b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58a0b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="58a0b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58a0b-106">设备 Exchange 访问状态原因。</span><span class="sxs-lookup"><span data-stu-id="58a0b-106">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="58a0b-107">成员</span><span class="sxs-lookup"><span data-stu-id="58a0b-107">Members</span></span>
|<span data-ttu-id="58a0b-108">成员</span><span class="sxs-lookup"><span data-stu-id="58a0b-108">Member</span></span>|<span data-ttu-id="58a0b-109">值</span><span class="sxs-lookup"><span data-stu-id="58a0b-109">Value</span></span>|<span data-ttu-id="58a0b-110">说明</span><span class="sxs-lookup"><span data-stu-id="58a0b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58a0b-111">无</span><span class="sxs-lookup"><span data-stu-id="58a0b-111">none</span></span>|<span data-ttu-id="58a0b-112">0</span><span class="sxs-lookup"><span data-stu-id="58a0b-112">0</span></span>|<span data-ttu-id="58a0b-113">未发现来自 Exchange 的访问状态原因</span><span class="sxs-lookup"><span data-stu-id="58a0b-113">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="58a0b-114">unknown</span><span class="sxs-lookup"><span data-stu-id="58a0b-114">unknown</span></span>|<span data-ttu-id="58a0b-115">1</span><span class="sxs-lookup"><span data-stu-id="58a0b-115">1</span></span>|<span data-ttu-id="58a0b-116">未知访问状态原因</span><span class="sxs-lookup"><span data-stu-id="58a0b-116">Unknown access state reason</span></span>|
|<span data-ttu-id="58a0b-117">exchangeGlobalRule</span><span class="sxs-lookup"><span data-stu-id="58a0b-117">exchangeGlobalRule</span></span>|<span data-ttu-id="58a0b-118">双面</span><span class="sxs-lookup"><span data-stu-id="58a0b-118">2</span></span>|<span data-ttu-id="58a0b-119">由 Exchange 全局规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="58a0b-119">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="58a0b-120">exchangeIndividualRule</span><span class="sxs-lookup"><span data-stu-id="58a0b-120">exchangeIndividualRule</span></span>|<span data-ttu-id="58a0b-121">第三章</span><span class="sxs-lookup"><span data-stu-id="58a0b-121">3</span></span>|<span data-ttu-id="58a0b-122">由 Exchange 单个规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="58a0b-122">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="58a0b-123">exchangeDeviceRule</span><span class="sxs-lookup"><span data-stu-id="58a0b-123">exchangeDeviceRule</span></span>|<span data-ttu-id="58a0b-124">4</span><span class="sxs-lookup"><span data-stu-id="58a0b-124">4</span></span>|<span data-ttu-id="58a0b-125">由 Exchange 设备规则确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="58a0b-125">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="58a0b-126">exchangeUpgrade</span><span class="sxs-lookup"><span data-stu-id="58a0b-126">exchangeUpgrade</span></span>|<span data-ttu-id="58a0b-127">5</span><span class="sxs-lookup"><span data-stu-id="58a0b-127">5</span></span>|<span data-ttu-id="58a0b-128">Exchange 升级导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="58a0b-128">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="58a0b-129">exchangeMailboxPolicy</span><span class="sxs-lookup"><span data-stu-id="58a0b-129">exchangeMailboxPolicy</span></span>|<span data-ttu-id="58a0b-130">型</span><span class="sxs-lookup"><span data-stu-id="58a0b-130">6</span></span>|<span data-ttu-id="58a0b-131">由 Exchange 邮箱策略确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="58a0b-131">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="58a0b-132">相互</span><span class="sxs-lookup"><span data-stu-id="58a0b-132">other</span></span>|<span data-ttu-id="58a0b-133">步</span><span class="sxs-lookup"><span data-stu-id="58a0b-133">7</span></span>|<span data-ttu-id="58a0b-134">由 Exchange 确定的访问状态</span><span class="sxs-lookup"><span data-stu-id="58a0b-134">Access state determined by Exchange</span></span>|
|<span data-ttu-id="58a0b-135">合格</span><span class="sxs-lookup"><span data-stu-id="58a0b-135">compliant</span></span>|<span data-ttu-id="58a0b-136">utf-8</span><span class="sxs-lookup"><span data-stu-id="58a0b-136">8</span></span>|<span data-ttu-id="58a0b-137">合规性挑战授予的访问状态</span><span class="sxs-lookup"><span data-stu-id="58a0b-137">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="58a0b-138">notCompliant</span><span class="sxs-lookup"><span data-stu-id="58a0b-138">notCompliant</span></span>|<span data-ttu-id="58a0b-139">第</span><span class="sxs-lookup"><span data-stu-id="58a0b-139">9</span></span>|<span data-ttu-id="58a0b-140">由合规性挑战吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="58a0b-140">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="58a0b-141">notEnrolled</span><span class="sxs-lookup"><span data-stu-id="58a0b-141">notEnrolled</span></span>|<span data-ttu-id="58a0b-142">10 </span><span class="sxs-lookup"><span data-stu-id="58a0b-142">10</span></span>|<span data-ttu-id="58a0b-143">由管理质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="58a0b-143">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="58a0b-144">unknownLocation</span><span class="sxs-lookup"><span data-stu-id="58a0b-144">unknownLocation</span></span>|<span data-ttu-id="58a0b-145">12</span><span class="sxs-lookup"><span data-stu-id="58a0b-145">12</span></span>|<span data-ttu-id="58a0b-146">由于未知位置导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="58a0b-146">Access state due to unknown location</span></span>|
|<span data-ttu-id="58a0b-147">mfaRequired</span><span class="sxs-lookup"><span data-stu-id="58a0b-147">mfaRequired</span></span>|<span data-ttu-id="58a0b-148">13</span><span class="sxs-lookup"><span data-stu-id="58a0b-148">13</span></span>|<span data-ttu-id="58a0b-149">由于 MFA 质询而导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="58a0b-149">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="58a0b-150">azureADBlockDueToAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="58a0b-150">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="58a0b-151">日</span><span class="sxs-lookup"><span data-stu-id="58a0b-151">14</span></span>|<span data-ttu-id="58a0b-152">由 AAD 访问策略吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="58a0b-152">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="58a0b-153">compromisedPassword</span><span class="sxs-lookup"><span data-stu-id="58a0b-153">compromisedPassword</span></span>|<span data-ttu-id="58a0b-154">个</span><span class="sxs-lookup"><span data-stu-id="58a0b-154">15</span></span>|<span data-ttu-id="58a0b-155">通过密码被破解的密码吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="58a0b-155">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="58a0b-156">deviceNotKnownWithManagedApp</span><span class="sxs-lookup"><span data-stu-id="58a0b-156">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="58a0b-157">位</span><span class="sxs-lookup"><span data-stu-id="58a0b-157">16</span></span>|<span data-ttu-id="58a0b-158">由托管应用程序质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="58a0b-158">Access state revoked by managed application challenge</span></span>|



