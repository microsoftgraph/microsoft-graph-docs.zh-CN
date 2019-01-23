---
title: 如何通过 Microsoft Intune 保护公司的应用数据
description: Microsoft Intune 应用保护策略可帮助保护公司数据，避免数据丢失。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 563f787f2eb37b278a16c35639e0d607d3d9ee68
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419000"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a><span data-ttu-id="ceaa2-103">如何通过 Microsoft Intune 保护公司的应用数据</span><span class="sxs-lookup"><span data-stu-id="ceaa2-103">How to protect your company app data with Microsoft Intune</span></span>

> <span data-ttu-id="ceaa2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ceaa2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ceaa2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ceaa2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ceaa2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ceaa2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="ceaa2-107">Microsoft Intune 应用保护策略可帮助保护公司数据，避免数据丢失。</span><span class="sxs-lookup"><span data-stu-id="ceaa2-107">Microsoft Intune app protection policies help protect your company data and prevent data loss.</span></span>

<span data-ttu-id="ceaa2-108">你可以使用 Intune 应用保护策略帮助保护公司的数据。</span><span class="sxs-lookup"><span data-stu-id="ceaa2-108">You can use Intune app protection policies to help protect your company’s data.</span></span> <span data-ttu-id="ceaa2-109">因为 Intune 应用程序保护策略可用于独立于任何移动设备管理 (MDM) 解决方案，可用于保护贵公司的数据使用或不注册设备的设备管理解决方案中。</span><span class="sxs-lookup"><span data-stu-id="ceaa2-109">Because Intune app protection policies can be used independent of any mobile-device management (MDM) solution, you can use it to protect your company’s data with or without enrolling devices in a device management solution.</span></span> <span data-ttu-id="ceaa2-110">通过实现应用级策略，既可以限制对公司资源的访问，也可以将数据保留在 IT 部门的范围之内。</span><span class="sxs-lookup"><span data-stu-id="ceaa2-110">By implementing app-level policies, you can restrict access to company resources and keep data within the purview of your IT department.</span></span>

<span data-ttu-id="ceaa2-111">以下 Graph 资源可用于在 Intune 中管理应用保护策略：</span><span class="sxs-lookup"><span data-stu-id="ceaa2-111">The following Graph resources are available to manage app protection polices in Intune:</span></span>

