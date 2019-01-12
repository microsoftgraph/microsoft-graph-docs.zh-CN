---
title: Microsoft Intune 中共享的资源
description: 这些终结点用于多个 Microsoft Graph API 中 Intune 工作流。  用途、 用途以及使用给定的资源所需的权限会有所不同，根据特定工作流和基础调用上下文。  此外，仅对特定的工作流支持某些方法、 属性和操作。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 6180868d4aec195afcc037146f475e56a91aa669
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952557"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="b8533-105">Microsoft Intune 中共享的资源</span><span class="sxs-lookup"><span data-stu-id="b8533-105">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="b8533-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b8533-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8533-107">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b8533-107">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8533-108">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b8533-108">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="b8533-109">这些终结点用于多个 Microsoft Graph API 中 Intune 工作流。</span><span class="sxs-lookup"><span data-stu-id="b8533-109">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="b8533-110">用途、 用途以及使用给定的资源所需的权限会有所不同，根据特定工作流和基础调用上下文。</span><span class="sxs-lookup"><span data-stu-id="b8533-110">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="b8533-111">此外，仅对特定的工作流支持某些方法、 属性和操作。</span><span class="sxs-lookup"><span data-stu-id="b8533-111">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="b8533-112">下面的图资源 Intune 工作流之间共享：</span><span class="sxs-lookup"><span data-stu-id="b8533-112">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="b8533-113">操作状态</span><span class="sxs-lookup"><span data-stu-id="b8533-113">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="b8533-114">所有设备分配目标</span><span class="sxs-lookup"><span data-stu-id="b8533-114">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="b8533-115">所有许可的用户分配目标</span><span class="sxs-lookup"><span data-stu-id="b8533-115">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="b8533-116">合规性状态</span><span class="sxs-lookup"><span data-stu-id="b8533-116">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="b8533-117">设备和应用管理分配目标</span><span class="sxs-lookup"><span data-stu-id="b8533-117">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="b8533-118">设备应用管理</span><span class="sxs-lookup"><span data-stu-id="b8533-118">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="b8533-119">设备类别</span><span class="sxs-lookup"><span data-stu-id="b8533-119">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="b8533-120">设备注册类型</span><span class="sxs-lookup"><span data-stu-id="b8533-120">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="b8533-121">设备管理</span><span class="sxs-lookup"><span data-stu-id="b8533-121">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="b8533-122">设备平台类型</span><span class="sxs-lookup"><span data-stu-id="b8533-122">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="b8533-123">设备类型</span><span class="sxs-lookup"><span data-stu-id="b8533-123">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="b8533-124">启用</span><span class="sxs-lookup"><span data-stu-id="b8533-124">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="b8533-125">排除组分配目标</span><span class="sxs-lookup"><span data-stu-id="b8533-125">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="b8533-126">组分配目标</span><span class="sxs-lookup"><span data-stu-id="b8533-126">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="b8533-127">安装用途</span><span class="sxs-lookup"><span data-stu-id="b8533-127">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="b8533-128">IP 范围</span><span class="sxs-lookup"><span data-stu-id="b8533-128">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="b8533-129">IPv4 范围</span><span class="sxs-lookup"><span data-stu-id="b8533-129">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="b8533-130">IPv6 范围</span><span class="sxs-lookup"><span data-stu-id="b8533-130">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="b8533-131">键/值对</span><span class="sxs-lookup"><span data-stu-id="b8533-131">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="b8533-132">MIME 内容</span><span class="sxs-lookup"><span data-stu-id="b8533-132">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="b8533-133">代理域</span><span class="sxs-lookup"><span data-stu-id="b8533-133">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="b8533-134">Report</span><span class="sxs-lookup"><span data-stu-id="b8533-134">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="b8533-135">报表根目录</span><span class="sxs-lookup"><span data-stu-id="b8533-135">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="b8533-136">结果的应用程序状态</span><span class="sxs-lookup"><span data-stu-id="b8533-136">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="b8533-137">RGB 颜色</span><span class="sxs-lookup"><span data-stu-id="b8533-137">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="b8533-138">运行方式帐户类型</span><span class="sxs-lookup"><span data-stu-id="b8533-138">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="b8533-139">运行状态</span><span class="sxs-lookup"><span data-stu-id="b8533-139">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="b8533-140">保存 UI 状态生成选项</span><span class="sxs-lookup"><span data-stu-id="b8533-140">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="b8533-141">URI</span><span class="sxs-lookup"><span data-stu-id="b8533-141">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="b8533-142">用户</span><span class="sxs-lookup"><span data-stu-id="b8533-142">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="b8533-143">VPP 令牌帐户类型</span><span class="sxs-lookup"><span data-stu-id="b8533-143">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="b8533-144">VPP 令牌操作失败的原因</span><span class="sxs-lookup"><span data-stu-id="b8533-144">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="b8533-145">Windows 域与会配置</span><span class="sxs-lookup"><span data-stu-id="b8533-145">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
