---
title: 使用 Microsoft Intune 管理移动应用-Microsoft Graph API
description: 列出与租户组织的移动应用管理 (MAM) 相关的适用于 Intune 终结点 (REST) 的 Microsoft Graph API。
author: dougeby
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 62a3b0e9751acaa552dc1deed037bb3356cfce0b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702388"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a><span data-ttu-id="7ad49-103">如何通过 Microsoft Intune 保护公司的应用数据</span><span class="sxs-lookup"><span data-stu-id="7ad49-103">How to protect your company app data with Microsoft Intune</span></span>

<span data-ttu-id="7ad49-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ad49-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ad49-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7ad49-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ad49-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7ad49-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ad49-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7ad49-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ad49-108">Microsoft Intune 应用保护策略可帮助保护公司数据，避免数据丢失。</span><span class="sxs-lookup"><span data-stu-id="7ad49-108">Microsoft Intune app protection policies help protect your company data and prevent data loss.</span></span>

<span data-ttu-id="7ad49-109">你可以使用 Intune 应用保护策略帮助保护公司的数据。</span><span class="sxs-lookup"><span data-stu-id="7ad49-109">You can use Intune app protection policies to help protect your company’s data.</span></span> <span data-ttu-id="7ad49-110">由于 Intune 应用保护策略可独立于任何移动设备管理 (MDM) 解决方案使用，因此您可以使用它在设备管理解决方案中使用或不注册设备来保护公司的数据。</span><span class="sxs-lookup"><span data-stu-id="7ad49-110">Because Intune app protection policies can be used independent of any mobile-device management (MDM) solution, you can use it to protect your company’s data with or without enrolling devices in a device management solution.</span></span> <span data-ttu-id="7ad49-111">通过实现应用级策略，既可以限制对公司资源的访问，也可以将数据保留在 IT 部门的范围之内。</span><span class="sxs-lookup"><span data-stu-id="7ad49-111">By implementing app-level policies, you can restrict access to company resources and keep data within the purview of your IT department.</span></span>

<span data-ttu-id="7ad49-112">以下 Graph 资源可用于在 Intune 中管理应用保护策略：</span><span class="sxs-lookup"><span data-stu-id="7ad49-112">The following Graph resources are available to manage app protection polices in Intune:</span></span>

