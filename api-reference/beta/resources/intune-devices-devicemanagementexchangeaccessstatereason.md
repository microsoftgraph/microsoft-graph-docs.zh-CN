---
title: deviceManagementExchangeAccessStateReason 枚举类型
description: 设备 Exchange 访问状态的原因。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b7a076239e49c59cb95cd1c1f644bc9a2f1f906e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395858"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="a9501-103">deviceManagementExchangeAccessStateReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a9501-103">deviceManagementExchangeAccessStateReason enum type</span></span>

> <span data-ttu-id="a9501-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a9501-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a9501-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a9501-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a9501-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a9501-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9501-107">设备 Exchange 访问状态的原因。</span><span class="sxs-lookup"><span data-stu-id="a9501-107">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="a9501-108">成员</span><span class="sxs-lookup"><span data-stu-id="a9501-108">Members</span></span>
|<span data-ttu-id="a9501-109">成员</span><span class="sxs-lookup"><span data-stu-id="a9501-109">Member</span></span>|<span data-ttu-id="a9501-110">值</span><span class="sxs-lookup"><span data-stu-id="a9501-110">Value</span></span>|<span data-ttu-id="a9501-111">说明</span><span class="sxs-lookup"><span data-stu-id="a9501-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9501-112">无</span><span class="sxs-lookup"><span data-stu-id="a9501-112">none</span></span>|<span data-ttu-id="a9501-113">0</span><span class="sxs-lookup"><span data-stu-id="a9501-113">0</span></span>|<span data-ttu-id="a9501-114">从 Exchange 发现没有访问状态理由</span><span class="sxs-lookup"><span data-stu-id="a9501-114">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="a9501-115">unknown</span><span class="sxs-lookup"><span data-stu-id="a9501-115">unknown</span></span>|<span data-ttu-id="a9501-116">1</span><span class="sxs-lookup"><span data-stu-id="a9501-116">1</span></span>|<span data-ttu-id="a9501-117">未知的访问状态的原因</span><span class="sxs-lookup"><span data-stu-id="a9501-117">Unknown access state reason</span></span>|
|<span data-ttu-id="a9501-118">exchangeGlobalRule</span><span class="sxs-lookup"><span data-stu-id="a9501-118">exchangeGlobalRule</span></span>|<span data-ttu-id="a9501-119">2</span><span class="sxs-lookup"><span data-stu-id="a9501-119">2</span></span>|<span data-ttu-id="a9501-120">由 Exchange 全局规则的访问状态</span><span class="sxs-lookup"><span data-stu-id="a9501-120">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="a9501-121">exchangeIndividualRule</span><span class="sxs-lookup"><span data-stu-id="a9501-121">exchangeIndividualRule</span></span>|<span data-ttu-id="a9501-122">3</span><span class="sxs-lookup"><span data-stu-id="a9501-122">3</span></span>|<span data-ttu-id="a9501-123">由 Exchange 单个规则的访问状态</span><span class="sxs-lookup"><span data-stu-id="a9501-123">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="a9501-124">exchangeDeviceRule</span><span class="sxs-lookup"><span data-stu-id="a9501-124">exchangeDeviceRule</span></span>|<span data-ttu-id="a9501-125">4</span><span class="sxs-lookup"><span data-stu-id="a9501-125">4</span></span>|<span data-ttu-id="a9501-126">由 Exchange 设备规则的访问状态</span><span class="sxs-lookup"><span data-stu-id="a9501-126">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="a9501-127">exchangeUpgrade</span><span class="sxs-lookup"><span data-stu-id="a9501-127">exchangeUpgrade</span></span>|<span data-ttu-id="a9501-128">5</span><span class="sxs-lookup"><span data-stu-id="a9501-128">5</span></span>|<span data-ttu-id="a9501-129">由于 Exchange 升级的访问状态</span><span class="sxs-lookup"><span data-stu-id="a9501-129">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="a9501-130">exchangeMailboxPolicy</span><span class="sxs-lookup"><span data-stu-id="a9501-130">exchangeMailboxPolicy</span></span>|<span data-ttu-id="a9501-131">6</span><span class="sxs-lookup"><span data-stu-id="a9501-131">6</span></span>|<span data-ttu-id="a9501-132">由 Exchange 邮箱策略的访问状态</span><span class="sxs-lookup"><span data-stu-id="a9501-132">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="a9501-133">其他</span><span class="sxs-lookup"><span data-stu-id="a9501-133">other</span></span>|<span data-ttu-id="a9501-134">7</span><span class="sxs-lookup"><span data-stu-id="a9501-134">7</span></span>|<span data-ttu-id="a9501-135">由 Exchange 的访问状态</span><span class="sxs-lookup"><span data-stu-id="a9501-135">Access state determined by Exchange</span></span>|
|<span data-ttu-id="a9501-136">符合标准</span><span class="sxs-lookup"><span data-stu-id="a9501-136">compliant</span></span>|<span data-ttu-id="a9501-137">8</span><span class="sxs-lookup"><span data-stu-id="a9501-137">8</span></span>|<span data-ttu-id="a9501-138">通过合规性质询授予的访问状态</span><span class="sxs-lookup"><span data-stu-id="a9501-138">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="a9501-139">notCompliant</span><span class="sxs-lookup"><span data-stu-id="a9501-139">notCompliant</span></span>|<span data-ttu-id="a9501-140">9</span><span class="sxs-lookup"><span data-stu-id="a9501-140">9</span></span>|<span data-ttu-id="a9501-141">合规性质询被吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="a9501-141">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="a9501-142">notEnrolled</span><span class="sxs-lookup"><span data-stu-id="a9501-142">notEnrolled</span></span>|<span data-ttu-id="a9501-143">10</span><span class="sxs-lookup"><span data-stu-id="a9501-143">10</span></span>|<span data-ttu-id="a9501-144">管理质询被吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="a9501-144">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="a9501-145">unknownLocation</span><span class="sxs-lookup"><span data-stu-id="a9501-145">unknownLocation</span></span>|<span data-ttu-id="a9501-146">12</span><span class="sxs-lookup"><span data-stu-id="a9501-146">12</span></span>|<span data-ttu-id="a9501-147">由于未知位置的访问状态</span><span class="sxs-lookup"><span data-stu-id="a9501-147">Access state due to unknown location</span></span>|
|<span data-ttu-id="a9501-148">mfaRequired</span><span class="sxs-lookup"><span data-stu-id="a9501-148">mfaRequired</span></span>|<span data-ttu-id="a9501-149">13</span><span class="sxs-lookup"><span data-stu-id="a9501-149">13</span></span>|<span data-ttu-id="a9501-150">由于 MFA 质询的访问状态</span><span class="sxs-lookup"><span data-stu-id="a9501-150">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="a9501-151">azureADBlockDueToAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="a9501-151">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="a9501-152">14</span><span class="sxs-lookup"><span data-stu-id="a9501-152">14</span></span>|<span data-ttu-id="a9501-153">由 AAD 访问策略吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="a9501-153">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="a9501-154">compromisedPassword</span><span class="sxs-lookup"><span data-stu-id="a9501-154">compromisedPassword</span></span>|<span data-ttu-id="a9501-155">15</span><span class="sxs-lookup"><span data-stu-id="a9501-155">15</span></span>|<span data-ttu-id="a9501-156">由受到攻击的密码吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="a9501-156">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="a9501-157">deviceNotKnownWithManagedApp</span><span class="sxs-lookup"><span data-stu-id="a9501-157">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="a9501-158">16</span><span class="sxs-lookup"><span data-stu-id="a9501-158">16</span></span>|<span data-ttu-id="a9501-159">由托管应用程序质询吊销的访问状态</span><span class="sxs-lookup"><span data-stu-id="a9501-159">Access state revoked by managed application challenge</span></span>|




