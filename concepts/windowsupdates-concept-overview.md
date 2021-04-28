---
title: Windows更新 API 概述
description: 适用于Windows更新部署服务可让你的组织控制提供给你的设备的更新。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 98b75f278e33f56cf726a18c266000b06d817a6f
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067667"
---
# <a name="windows-updates-api-overview"></a><span data-ttu-id="8bf8f-103">Windows更新 API 概述</span><span class="sxs-lookup"><span data-stu-id="8bf8f-103">Windows updates API overview</span></span>

<span data-ttu-id="8bf8f-104">the Windows Update for Business deployment service provides control over device updates through the ability to approve， schedule and safeguard content delivered by Windows Update.</span><span class="sxs-lookup"><span data-stu-id="8bf8f-104">The Windows Update for Business deployment service provides control over device updates through the ability to approve, schedule and safeguard content delivered by Windows Update.</span></span> 

## <a name="why-use-the-windows-update-for-business-deployment-service"></a><span data-ttu-id="8bf8f-105">为什么使用 Windows Update for Business 部署服务？</span><span class="sxs-lookup"><span data-stu-id="8bf8f-105">Why use the Windows Update for Business deployment service?</span></span>

<span data-ttu-id="8bf8f-106">IT 专业人员和管理工具供应商都可以使用部署服务：</span><span class="sxs-lookup"><span data-stu-id="8bf8f-106">IT Professionals and management tool vendors alike can use the deployment service to:</span></span>
* <span data-ttu-id="8bf8f-107">将更新部署安排在特定的日期开始</span><span class="sxs-lookup"><span data-stu-id="8bf8f-107">Schedule update deployments to begin on a specific date</span></span>
* <span data-ttu-id="8bf8f-108">使用富表达式在几天或几周内阶段部署</span><span class="sxs-lookup"><span data-stu-id="8bf8f-108">Stage deployments over a period of days or weeks using rich expressions</span></span>
* <span data-ttu-id="8bf8f-109">绕过预配置的 Windows 更新 for Business 策略以立即部署安全更新</span><span class="sxs-lookup"><span data-stu-id="8bf8f-109">Bypass pre-configured Windows Update for Business policies to immediately deploy a security update</span></span>
* <span data-ttu-id="8bf8f-110">通过针对唯一设备总体部署定制的部署，确保组织中硬件和软件 (范围) </span><span class="sxs-lookup"><span data-stu-id="8bf8f-110">Ensure coverage of hardware and software in your organization through deployments tailored to unique device population(s)</span></span>