- [<span data-ttu-id="7ad49-113">Android 管理的应用注册</span><span class="sxs-lookup"><span data-stu-id="7ad49-113">Android managed app registration</span></span>](intune-mam-androidmanagedappregistration.md)
- [<span data-ttu-id="7ad49-114">Android 托管应用安全网络应用验证类型</span><span class="sxs-lookup"><span data-stu-id="7ad49-114">Android managed app safety net apps verification type</span></span>](intune-mam-androidmanagedappsafetynetappsverificationtype.md)
- [<span data-ttu-id="7ad49-115">Android 托管应用安全网络设备证明类型</span><span class="sxs-lookup"><span data-stu-id="7ad49-115">Android managed app safety net device attestation type</span></span>](intune-mam-androidmanagedappsafetynetdeviceattestationtype.md)
- [<span data-ttu-id="7ad49-116">Android 托管应用安全 net 评估类型</span><span class="sxs-lookup"><span data-stu-id="7ad49-116">Android managed app safety net evaluation type</span></span>](intune-mam-androidmanagedappsafetynetevaluationtype.md)
- [<span data-ttu-id="7ad49-117">Android 移动应用标识符</span><span class="sxs-lookup"><span data-stu-id="7ad49-117">Android mobile app identifier</span></span>](intune-mam-androidmobileappidentifier.md)
- [<span data-ttu-id="7ad49-118">应用管理级别</span><span class="sxs-lookup"><span data-stu-id="7ad49-118">App management level</span></span>](intune-mam-appmanagementlevel.md)
- [<span data-ttu-id="7ad49-119">应用程序类型</span><span class="sxs-lookup"><span data-stu-id="7ad49-119">Application type</span></span>](intune-wip-applicationtype.md)
- [<span data-ttu-id="7ad49-120">默认托管的应用保护</span><span class="sxs-lookup"><span data-stu-id="7ad49-120">Default managed app protection</span></span>](intune-mam-defaultmanagedappprotection.md)
- [<span data-ttu-id="7ad49-121">Intune 品牌打造配置文件</span><span class="sxs-lookup"><span data-stu-id="7ad49-121">Intune branding profile</span></span>](intune-wip-intunebrandingprofile.md)
- [<span data-ttu-id="7ad49-122">Intune 品牌打造配置文件分配</span><span class="sxs-lookup"><span data-stu-id="7ad49-122">Intune branding profile assignment</span></span>](intune-wip-intunebrandingprofileassignment.md)
- [<span data-ttu-id="7ad49-123">iOS 管理的应用注册</span><span class="sxs-lookup"><span data-stu-id="7ad49-123">iOS managed app registration</span></span>](intune-mam-iosmanagedappregistration.md)
- [<span data-ttu-id="7ad49-124">iOS 移动应用标识符</span><span class="sxs-lookup"><span data-stu-id="7ad49-124">iOS mobile app identifier</span></span>](intune-mam-iosmobileappidentifier.md)
- [<span data-ttu-id="7ad49-125">JSON</span><span class="sxs-lookup"><span data-stu-id="7ad49-125">JSON</span></span>](intune-mam-json.md)
- [<span data-ttu-id="7ad49-126">受管理的应用剪贴板共享级别</span><span class="sxs-lookup"><span data-stu-id="7ad49-126">Managed app clipboard sharing level</span></span>](intune-mam-managedappclipboardsharinglevel.md)
- [<span data-ttu-id="7ad49-127">托管的应用配置</span><span class="sxs-lookup"><span data-stu-id="7ad49-127">Managed app configuration</span></span>](intune-mam-managedappconfiguration.md)
- [<span data-ttu-id="7ad49-128">受管理应用的数据加密类型</span><span class="sxs-lookup"><span data-stu-id="7ad49-128">Managed app data encryption type</span></span>](intune-mam-managedappdataencryptiontype.md)
- [<span data-ttu-id="7ad49-129">托管应用数据摄取位置</span><span class="sxs-lookup"><span data-stu-id="7ad49-129">Managed app data ingestion location</span></span>](intune-mam-managedappdataingestionlocation.md)
- [<span data-ttu-id="7ad49-130">受管理应用的数据存储位置</span><span class="sxs-lookup"><span data-stu-id="7ad49-130">Managed app data storage location</span></span>](intune-mam-managedappdatastoragelocation.md)
- [<span data-ttu-id="7ad49-131">受管理应用的数据传输级别</span><span class="sxs-lookup"><span data-stu-id="7ad49-131">Managed app data transfer level</span></span>](intune-mam-managedappdatatransferlevel.md)
- [<span data-ttu-id="7ad49-132">托管应用设备威胁级别</span><span class="sxs-lookup"><span data-stu-id="7ad49-132">Managed app device threat level</span></span>](intune-mam-managedappdevicethreatlevel.md)
- [<span data-ttu-id="7ad49-133">托管的应用诊断状态</span><span class="sxs-lookup"><span data-stu-id="7ad49-133">Managed app diagnostic status</span></span>](intune-mam-managedappdiagnosticstatus.md)
- [<span data-ttu-id="7ad49-134">受管理应用的已标记原因</span><span class="sxs-lookup"><span data-stu-id="7ad49-134">Managed app flagged reason</span></span>](intune-mam-managedappflaggedreason.md)
- [<span data-ttu-id="7ad49-135">托管应用程序通知限制</span><span class="sxs-lookup"><span data-stu-id="7ad49-135">Managed app notification restriction</span></span>](intune-mam-managedappnotificationrestriction.md)
- [<span data-ttu-id="7ad49-136">托管的应用操作</span><span class="sxs-lookup"><span data-stu-id="7ad49-136">Managed app operation</span></span>](intune-mam-managedappoperation.md)
- [<span data-ttu-id="7ad49-137">托管应用电话号码重定向级别</span><span class="sxs-lookup"><span data-stu-id="7ad49-137">Managed app phone number redirect level</span></span>](intune-mam-managedappphonenumberredirectlevel.md)
- [<span data-ttu-id="7ad49-138">托管的应用 PIN 字符集</span><span class="sxs-lookup"><span data-stu-id="7ad49-138">Managed app PIN character set</span></span>](intune-mam-managedapppincharacterset.md)
- [<span data-ttu-id="7ad49-139">托管的应用策略</span><span class="sxs-lookup"><span data-stu-id="7ad49-139">Managed app policy</span></span>](intune-mam-managedapppolicy.md)
- [<span data-ttu-id="7ad49-140">托管应用策略部署摘要</span><span class="sxs-lookup"><span data-stu-id="7ad49-140">Managed app policy deployment summary</span></span>](intune-mam-managedapppolicydeploymentsummary.md)
- [<span data-ttu-id="7ad49-141">每个应用的托管应用策略部署摘要</span><span class="sxs-lookup"><span data-stu-id="7ad49-141">Managed app policy deployment summary per app</span></span>](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [<span data-ttu-id="7ad49-142">托管的应用保护</span><span class="sxs-lookup"><span data-stu-id="7ad49-142">Managed app protection</span></span>](intune-mam-managedappprotection.md)
- [<span data-ttu-id="7ad49-143">托管应用注册</span><span class="sxs-lookup"><span data-stu-id="7ad49-143">Managed app registration</span></span>](intune-mam-managedappregistration.md)
- [<span data-ttu-id="7ad49-144">托管的应用修正操作</span><span class="sxs-lookup"><span data-stu-id="7ad49-144">Managed app remediation action</span></span>](intune-mam-managedappremediationaction.md)
- [<span data-ttu-id="7ad49-145">托管应用状态</span><span class="sxs-lookup"><span data-stu-id="7ad49-145">Managed app status</span></span>](intune-mam-managedappstatus.md)
- [<span data-ttu-id="7ad49-146">托管应用原始状态</span><span class="sxs-lookup"><span data-stu-id="7ad49-146">Managed app status raw</span></span>](intune-mam-managedappstatusraw.md)
- [<span data-ttu-id="7ad49-147">托管浏览器类型</span><span class="sxs-lookup"><span data-stu-id="7ad49-147">Managed browser type</span></span>](intune-mam-managedbrowsertype.md)
- [<span data-ttu-id="7ad49-148">托管移动应用</span><span class="sxs-lookup"><span data-stu-id="7ad49-148">Managed mobile app</span></span>](intune-mam-managedmobileapp.md)
- [<span data-ttu-id="7ad49-149">移动应用标识符</span><span class="sxs-lookup"><span data-stu-id="7ad49-149">Mobile app identifier</span></span>](intune-mam-mobileappidentifier.md)
- [<span data-ttu-id="7ad49-150">目标托管应用程序策略分配</span><span class="sxs-lookup"><span data-stu-id="7ad49-150">Targeted managed app policy assignment</span></span>](intune-mam-targetedmanagedapppolicyassignment.md)
- [<span data-ttu-id="7ad49-151">目标托管应用保护</span><span class="sxs-lookup"><span data-stu-id="7ad49-151">Targeted managed app protection</span></span>](intune-mam-targetedmanagedappprotection.md)
- [<span data-ttu-id="7ad49-152">Windows 信息保护</span><span class="sxs-lookup"><span data-stu-id="7ad49-152">Windows information protection</span></span>](intune-mam-windowsinformationprotection.md)
- [<span data-ttu-id="7ad49-153">Windows 信息保护应用</span><span class="sxs-lookup"><span data-stu-id="7ad49-153">Windows information protection app</span></span>](intune-mam-windowsinformationprotectionapp.md)
- [<span data-ttu-id="7ad49-154">Windows 信息保护应用学习摘要</span><span class="sxs-lookup"><span data-stu-id="7ad49-154">Windows information protection app learning summary</span></span>](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [<span data-ttu-id="7ad49-155">Windows 信息保护应用锁定程序文件</span><span class="sxs-lookup"><span data-stu-id="7ad49-155">Windows information protection app locker file</span></span>](intune-mam-windowsinformationprotectionapplockerfile.md)
- [<span data-ttu-id="7ad49-156">Windows 信息保护数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="7ad49-156">Windows information protection data recovery certificate</span></span>](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [<span data-ttu-id="7ad49-157">Windows 信息保护桌面应用</span><span class="sxs-lookup"><span data-stu-id="7ad49-157">Windows information protection desktop app</span></span>](intune-mam-windowsinformationprotectiondesktopapp.md)
- [<span data-ttu-id="7ad49-158">Windows 信息保护设备注册</span><span class="sxs-lookup"><span data-stu-id="7ad49-158">Windows information protection device registration</span></span>](intune-mam-windowsinformationprotectiondeviceregistration.md)
- [<span data-ttu-id="7ad49-159">Windows 信息保护强制级别</span><span class="sxs-lookup"><span data-stu-id="7ad49-159">Windows information protection enforcement level</span></span>](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [<span data-ttu-id="7ad49-160">Windows 信息保护 IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="7ad49-160">Windows information protection IP range collection</span></span>](intune-mam-windowsinformationprotectioniprangecollection.md)
- [<span data-ttu-id="7ad49-161">Windows 信息保护网络学习摘要</span><span class="sxs-lookup"><span data-stu-id="7ad49-161">Windows information protection network learning summary</span></span>](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [<span data-ttu-id="7ad49-162">Windows 信息保护 PIN 字符要求</span><span class="sxs-lookup"><span data-stu-id="7ad49-162">Windows information protection PIN character requirements</span></span>](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [<span data-ttu-id="7ad49-163">Windows 信息保护策略</span><span class="sxs-lookup"><span data-stu-id="7ad49-163">Windows information protection policy</span></span>](intune-mam-windowsinformationprotectionpolicy.md)
- [<span data-ttu-id="7ad49-164">Windows 信息保护代理域集合</span><span class="sxs-lookup"><span data-stu-id="7ad49-164">Windows information protection proxied domain collection</span></span>](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [<span data-ttu-id="7ad49-165">Windows 信息保护资源集合</span><span class="sxs-lookup"><span data-stu-id="7ad49-165">Windows information protection resource collection</span></span>](intune-mam-windowsinformationprotectionresourcecollection.md)
- [<span data-ttu-id="7ad49-166">Windows 信息保护应用商店应用</span><span class="sxs-lookup"><span data-stu-id="7ad49-166">Windows information protection store app</span></span>](intune-mam-windowsinformationprotectionstoreapp.md)
- [<span data-ttu-id="7ad49-167">Windows 信息保护擦除操作</span><span class="sxs-lookup"><span data-stu-id="7ad49-167">Windows information protection wipe action</span></span>](intune-mam-windowsinformationprotectionwipeaction.md)