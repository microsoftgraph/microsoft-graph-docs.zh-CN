---
title: Microsoft Intune 中共享的资源
description: 这些终结点用于多个 Microsoft Graph API 中 Intune 工作流。  用途、 用途以及使用给定的资源所需的权限会有所不同，根据特定工作流和基础调用上下文。  此外，仅对特定的工作流支持某些方法、 属性和操作。
localization_priority: Normal
ms.openlocfilehash: c381ba84c9240a2b8e7428a3c055b8baf35fb243
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852624"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="c291f-105">Microsoft Intune 中共享的资源</span><span class="sxs-lookup"><span data-stu-id="c291f-105">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="c291f-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c291f-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c291f-107">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c291f-107">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c291f-108">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c291f-108">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="c291f-109">这些终结点用于多个 Microsoft Graph API 中 Intune 工作流。</span><span class="sxs-lookup"><span data-stu-id="c291f-109">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="c291f-110">用途、 用途以及使用给定的资源所需的权限会有所不同，根据特定工作流和基础调用上下文。</span><span class="sxs-lookup"><span data-stu-id="c291f-110">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="c291f-111">此外，仅对特定的工作流支持某些方法、 属性和操作。</span><span class="sxs-lookup"><span data-stu-id="c291f-111">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="c291f-112">下面的图资源 Intune 工作流之间共享：</span><span class="sxs-lookup"><span data-stu-id="c291f-112">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="c291f-113">操作状态</span><span class="sxs-lookup"><span data-stu-id="c291f-113">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="c291f-114">所有设备分配目标</span><span class="sxs-lookup"><span data-stu-id="c291f-114">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="c291f-115">所有许可的用户分配目标</span><span class="sxs-lookup"><span data-stu-id="c291f-115">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="c291f-116">合规性状态</span><span class="sxs-lookup"><span data-stu-id="c291f-116">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="c291f-117">设备和应用管理分配目标</span><span class="sxs-lookup"><span data-stu-id="c291f-117">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="c291f-118">设备应用管理</span><span class="sxs-lookup"><span data-stu-id="c291f-118">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="c291f-119">设备类别</span><span class="sxs-lookup"><span data-stu-id="c291f-119">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="c291f-120">设备注册类型</span><span class="sxs-lookup"><span data-stu-id="c291f-120">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="c291f-121">设备管理</span><span class="sxs-lookup"><span data-stu-id="c291f-121">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="c291f-122">设备平台类型</span><span class="sxs-lookup"><span data-stu-id="c291f-122">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="c291f-123">设备类型</span><span class="sxs-lookup"><span data-stu-id="c291f-123">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="c291f-124">启用</span><span class="sxs-lookup"><span data-stu-id="c291f-124">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="c291f-125">排除组分配目标</span><span class="sxs-lookup"><span data-stu-id="c291f-125">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="c291f-126">组分配目标</span><span class="sxs-lookup"><span data-stu-id="c291f-126">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="c291f-127">安装用途</span><span class="sxs-lookup"><span data-stu-id="c291f-127">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="c291f-128">IP 范围</span><span class="sxs-lookup"><span data-stu-id="c291f-128">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="c291f-129">IPv4 范围</span><span class="sxs-lookup"><span data-stu-id="c291f-129">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="c291f-130">IPv6 范围</span><span class="sxs-lookup"><span data-stu-id="c291f-130">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="c291f-131">键/值对</span><span class="sxs-lookup"><span data-stu-id="c291f-131">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="c291f-132">MIME 内容</span><span class="sxs-lookup"><span data-stu-id="c291f-132">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="c291f-133">代理域</span><span class="sxs-lookup"><span data-stu-id="c291f-133">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="c291f-134">Report</span><span class="sxs-lookup"><span data-stu-id="c291f-134">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="c291f-135">报表根目录</span><span class="sxs-lookup"><span data-stu-id="c291f-135">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="c291f-136">结果的应用程序状态</span><span class="sxs-lookup"><span data-stu-id="c291f-136">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="c291f-137">RGB 颜色</span><span class="sxs-lookup"><span data-stu-id="c291f-137">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="c291f-138">运行方式帐户类型</span><span class="sxs-lookup"><span data-stu-id="c291f-138">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="c291f-139">运行状态</span><span class="sxs-lookup"><span data-stu-id="c291f-139">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="c291f-140">保存 UI 状态生成选项</span><span class="sxs-lookup"><span data-stu-id="c291f-140">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="c291f-141">URI</span><span class="sxs-lookup"><span data-stu-id="c291f-141">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="c291f-142">用户</span><span class="sxs-lookup"><span data-stu-id="c291f-142">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="c291f-143">VPP 令牌帐户类型</span><span class="sxs-lookup"><span data-stu-id="c291f-143">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="c291f-144">VPP 令牌操作失败的原因</span><span class="sxs-lookup"><span data-stu-id="c291f-144">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="c291f-145">Windows 域与会配置</span><span class="sxs-lookup"><span data-stu-id="c291f-145">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