- [<span data-ttu-id="ceaa2-112">Android 管理的应用保护</span><span class="sxs-lookup"><span data-stu-id="ceaa2-112">Android managed app protection</span></span>](intune-mam-androidmanagedappprotection.md)
- [<span data-ttu-id="ceaa2-113">Android 管理的应用注册</span><span class="sxs-lookup"><span data-stu-id="ceaa2-113">Android managed app registration</span></span>](intune-mam-androidmanagedappregistration.md)
- [<span data-ttu-id="ceaa2-114">Android 移动应用标识符</span><span class="sxs-lookup"><span data-stu-id="ceaa2-114">Android mobile app identifier</span></span>](intune-mam-androidmobileappidentifier.md)
- [<span data-ttu-id="ceaa2-115">应用程序管理级别</span><span class="sxs-lookup"><span data-stu-id="ceaa2-115">App management level</span></span>](intune-mam-appmanagementlevel.md)
- [<span data-ttu-id="ceaa2-116">应用程序类型</span><span class="sxs-lookup"><span data-stu-id="ceaa2-116">Application type</span></span>](intune-wip-applicationtype.md)
- [<span data-ttu-id="ceaa2-117">默认托管的应用保护</span><span class="sxs-lookup"><span data-stu-id="ceaa2-117">Default managed app protection</span></span>](intune-mam-defaultmanagedappprotection.md)
- [<span data-ttu-id="ceaa2-118">Intune 品牌配置文件</span><span class="sxs-lookup"><span data-stu-id="ceaa2-118">Intune branding profile</span></span>](intune-wip-intunebrandingprofile.md)
- [<span data-ttu-id="ceaa2-119">Intune 品牌的配置文件分配</span><span class="sxs-lookup"><span data-stu-id="ceaa2-119">Intune branding profile assignment</span></span>](intune-wip-intunebrandingprofileassignment.md)
- [<span data-ttu-id="ceaa2-120">iOS 管理的应用保护</span><span class="sxs-lookup"><span data-stu-id="ceaa2-120">iOS managed app protection</span></span>](intune-mam-iosmanagedappprotection.md)
- [<span data-ttu-id="ceaa2-121">iOS 管理的应用注册</span><span class="sxs-lookup"><span data-stu-id="ceaa2-121">iOS managed app registration</span></span>](intune-mam-iosmanagedappregistration.md)
- [<span data-ttu-id="ceaa2-122">iOS 移动应用标识符</span><span class="sxs-lookup"><span data-stu-id="ceaa2-122">iOS mobile app identifier</span></span>](intune-mam-iosmobileappidentifier.md)
- [<span data-ttu-id="ceaa2-123">JSON</span><span class="sxs-lookup"><span data-stu-id="ceaa2-123">JSON</span></span>](intune-mam-json.md)
- [<span data-ttu-id="ceaa2-124">托管应用程序剪贴板共享级别</span><span class="sxs-lookup"><span data-stu-id="ceaa2-124">Managed app clipboard sharing level</span></span>](intune-mam-managedappclipboardsharinglevel.md)
- [<span data-ttu-id="ceaa2-125">托管的应用配置</span><span class="sxs-lookup"><span data-stu-id="ceaa2-125">Managed app configuration</span></span>](intune-mam-managedappconfiguration.md)
- [<span data-ttu-id="ceaa2-126">托管应用程序数据的加密类型</span><span class="sxs-lookup"><span data-stu-id="ceaa2-126">Managed app data encryption type</span></span>](intune-mam-managedappdataencryptiontype.md)
- [<span data-ttu-id="ceaa2-127">托管的应用程序数据存储位置</span><span class="sxs-lookup"><span data-stu-id="ceaa2-127">Managed app data storage location</span></span>](intune-mam-managedappdatastoragelocation.md)
- [<span data-ttu-id="ceaa2-128">托管的应用程序数据传输级别</span><span class="sxs-lookup"><span data-stu-id="ceaa2-128">Managed app data transfer level</span></span>](intune-mam-managedappdatatransferlevel.md)
- [<span data-ttu-id="ceaa2-129">托管的应用诊断状态</span><span class="sxs-lookup"><span data-stu-id="ceaa2-129">Managed app diagnostic status</span></span>](intune-mam-managedappdiagnosticstatus.md)
- [<span data-ttu-id="ceaa2-130">托管的应用程序标记原因</span><span class="sxs-lookup"><span data-stu-id="ceaa2-130">Managed app flagged reason</span></span>](intune-mam-managedappflaggedreason.md)
- [<span data-ttu-id="ceaa2-131">托管的应用操作</span><span class="sxs-lookup"><span data-stu-id="ceaa2-131">Managed app operation</span></span>](intune-mam-managedappoperation.md)
- [<span data-ttu-id="ceaa2-132">托管的应用程序 PIN 字符集。</span><span class="sxs-lookup"><span data-stu-id="ceaa2-132">Managed app PIN character set</span></span>](intune-mam-managedapppincharacterset.md)
- [<span data-ttu-id="ceaa2-133">托管的应用策略</span><span class="sxs-lookup"><span data-stu-id="ceaa2-133">Managed app policy</span></span>](intune-mam-managedapppolicy.md)
- [<span data-ttu-id="ceaa2-134">托管应用策略部署摘要</span><span class="sxs-lookup"><span data-stu-id="ceaa2-134">Managed app policy deployment summary</span></span>](intune-mam-managedapppolicydeploymentsummary.md)
- [<span data-ttu-id="ceaa2-135">每个应用的托管应用策略部署摘要</span><span class="sxs-lookup"><span data-stu-id="ceaa2-135">Managed app policy deployment summary per app</span></span>](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [<span data-ttu-id="ceaa2-136">托管的应用保护</span><span class="sxs-lookup"><span data-stu-id="ceaa2-136">Managed app protection</span></span>](intune-mam-managedappprotection.md)
- [<span data-ttu-id="ceaa2-137">托管应用注册</span><span class="sxs-lookup"><span data-stu-id="ceaa2-137">Managed app registration</span></span>](intune-mam-managedappregistration.md)
- [<span data-ttu-id="ceaa2-138">托管的应用程序修复操作</span><span class="sxs-lookup"><span data-stu-id="ceaa2-138">Managed app remediation action</span></span>](intune-mam-managedappremediationaction.md)
- [<span data-ttu-id="ceaa2-139">托管应用状态</span><span class="sxs-lookup"><span data-stu-id="ceaa2-139">Managed app status</span></span>](intune-mam-managedappstatus.md)
- [<span data-ttu-id="ceaa2-140">托管应用原始状态</span><span class="sxs-lookup"><span data-stu-id="ceaa2-140">Managed app status raw</span></span>](intune-mam-managedappstatusraw.md)
- [<span data-ttu-id="ceaa2-141">托管移动应用</span><span class="sxs-lookup"><span data-stu-id="ceaa2-141">Managed mobile app</span></span>](intune-mam-managedmobileapp.md)
- [<span data-ttu-id="ceaa2-142">MDM Windows 信息保护策略</span><span class="sxs-lookup"><span data-stu-id="ceaa2-142">MDM windows information protection policy</span></span>](intune-mam-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="ceaa2-143">移动应用标识符</span><span class="sxs-lookup"><span data-stu-id="ceaa2-143">Mobile app identifier</span></span>](intune-mam-mobileappidentifier.md)
- [<span data-ttu-id="ceaa2-144">目标托管应用配置</span><span class="sxs-lookup"><span data-stu-id="ceaa2-144">Targeted managed app configuration</span></span>](intune-mam-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="ceaa2-145">目标托管应用程序策略分配</span><span class="sxs-lookup"><span data-stu-id="ceaa2-145">Targeted managed app policy assignment</span></span>](intune-mam-targetedmanagedapppolicyassignment.md)
- [<span data-ttu-id="ceaa2-146">目标托管应用保护</span><span class="sxs-lookup"><span data-stu-id="ceaa2-146">Targeted managed app protection</span></span>](intune-mam-targetedmanagedappprotection.md)
- [<span data-ttu-id="ceaa2-147">Windows 信息保护</span><span class="sxs-lookup"><span data-stu-id="ceaa2-147">Windows information protection</span></span>](intune-mam-windowsinformationprotection.md)
- [<span data-ttu-id="ceaa2-148">Windows 信息保护应用</span><span class="sxs-lookup"><span data-stu-id="ceaa2-148">Windows information protection app</span></span>](intune-mam-windowsinformationprotectionapp.md)
- [<span data-ttu-id="ceaa2-149">Windows 信息保护应用学习摘要</span><span class="sxs-lookup"><span data-stu-id="ceaa2-149">Windows information protection app learning summary</span></span>](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [<span data-ttu-id="ceaa2-150">Windows 信息保护应用锁定程序文件</span><span class="sxs-lookup"><span data-stu-id="ceaa2-150">Windows information protection app locker file</span></span>](intune-mam-windowsinformationprotectionapplockerfile.md)
- [<span data-ttu-id="ceaa2-151">Windows 信息保护数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="ceaa2-151">Windows information protection data recovery certificate</span></span>](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [<span data-ttu-id="ceaa2-152">Windows 信息保护桌面应用</span><span class="sxs-lookup"><span data-stu-id="ceaa2-152">Windows information protection desktop app</span></span>](intune-mam-windowsinformationprotectiondesktopapp.md)
- [<span data-ttu-id="ceaa2-153">Windows 信息保护设备注册</span><span class="sxs-lookup"><span data-stu-id="ceaa2-153">Windows information protection device registration</span></span>](intune-mam-windowsinformationprotectiondeviceregistration.md)
- [<span data-ttu-id="ceaa2-154">Windows 的信息保护实施级别</span><span class="sxs-lookup"><span data-stu-id="ceaa2-154">Windows information protection enforcement level</span></span>](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [<span data-ttu-id="ceaa2-155">Windows 信息保护 IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="ceaa2-155">Windows information protection IP range collection</span></span>](intune-mam-windowsinformationprotectioniprangecollection.md)
- [<span data-ttu-id="ceaa2-156">Windows 信息保护网络学习摘要</span><span class="sxs-lookup"><span data-stu-id="ceaa2-156">Windows information protection network learning summary</span></span>](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [<span data-ttu-id="ceaa2-157">Windows 信息保护 PIN 字符要求</span><span class="sxs-lookup"><span data-stu-id="ceaa2-157">Windows information protection PIN character requirements</span></span>](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [<span data-ttu-id="ceaa2-158">Windows 信息保护策略</span><span class="sxs-lookup"><span data-stu-id="ceaa2-158">Windows information protection policy</span></span>](intune-mam-windowsinformationprotectionpolicy.md)
- [<span data-ttu-id="ceaa2-159">Windows 信息保护代理域集合</span><span class="sxs-lookup"><span data-stu-id="ceaa2-159">Windows information protection proxied domain collection</span></span>](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [<span data-ttu-id="ceaa2-160">Windows 信息保护资源集合</span><span class="sxs-lookup"><span data-stu-id="ceaa2-160">Windows information protection resource collection</span></span>](intune-mam-windowsinformationprotectionresourcecollection.md)
- [<span data-ttu-id="ceaa2-161">Windows 信息保护应用商店应用</span><span class="sxs-lookup"><span data-stu-id="ceaa2-161">Windows information protection store app</span></span>](intune-mam-windowsinformationprotectionstoreapp.md)
- [<span data-ttu-id="ceaa2-162">Windows 信息保护擦除操作</span><span class="sxs-lookup"><span data-stu-id="ceaa2-162">Windows information protection wipe action</span></span>](intune-mam-windowsinformationprotectionwipeaction.md)