<span data-ttu-id="8bf8f-111">现在，部署服务支持管理Windows 10功能更新和Windows 10安全更新。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-111">Today, the deployment service supports managing Windows 10 feature updates and expediting Windows 10 security updates.</span></span> <span data-ttu-id="8bf8f-112">若要了解有关企业更新上下文中的部署服务Windows，请参阅[部署服务概述](https://docs.microsoft.com/windows/deployment/update/deployment-service-overview)。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-112">To learn more about the deployment service in the context of Windows Update for Business, please see [Overview of the deployment service](https://docs.microsoft.com/windows/deployment/update/deployment-service-overview).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8bf8f-113">先决条件</span><span class="sxs-lookup"><span data-stu-id="8bf8f-113">Prerequisites</span></span>    

<span data-ttu-id="8bf8f-114">若要使用部署服务，组织必须拥有以下订阅之一：</span><span class="sxs-lookup"><span data-stu-id="8bf8f-114">To use the deployment service, your organization must have one of the following subscriptions:</span></span>
* <span data-ttu-id="8bf8f-115">Windows 10 企业版E3 或 E5 (包含在 Microsoft 365 F3、E3 或 E5) </span><span class="sxs-lookup"><span data-stu-id="8bf8f-115">Windows 10 Enterprise E3 or E5 (included in Microsoft 365 F3, E3, or E5)</span></span>
* <span data-ttu-id="8bf8f-116">Windows 10 教育版A3 或 A5 (A3 或 A5 Microsoft 365中) </span><span class="sxs-lookup"><span data-stu-id="8bf8f-116">Windows 10 Education A3 or A5 (included in Microsoft 365 A3 or A5)</span></span>
* <span data-ttu-id="8bf8f-117">Windows虚拟桌面访问 E3 或 E5</span><span class="sxs-lookup"><span data-stu-id="8bf8f-117">Windows Virtual Desktop Access E3 or E5</span></span>
* <span data-ttu-id="8bf8f-118">Microsoft 365 商业高级版</span><span class="sxs-lookup"><span data-stu-id="8bf8f-118">Microsoft 365 Business Premium</span></span>

<span data-ttu-id="8bf8f-119">此外，部署服务管理的设备必须：</span><span class="sxs-lookup"><span data-stu-id="8bf8f-119">Additionally, devices managed by the deployment service must:</span></span>
* <span data-ttu-id="8bf8f-120">加入 Azure AD 或加入混合 AD</span><span class="sxs-lookup"><span data-stu-id="8bf8f-120">Be Azure AD joined or Hybrid AD joined</span></span>
* <span data-ttu-id="8bf8f-121">运行下列版本之一Windows 10：Windows 10 专业版、Windows 10 企业版、Windows 10 教育版、Windows 10 专业教育版</span><span class="sxs-lookup"><span data-stu-id="8bf8f-121">Run one of the following Windows 10 editions: Windows 10 Pro, Windows 10 Enterprise, Windows 10 Education, Windows 10 Pro Education</span></span>
* <span data-ttu-id="8bf8f-122">已安装Windows 10版本 1709 或更高版本</span><span class="sxs-lookup"><span data-stu-id="8bf8f-122">Have installed Windows 10 version 1709 or later</span></span>

## <a name="enroll-devices-to-be-managed"></a><span data-ttu-id="8bf8f-123">注册要管理的设备</span><span class="sxs-lookup"><span data-stu-id="8bf8f-123">Enroll devices to be managed</span></span>

<span data-ttu-id="8bf8f-124">若要开始使用部署服务， [请注册更新管理中的设备](windowsupdates-enroll.md)。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-124">To start using the deployment service, [enroll devices in update management](windowsupdates-enroll.md).</span></span>

## <a name="approve-and-schedule-windows-content-delivered-from-windows-update"></a><span data-ttu-id="8bf8f-125">批准和安排Windows更新中Windows的内容</span><span class="sxs-lookup"><span data-stu-id="8bf8f-125">Approve and schedule Windows content delivered from Windows Update</span></span>

<span data-ttu-id="8bf8f-126">部署服务简化了针对各种设备生态系统的审阅、批准、计划和部署内容。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-126">The deployment service simplifies reviewing, approving, scheduling, and deploying content for a diverse device ecosystem.</span></span> <span data-ttu-id="8bf8f-127">存在更新目录以提供专为审批定制的视图，帮助您重点关注重要的审批决策，并避免需要对相关更新的深入列表进行排序。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-127">An updates catalog exists to provide a view tailored for approvals, helping you focus on approval decisions that matter and avoiding the need to sort through deep lists of related updates.</span></span>

<span data-ttu-id="8bf8f-128">选择要部署的更新后，可以将部署安排为在将来开始，或在一定时段内部署。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-128">Once you choose an update to deploy, you can schedule deployments to start at a future time, or deploy over a period of time.</span></span> <span data-ttu-id="8bf8f-129">如果选择在一段时间内部署更新，部署服务将自动优化设备提供更新的顺序。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-129">If you choose to deploy an update over a period of time, the deployment service automatically optimizes the order in which devices are offered updates.</span></span> <span data-ttu-id="8bf8f-130">如果可能，该服务对设备进行订购，以确保在部署早期表示硬件和软件资产的多样性，以最大限度地减少可能遇到意外更新问题的设备数量。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-130">When possible, the service orders devices to ensure that a diversity of hardware and software assets are represented early in the deployment to minimize the number of devices that may encounter an unexpected update issue.</span></span> 

<span data-ttu-id="8bf8f-131">详细了解部署服务：</span><span class="sxs-lookup"><span data-stu-id="8bf8f-131">Learn more about the deployment service:</span></span>
* [<span data-ttu-id="8bf8f-132">软件更新</span><span class="sxs-lookup"><span data-stu-id="8bf8f-132">Software updates</span></span>](windowsupdates-software-updates.md)
* [<span data-ttu-id="8bf8f-133">部署</span><span class="sxs-lookup"><span data-stu-id="8bf8f-133">Deployments</span></span>](windowsupdates-deployments.md)
* [<span data-ttu-id="8bf8f-134">计划部署</span><span class="sxs-lookup"><span data-stu-id="8bf8f-134">Schedule a deployment</span></span>](windowsupdates-schedule-deployment.md)

## <a name="immediately-deploy-an-update-when-critical-needs-arise"></a><span data-ttu-id="8bf8f-135">出现关键需求时立即部署更新</span><span class="sxs-lookup"><span data-stu-id="8bf8f-135">Immediately deploy an update when critical needs arise</span></span>

<span data-ttu-id="8bf8f-136">在出现关键安全问题的情况下，可以使用部署服务绕过标准更新策略并加快安全更新的部署。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-136">In the case of a critical security issue, you can use the deployment service to bypass a standard update policy and expedite deployment of a security update.</span></span>

<span data-ttu-id="8bf8f-137">若要了解更多信息，请参阅 [部署加速安全更新](windowsupdates-deploy-expedited-update.md)。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-137">To learn more, see [Deploy an expedited security update](windowsupdates-deploy-expedited-update.md).</span></span>

## <a name="protect-devices-by-default"></a><span data-ttu-id="8bf8f-138">默认情况下保护设备</span><span class="sxs-lookup"><span data-stu-id="8bf8f-138">Protect devices by default</span></span>

<span data-ttu-id="8bf8f-139">享受保护 [保留的好处](https://docs.microsoft.com/windows/deployment/update/safeguard-holds) ，防止出现质量或兼容性问题的设备安装更新，否则导致失败或回滚。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-139">Enjoy the benefit of [safeguard holds](https://docs.microsoft.com/windows/deployment/update/safeguard-holds) which prevent devices with a quality or compatibility issue from installing an update, resulting in failure or rollback otherwise.</span></span>

<span data-ttu-id="8bf8f-140">此外，还可以配置组织独有的监视规则。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-140">Additionally, you can configure monitoring rules that are unique to your organization.</span></span> <span data-ttu-id="8bf8f-141">这些规则可以基于设备信号（如回滚）发送警报或暂停部署。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-141">These rules can send an alert or pause a deployment based on device signals such as rollbacks.</span></span>

<span data-ttu-id="8bf8f-142">若要了解更多信息，请参阅 [管理部署的监视规则](windowsupdates-manage-monitoring-rules.md)。</span><span class="sxs-lookup"><span data-stu-id="8bf8f-142">To learn more, see [Manage monitoring rules for a deployment](windowsupdates-manage-monitoring-rules.md).</span></span>

## <a name="api-reference"></a><span data-ttu-id="8bf8f-143">API 参考</span><span class="sxs-lookup"><span data-stu-id="8bf8f-143">API reference</span></span>

<span data-ttu-id="8bf8f-144">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="8bf8f-144">Looking for the API reference for this service?</span></span>

<span data-ttu-id="8bf8f-145">请参阅[microsoft Windows beta 中的 Graph 更新 API。](/graph/api/resources/windowsupdates-updates?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="8bf8f-145">See [Windows updates API in Microsoft Graph beta](/graph/api/resources/windowsupdates-updates?view=graph-rest-beta&preserve-view=true).</span></span>
