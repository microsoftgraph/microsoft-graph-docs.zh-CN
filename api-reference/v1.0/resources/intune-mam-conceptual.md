---
title: 如何通过 Microsoft Intune 保护公司的应用数据
description: Microsoft Intune 应用保护策略可帮助保护公司数据，避免数据丢失。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 85c002b9b9a8271b47209ca11bb27eb2885815a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465550"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a><span data-ttu-id="79a07-103">如何通过 Microsoft Intune 保护公司的应用数据</span><span class="sxs-lookup"><span data-stu-id="79a07-103">How to protect your company app data with Microsoft Intune</span></span>

> <span data-ttu-id="79a07-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="79a07-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="79a07-105">Microsoft Intune 应用保护策略可帮助保护公司数据，避免数据丢失。</span><span class="sxs-lookup"><span data-stu-id="79a07-105">Microsoft Intune app protection policies help protect your company data and prevent data loss.</span></span>

<span data-ttu-id="79a07-106">你可以使用 Intune 应用保护策略帮助保护公司的数据。</span><span class="sxs-lookup"><span data-stu-id="79a07-106">You can use Intune app protection policies to help protect your company’s data.</span></span> <span data-ttu-id="79a07-107">由于 Intune 应用保护策略可以独立于移动设备管理 (MDM) 解决方案使用，无论是否在设备管理解决方案中注册设备，你都可以保护公司的数据。</span><span class="sxs-lookup"><span data-stu-id="79a07-107">Because Intune app protection policies can be used independent of any mobile-device management (MDM) solution, you protect your company’s data with or without enrolling devices in a device management solution.</span></span> <span data-ttu-id="79a07-108">通过实现应用级策略，既可以限制对公司资源的访问，也可以将数据保留在 IT 部门的范围之内。</span><span class="sxs-lookup"><span data-stu-id="79a07-108">By implementing app-level policies, you can restrict access to company resources and keep data within the purview of your IT department.</span></span>

<span data-ttu-id="79a07-109">以下 Graph 资源可用于在 Intune 中管理应用保护策略：</span><span class="sxs-lookup"><span data-stu-id="79a07-109">The following Graph resources are available to manage app protection polices in Intune:</span></span>  

