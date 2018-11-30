---
title: 如何通过 Microsoft Intune 保护公司的应用数据
description: Microsoft Intune 应用保护策略可帮助保护公司数据，避免数据丢失。
ms.openlocfilehash: 9dffd9c06baf49274d3c5a0192aa5410f4647c9d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041630"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a><span data-ttu-id="a5c34-103">如何通过 Microsoft Intune 保护公司的应用数据</span><span class="sxs-lookup"><span data-stu-id="a5c34-103">How to protect your company app data with Microsoft Intune</span></span>

> <span data-ttu-id="a5c34-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a5c34-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5c34-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a5c34-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5c34-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a5c34-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="a5c34-107">Microsoft Intune 应用保护策略可帮助保护公司数据，避免数据丢失。</span><span class="sxs-lookup"><span data-stu-id="a5c34-107">Microsoft Intune app protection policies help protect your company data and prevent data loss.</span></span>

<span data-ttu-id="a5c34-108">你可以使用 Intune 应用保护策略帮助保护公司的数据。</span><span class="sxs-lookup"><span data-stu-id="a5c34-108">You can use Intune app protection policies to help protect your company’s data.</span></span> <span data-ttu-id="a5c34-109">因为 Intune 应用程序保护策略可用于独立于任何移动设备管理 (MDM) 解决方案，可用于保护贵公司的数据使用或不注册设备的设备管理解决方案中。</span><span class="sxs-lookup"><span data-stu-id="a5c34-109">Because Intune app protection policies can be used independent of any mobile-device management (MDM) solution, you can use it to protect your company’s data with or without enrolling devices in a device management solution.</span></span> <span data-ttu-id="a5c34-110">通过实现应用级策略，既可以限制对公司资源的访问，也可以将数据保留在 IT 部门的范围之内。</span><span class="sxs-lookup"><span data-stu-id="a5c34-110">By implementing app-level policies, you can restrict access to company resources and keep data within the purview of your IT department.</span></span>

<span data-ttu-id="a5c34-111">以下 Graph 资源可用于在 Intune 中管理应用保护策略：</span><span class="sxs-lookup"><span data-stu-id="a5c34-111">The following Graph resources are available to manage app protection polices in Intune:</span></span>

