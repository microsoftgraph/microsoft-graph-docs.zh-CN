---
title: deviceManagementExchangeAccessStateReason 枚举类型
description: 设备Exchange访问状态原因。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7aa61e8ecdf88663123a486cb9bccb033aeecbb5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754572"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="e063c-103">deviceManagementExchangeAccessStateReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e063c-103">deviceManagementExchangeAccessStateReason enum type</span></span>

<span data-ttu-id="e063c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e063c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e063c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e063c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e063c-106">设备Exchange访问状态原因。</span><span class="sxs-lookup"><span data-stu-id="e063c-106">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="e063c-107">成员</span><span class="sxs-lookup"><span data-stu-id="e063c-107">Members</span></span>
|<span data-ttu-id="e063c-108">成员</span><span class="sxs-lookup"><span data-stu-id="e063c-108">Member</span></span>|<span data-ttu-id="e063c-109">值</span><span class="sxs-lookup"><span data-stu-id="e063c-109">Value</span></span>|<span data-ttu-id="e063c-110">Description</span><span class="sxs-lookup"><span data-stu-id="e063c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e063c-111">无</span><span class="sxs-lookup"><span data-stu-id="e063c-111">none</span></span>|<span data-ttu-id="e063c-112">0</span><span class="sxs-lookup"><span data-stu-id="e063c-112">0</span></span>|<span data-ttu-id="e063c-113">未从用户发现任何访问Exchange</span><span class="sxs-lookup"><span data-stu-id="e063c-113">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="e063c-114">unknown</span><span class="sxs-lookup"><span data-stu-id="e063c-114">unknown</span></span>|<span data-ttu-id="e063c-115">1</span><span class="sxs-lookup"><span data-stu-id="e063c-115">1</span></span>|<span data-ttu-id="e063c-116">未知访问状态原因</span><span class="sxs-lookup"><span data-stu-id="e063c-116">Unknown access state reason</span></span>|
|<span data-ttu-id="e063c-117">exchangeGlobalRule</span><span class="sxs-lookup"><span data-stu-id="e063c-117">exchangeGlobalRule</span></span>|<span data-ttu-id="e063c-118">2</span><span class="sxs-lookup"><span data-stu-id="e063c-118">2</span></span>|<span data-ttu-id="e063c-119">由全局规则Exchange的访问状态</span><span class="sxs-lookup"><span data-stu-id="e063c-119">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="e063c-120">exchangeIndividualRule</span><span class="sxs-lookup"><span data-stu-id="e063c-120">exchangeIndividualRule</span></span>|<span data-ttu-id="e063c-121">3</span><span class="sxs-lookup"><span data-stu-id="e063c-121">3</span></span>|<span data-ttu-id="e063c-122">由单个规则Exchange的访问状态</span><span class="sxs-lookup"><span data-stu-id="e063c-122">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="e063c-123">exchangeDeviceRule</span><span class="sxs-lookup"><span data-stu-id="e063c-123">exchangeDeviceRule</span></span>|<span data-ttu-id="e063c-124">4 </span><span class="sxs-lookup"><span data-stu-id="e063c-124">4</span></span>|<span data-ttu-id="e063c-125">由设备规则Exchange的访问状态</span><span class="sxs-lookup"><span data-stu-id="e063c-125">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="e063c-126">exchangeUpgrade</span><span class="sxs-lookup"><span data-stu-id="e063c-126">exchangeUpgrade</span></span>|<span data-ttu-id="e063c-127">5 </span><span class="sxs-lookup"><span data-stu-id="e063c-127">5</span></span>|<span data-ttu-id="e063c-128">由于升级Exchange访问状态</span><span class="sxs-lookup"><span data-stu-id="e063c-128">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="e063c-129">exchangeMailboxPolicy</span><span class="sxs-lookup"><span data-stu-id="e063c-129">exchangeMailboxPolicy</span></span>|<span data-ttu-id="e063c-130">6 </span><span class="sxs-lookup"><span data-stu-id="e063c-130">6</span></span>|<span data-ttu-id="e063c-131">由邮箱策略Exchange的访问状态</span><span class="sxs-lookup"><span data-stu-id="e063c-131">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="e063c-132">other</span><span class="sxs-lookup"><span data-stu-id="e063c-132">other</span></span>|<span data-ttu-id="e063c-133">7 </span><span class="sxs-lookup"><span data-stu-id="e063c-133">7</span></span>|<span data-ttu-id="e063c-134">访问状态由用户Exchange</span><span class="sxs-lookup"><span data-stu-id="e063c-134">Access state determined by Exchange</span></span>|
|<span data-ttu-id="e063c-135">compliant</span><span class="sxs-lookup"><span data-stu-id="e063c-135">compliant</span></span>|<span data-ttu-id="e063c-136">8 </span><span class="sxs-lookup"><span data-stu-id="e063c-136">8</span></span>|<span data-ttu-id="e063c-137">合规性质询授予的访问状态</span><span class="sxs-lookup"><span data-stu-id="e063c-137">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="e063c-138">notCompliant</span><span class="sxs-lookup"><span data-stu-id="e063c-138">notCompliant</span></span>|<span data-ttu-id="e063c-139">9 </span><span class="sxs-lookup"><span data-stu-id="e063c-139">9</span></span>|<span data-ttu-id="e063c-140">合规性质询撤销的访问状态</span><span class="sxs-lookup"><span data-stu-id="e063c-140">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="e063c-141">notEnrolled</span><span class="sxs-lookup"><span data-stu-id="e063c-141">notEnrolled</span></span>|<span data-ttu-id="e063c-142">10  </span><span class="sxs-lookup"><span data-stu-id="e063c-142">10</span></span>|<span data-ttu-id="e063c-143">管理质询撤销的访问状态</span><span class="sxs-lookup"><span data-stu-id="e063c-143">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="e063c-144">unknownLocation</span><span class="sxs-lookup"><span data-stu-id="e063c-144">unknownLocation</span></span>|<span data-ttu-id="e063c-145">12 </span><span class="sxs-lookup"><span data-stu-id="e063c-145">12</span></span>|<span data-ttu-id="e063c-146">由于位置未知而进入访问状态</span><span class="sxs-lookup"><span data-stu-id="e063c-146">Access state due to unknown location</span></span>|
|<span data-ttu-id="e063c-147">mfaRequired</span><span class="sxs-lookup"><span data-stu-id="e063c-147">mfaRequired</span></span>|<span data-ttu-id="e063c-148">13</span><span class="sxs-lookup"><span data-stu-id="e063c-148">13</span></span>|<span data-ttu-id="e063c-149">MFA 质询导致的访问状态</span><span class="sxs-lookup"><span data-stu-id="e063c-149">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="e063c-150">azureADBlockDueToAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="e063c-150">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="e063c-151">14 </span><span class="sxs-lookup"><span data-stu-id="e063c-151">14</span></span>|<span data-ttu-id="e063c-152">AAD 访问策略吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="e063c-152">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="e063c-153">compromisedPassword</span><span class="sxs-lookup"><span data-stu-id="e063c-153">compromisedPassword</span></span>|<span data-ttu-id="e063c-154">15</span><span class="sxs-lookup"><span data-stu-id="e063c-154">15</span></span>|<span data-ttu-id="e063c-155">通过泄露的密码吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="e063c-155">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="e063c-156">deviceNotKnownWithManagedApp</span><span class="sxs-lookup"><span data-stu-id="e063c-156">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="e063c-157">16 </span><span class="sxs-lookup"><span data-stu-id="e063c-157">16</span></span>|<span data-ttu-id="e063c-158">托管应用程序质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="e063c-158">Access state revoked by managed application challenge</span></span>|