- [<span data-ttu-id="79a07-110">Android 管理的应用保护</span><span class="sxs-lookup"><span data-stu-id="79a07-110">Android managed app protection</span></span>](intune-mam-androidmanagedappprotection.md)
- [<span data-ttu-id="79a07-111">Android 管理的应用注册</span><span class="sxs-lookup"><span data-stu-id="79a07-111">Android managed app registration</span></span>](intune-mam-androidmanagedappregistration.md)
- [<span data-ttu-id="79a07-112">Android 移动应用标识符</span><span class="sxs-lookup"><span data-stu-id="79a07-112">Android mobile app identifier</span></span>](intune-mam-androidmobileappidentifier.md)
- [<span data-ttu-id="79a07-113">应用程序类型</span><span class="sxs-lookup"><span data-stu-id="79a07-113">Application type</span></span>](intune-wip-applicationtype.md)
- [<span data-ttu-id="79a07-114">默认托管的应用保护</span><span class="sxs-lookup"><span data-stu-id="79a07-114">Default managed app protection</span></span>](intune-mam-defaultmanagedappprotection.md)
- [<span data-ttu-id="79a07-115">iOS 管理的应用保护</span><span class="sxs-lookup"><span data-stu-id="79a07-115">iOS managed app protection</span></span>](intune-mam-iosmanagedappprotection.md)
- [<span data-ttu-id="79a07-116">iOS 管理的应用注册</span><span class="sxs-lookup"><span data-stu-id="79a07-116">iOS managed app registration</span></span>](intune-mam-iosmanagedappregistration.md)
- [<span data-ttu-id="79a07-117">iOS 移动应用标识符</span><span class="sxs-lookup"><span data-stu-id="79a07-117">iOS mobile app identifier</span></span>](intune-mam-iosmobileappidentifier.md)
- [<span data-ttu-id="79a07-118">IP 范围</span><span class="sxs-lookup"><span data-stu-id="79a07-118">IP range</span></span>](intune-mam-iprange.md)
- [<span data-ttu-id="79a07-119">IPv4 范围</span><span class="sxs-lookup"><span data-stu-id="79a07-119">IPv4 range</span></span>](intune-mam-ipv4range.md)
- [<span data-ttu-id="79a07-120">IPv6 范围</span><span class="sxs-lookup"><span data-stu-id="79a07-120">IPv6 range</span></span>](intune-mam-ipv6range.md)
- [<span data-ttu-id="79a07-121">JSON</span><span class="sxs-lookup"><span data-stu-id="79a07-121">JSON</span></span>](intune-mam-json.md)
- [<span data-ttu-id="79a07-122">键/值对</span><span class="sxs-lookup"><span data-stu-id="79a07-122">Key/value pair</span></span>](intune-mam-keyvaluepair.md)
- [<span data-ttu-id="79a07-123">受管理的应用剪贴板共享级别</span><span class="sxs-lookup"><span data-stu-id="79a07-123">Managed app clipboard sharing level</span></span>](intune-mam-managedappclipboardsharinglevel.md)
- [<span data-ttu-id="79a07-124">托管的应用配置</span><span class="sxs-lookup"><span data-stu-id="79a07-124">Managed app configuration</span></span>](intune-mam-managedappconfiguration.md)
- [<span data-ttu-id="79a07-125">受管理应用的数据加密类型</span><span class="sxs-lookup"><span data-stu-id="79a07-125">Managed app data encryption type</span></span>](intune-mam-managedappdataencryptiontype.md)
- [<span data-ttu-id="79a07-126">受管理应用的数据存储位置</span><span class="sxs-lookup"><span data-stu-id="79a07-126">Managed app data storage location</span></span>](intune-mam-managedappdatastoragelocation.md)
- [<span data-ttu-id="79a07-127">受管理应用的数据传输级别</span><span class="sxs-lookup"><span data-stu-id="79a07-127">Managed app data transfer level</span></span>](intune-mam-managedappdatatransferlevel.md)
- [<span data-ttu-id="79a07-128">托管的应用诊断状态</span><span class="sxs-lookup"><span data-stu-id="79a07-128">Managed app diagnostic status</span></span>](intune-mam-managedappdiagnosticstatus.md)
- [<span data-ttu-id="79a07-129">受管理应用的已标记原因</span><span class="sxs-lookup"><span data-stu-id="79a07-129">Managed app flagged reason</span></span>](intune-mam-managedappflaggedreason.md)
- [<span data-ttu-id="79a07-130">托管的应用操作</span><span class="sxs-lookup"><span data-stu-id="79a07-130">Managed app operation</span></span>](intune-mam-managedappoperation.md)
- [<span data-ttu-id="79a07-131">托管的应用 PIN 字符集</span><span class="sxs-lookup"><span data-stu-id="79a07-131">Managed app PIN character set</span></span>](intune-mam-managedapppincharacterset.md)
- [<span data-ttu-id="79a07-132">托管的应用策略</span><span class="sxs-lookup"><span data-stu-id="79a07-132">Managed app policy</span></span>](intune-mam-managedapppolicy.md)
- [<span data-ttu-id="79a07-133">托管应用策略部署摘要</span><span class="sxs-lookup"><span data-stu-id="79a07-133">Managed app policy deployment summary</span></span>](intune-mam-managedapppolicydeploymentsummary.md)
- [<span data-ttu-id="79a07-134">每个应用的托管应用策略部署摘要</span><span class="sxs-lookup"><span data-stu-id="79a07-134">Managed app policy deployment summary per app</span></span>](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [<span data-ttu-id="79a07-135">托管的应用保护</span><span class="sxs-lookup"><span data-stu-id="79a07-135">Managed app protection</span></span>](intune-mam-managedappprotection.md)
- [<span data-ttu-id="79a07-136">托管应用注册</span><span class="sxs-lookup"><span data-stu-id="79a07-136">Managed app registration</span></span>](intune-mam-managedappregistration.md)
- [<span data-ttu-id="79a07-137">托管应用状态</span><span class="sxs-lookup"><span data-stu-id="79a07-137">Managed app status</span></span>](intune-mam-managedappstatus.md)
- [<span data-ttu-id="79a07-138">托管应用原始状态</span><span class="sxs-lookup"><span data-stu-id="79a07-138">Managed app status raw</span></span>](intune-mam-managedappstatusraw.md)
- [<span data-ttu-id="79a07-139">托管移动应用</span><span class="sxs-lookup"><span data-stu-id="79a07-139">Managed mobile app</span></span>](intune-mam-managedmobileapp.md)
- [<span data-ttu-id="79a07-140">MDM Windows 信息保护策略</span><span class="sxs-lookup"><span data-stu-id="79a07-140">MDM windows information protection policy</span></span>](intune-mam-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="79a07-141">移动应用标识符</span><span class="sxs-lookup"><span data-stu-id="79a07-141">Mobile app identifier</span></span>](intune-mam-mobileappidentifier.md)
- [<span data-ttu-id="79a07-142">代理域</span><span class="sxs-lookup"><span data-stu-id="79a07-142">Proxied domain</span></span>](intune-mam-proxieddomain.md)
- [<span data-ttu-id="79a07-143">目标托管应用配置</span><span class="sxs-lookup"><span data-stu-id="79a07-143">Targeted managed app configuration</span></span>](intune-mam-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="79a07-144">目标托管应用程序策略分配</span><span class="sxs-lookup"><span data-stu-id="79a07-144">Targeted managed app policy assignment</span></span>](intune-mam-targetedmanagedapppolicyassignment.md)
- [<span data-ttu-id="79a07-145">目标托管应用保护</span><span class="sxs-lookup"><span data-stu-id="79a07-145">Targeted managed app protection</span></span>](intune-mam-targetedmanagedappprotection.md)
- [<span data-ttu-id="79a07-146">Windows 信息保护</span><span class="sxs-lookup"><span data-stu-id="79a07-146">Windows information protection</span></span>](intune-mam-windowsinformationprotection.md)
- [<span data-ttu-id="79a07-147">Windows 信息保护应用</span><span class="sxs-lookup"><span data-stu-id="79a07-147">Windows information protection app</span></span>](intune-mam-windowsinformationprotectionapp.md)
- [<span data-ttu-id="79a07-148">Windows 信息保护应用学习摘要</span><span class="sxs-lookup"><span data-stu-id="79a07-148">Windows information protection app learning summary</span></span>](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [<span data-ttu-id="79a07-149">Windows 信息保护应用锁定程序文件</span><span class="sxs-lookup"><span data-stu-id="79a07-149">Windows information protection app locker file</span></span>](intune-mam-windowsinformationprotectionapplockerfile.md)
- [<span data-ttu-id="79a07-150">Windows 信息保护数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="79a07-150">Windows information protection data recovery certificate</span></span>](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [<span data-ttu-id="79a07-151">Windows 信息保护桌面应用</span><span class="sxs-lookup"><span data-stu-id="79a07-151">Windows information protection desktop app</span></span>](intune-mam-windowsinformationprotectiondesktopapp.md)
- [<span data-ttu-id="79a07-152">Windows 信息保护强制级别</span><span class="sxs-lookup"><span data-stu-id="79a07-152">Windows information protection enforcement level</span></span>](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [<span data-ttu-id="79a07-153">Windows 信息保护 IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="79a07-153">Windows information protection IP range collection</span></span>](intune-mam-windowsinformationprotectioniprangecollection.md)
- [<span data-ttu-id="79a07-154">Windows 信息保护网络学习摘要</span><span class="sxs-lookup"><span data-stu-id="79a07-154">Windows information protection network learning summary</span></span>](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [<span data-ttu-id="79a07-155">Windows 信息保护 PIN 字符要求</span><span class="sxs-lookup"><span data-stu-id="79a07-155">Windows information protection PIN character requirements</span></span>](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [<span data-ttu-id="79a07-156">Windows 信息保护策略</span><span class="sxs-lookup"><span data-stu-id="79a07-156">Windows information protection policy</span></span>](intune-mam-windowsinformationprotectionpolicy.md)
- [<span data-ttu-id="79a07-157">Windows 信息保护代理域集合</span><span class="sxs-lookup"><span data-stu-id="79a07-157">Windows information protection proxied domain collection</span></span>](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [<span data-ttu-id="79a07-158">Windows 信息保护资源集合</span><span class="sxs-lookup"><span data-stu-id="79a07-158">Windows information protection resource collection</span></span>](intune-mam-windowsinformationprotectionresourcecollection.md)
- [<span data-ttu-id="79a07-159">Windows 信息保护应用商店应用</span><span class="sxs-lookup"><span data-stu-id="79a07-159">Windows information protection store app</span></span>](intune-mam-windowsinformationprotectionstoreapp.md)