- [<span data-ttu-id="a5c34-112">Android 管理的应用保护</span><span class="sxs-lookup"><span data-stu-id="a5c34-112">Android managed app protection</span></span>](intune-mam-androidmanagedappprotection.md)
- [<span data-ttu-id="a5c34-113">Android 管理的应用注册</span><span class="sxs-lookup"><span data-stu-id="a5c34-113">Android managed app registration</span></span>](intune-mam-androidmanagedappregistration.md)
- [<span data-ttu-id="a5c34-114">Android 移动应用标识符</span><span class="sxs-lookup"><span data-stu-id="a5c34-114">Android mobile app identifier</span></span>](intune-mam-androidmobileappidentifier.md)
- [<span data-ttu-id="a5c34-115">应用程序管理级别</span><span class="sxs-lookup"><span data-stu-id="a5c34-115">App management level</span></span>](intune-mam-appmanagementlevel.md)
- [<span data-ttu-id="a5c34-116">应用程序类型</span><span class="sxs-lookup"><span data-stu-id="a5c34-116">Application type</span></span>](intune-wip-applicationtype.md)
- [<span data-ttu-id="a5c34-117">默认托管的应用保护</span><span class="sxs-lookup"><span data-stu-id="a5c34-117">Default managed app protection</span></span>](intune-mam-defaultmanagedappprotection.md)
- [<span data-ttu-id="a5c34-118">Intune 品牌配置文件</span><span class="sxs-lookup"><span data-stu-id="a5c34-118">Intune branding profile</span></span>](intune-wip-intunebrandingprofile.md)
- [<span data-ttu-id="a5c34-119">iOS 管理的应用保护</span><span class="sxs-lookup"><span data-stu-id="a5c34-119">iOS managed app protection</span></span>](intune-mam-iosmanagedappprotection.md)
- [<span data-ttu-id="a5c34-120">iOS 管理的应用注册</span><span class="sxs-lookup"><span data-stu-id="a5c34-120">iOS managed app registration</span></span>](intune-mam-iosmanagedappregistration.md)
- [<span data-ttu-id="a5c34-121">iOS 移动应用标识符</span><span class="sxs-lookup"><span data-stu-id="a5c34-121">iOS mobile app identifier</span></span>](intune-mam-iosmobileappidentifier.md)
- [<span data-ttu-id="a5c34-122">JSON</span><span class="sxs-lookup"><span data-stu-id="a5c34-122">JSON</span></span>](intune-mam-json.md)
- [<span data-ttu-id="a5c34-123">托管应用程序剪贴板共享级别</span><span class="sxs-lookup"><span data-stu-id="a5c34-123">Managed app clipboard sharing level</span></span>](intune-mam-managedappclipboardsharinglevel.md)
- [<span data-ttu-id="a5c34-124">托管的应用配置</span><span class="sxs-lookup"><span data-stu-id="a5c34-124">Managed app configuration</span></span>](intune-mam-managedappconfiguration.md)
- [<span data-ttu-id="a5c34-125">托管应用程序数据的加密类型</span><span class="sxs-lookup"><span data-stu-id="a5c34-125">Managed app data encryption type</span></span>](intune-mam-managedappdataencryptiontype.md)
- [<span data-ttu-id="a5c34-126">托管的应用程序数据存储位置</span><span class="sxs-lookup"><span data-stu-id="a5c34-126">Managed app data storage location</span></span>](intune-mam-managedappdatastoragelocation.md)
- [<span data-ttu-id="a5c34-127">托管的应用程序数据传输级别</span><span class="sxs-lookup"><span data-stu-id="a5c34-127">Managed app data transfer level</span></span>](intune-mam-managedappdatatransferlevel.md)
- [<span data-ttu-id="a5c34-128">托管的应用诊断状态</span><span class="sxs-lookup"><span data-stu-id="a5c34-128">Managed app diagnostic status</span></span>](intune-mam-managedappdiagnosticstatus.md)
- [<span data-ttu-id="a5c34-129">托管的应用程序标记原因</span><span class="sxs-lookup"><span data-stu-id="a5c34-129">Managed app flagged reason</span></span>](intune-mam-managedappflaggedreason.md)
- [<span data-ttu-id="a5c34-130">托管的应用操作</span><span class="sxs-lookup"><span data-stu-id="a5c34-130">Managed app operation</span></span>](intune-mam-managedappoperation.md)
- [<span data-ttu-id="a5c34-131">托管的应用程序 PIN 字符集。</span><span class="sxs-lookup"><span data-stu-id="a5c34-131">Managed app PIN character set</span></span>](intune-mam-managedapppincharacterset.md)
- [<span data-ttu-id="a5c34-132">托管的应用策略</span><span class="sxs-lookup"><span data-stu-id="a5c34-132">Managed app policy</span></span>](intune-mam-managedapppolicy.md)
- [<span data-ttu-id="a5c34-133">托管应用策略部署摘要</span><span class="sxs-lookup"><span data-stu-id="a5c34-133">Managed app policy deployment summary</span></span>](intune-mam-managedapppolicydeploymentsummary.md)
- [<span data-ttu-id="a5c34-134">每个应用的托管应用策略部署摘要</span><span class="sxs-lookup"><span data-stu-id="a5c34-134">Managed app policy deployment summary per app</span></span>](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [<span data-ttu-id="a5c34-135">托管的应用保护</span><span class="sxs-lookup"><span data-stu-id="a5c34-135">Managed app protection</span></span>](intune-mam-managedappprotection.md)
- [<span data-ttu-id="a5c34-136">托管应用注册</span><span class="sxs-lookup"><span data-stu-id="a5c34-136">Managed app registration</span></span>](intune-mam-managedappregistration.md)
- [<span data-ttu-id="a5c34-137">托管的应用程序修复操作</span><span class="sxs-lookup"><span data-stu-id="a5c34-137">Managed app remediation action</span></span>](intune-mam-managedappremediationaction.md)
- [<span data-ttu-id="a5c34-138">托管应用状态</span><span class="sxs-lookup"><span data-stu-id="a5c34-138">Managed app status</span></span>](intune-mam-managedappstatus.md)
- [<span data-ttu-id="a5c34-139">托管应用原始状态</span><span class="sxs-lookup"><span data-stu-id="a5c34-139">Managed app status raw</span></span>](intune-mam-managedappstatusraw.md)
- [<span data-ttu-id="a5c34-140">托管移动应用</span><span class="sxs-lookup"><span data-stu-id="a5c34-140">Managed mobile app</span></span>](intune-mam-managedmobileapp.md)
- [<span data-ttu-id="a5c34-141">MDM Windows 信息保护策略</span><span class="sxs-lookup"><span data-stu-id="a5c34-141">MDM windows information protection policy</span></span>](intune-mam-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="a5c34-142">移动应用标识符</span><span class="sxs-lookup"><span data-stu-id="a5c34-142">Mobile app identifier</span></span>](intune-mam-mobileappidentifier.md)
- [<span data-ttu-id="a5c34-143">目标托管应用配置</span><span class="sxs-lookup"><span data-stu-id="a5c34-143">Targeted managed app configuration</span></span>](intune-mam-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="a5c34-144">目标托管应用程序策略分配</span><span class="sxs-lookup"><span data-stu-id="a5c34-144">Targeted managed app policy assignment</span></span>](intune-mam-targetedmanagedapppolicyassignment.md)
- [<span data-ttu-id="a5c34-145">目标托管应用保护</span><span class="sxs-lookup"><span data-stu-id="a5c34-145">Targeted managed app protection</span></span>](intune-mam-targetedmanagedappprotection.md)
- [<span data-ttu-id="a5c34-146">Windows 信息保护</span><span class="sxs-lookup"><span data-stu-id="a5c34-146">Windows information protection</span></span>](intune-mam-windowsinformationprotection.md)
- [<span data-ttu-id="a5c34-147">Windows 信息保护应用</span><span class="sxs-lookup"><span data-stu-id="a5c34-147">Windows information protection app</span></span>](intune-mam-windowsinformationprotectionapp.md)
- [<span data-ttu-id="a5c34-148">Windows 信息保护应用学习摘要</span><span class="sxs-lookup"><span data-stu-id="a5c34-148">Windows information protection app learning summary</span></span>](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [<span data-ttu-id="a5c34-149">Windows 信息保护应用锁定程序文件</span><span class="sxs-lookup"><span data-stu-id="a5c34-149">Windows information protection app locker file</span></span>](intune-mam-windowsinformationprotectionapplockerfile.md)
- [<span data-ttu-id="a5c34-150">Windows 信息保护数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="a5c34-150">Windows information protection data recovery certificate</span></span>](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [<span data-ttu-id="a5c34-151">Windows 信息保护桌面应用</span><span class="sxs-lookup"><span data-stu-id="a5c34-151">Windows information protection desktop app</span></span>](intune-mam-windowsinformationprotectiondesktopapp.md)
- [<span data-ttu-id="a5c34-152">Windows 的信息保护实施级别</span><span class="sxs-lookup"><span data-stu-id="a5c34-152">Windows information protection enforcement level</span></span>](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [<span data-ttu-id="a5c34-153">Windows 信息保护 IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="a5c34-153">Windows information protection IP range collection</span></span>](intune-mam-windowsinformationprotectioniprangecollection.md)
- [<span data-ttu-id="a5c34-154">Windows 信息保护网络学习摘要</span><span class="sxs-lookup"><span data-stu-id="a5c34-154">Windows information protection network learning summary</span></span>](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [<span data-ttu-id="a5c34-155">Windows 信息保护 PIN 字符要求</span><span class="sxs-lookup"><span data-stu-id="a5c34-155">Windows information protection PIN character requirements</span></span>](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [<span data-ttu-id="a5c34-156">Windows 信息保护策略</span><span class="sxs-lookup"><span data-stu-id="a5c34-156">Windows information protection policy</span></span>](intune-mam-windowsinformationprotectionpolicy.md)
- [<span data-ttu-id="a5c34-157">Windows 信息保护代理域集合</span><span class="sxs-lookup"><span data-stu-id="a5c34-157">Windows information protection proxied domain collection</span></span>](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [<span data-ttu-id="a5c34-158">Windows 信息保护资源集合</span><span class="sxs-lookup"><span data-stu-id="a5c34-158">Windows information protection resource collection</span></span>](intune-mam-windowsinformationprotectionresourcecollection.md)
- [<span data-ttu-id="a5c34-159">Windows 信息保护应用商店应用</span><span class="sxs-lookup"><span data-stu-id="a5c34-159">Windows information protection store app</span></span>](intune-mam-windowsinformationprotectionstoreapp.md)
