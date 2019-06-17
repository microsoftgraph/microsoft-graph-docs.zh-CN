---
title: Microsoft Intune 中的共享资源-Microsoft Graph API
description: 列出支持租户组织的多个工作流的 Intune 终结点 (REST) 的 Microsoft Graph API。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: 2240f8ff55ca2dbcf4e7107495e07b72f95cdfa4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996188"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="0d18a-103">Microsoft Intune 中的共享资源</span><span class="sxs-lookup"><span data-stu-id="0d18a-103">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="0d18a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0d18a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d18a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0d18a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d18a-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0d18a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d18a-107">这些终结点在多个 Microsoft Graph API for Intune 工作流中使用。</span><span class="sxs-lookup"><span data-stu-id="0d18a-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="0d18a-108">使用给定资源所需的意向、目的和权限因特定工作流和基础调用的上下文而异。</span><span class="sxs-lookup"><span data-stu-id="0d18a-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="0d18a-109">此外, 特定工作流仅支持某些方法、属性和操作。</span><span class="sxs-lookup"><span data-stu-id="0d18a-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="0d18a-110">以下关系图资源在 Intune 工作流之间共享:</span><span class="sxs-lookup"><span data-stu-id="0d18a-110">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="0d18a-111">操作状态</span><span class="sxs-lookup"><span data-stu-id="0d18a-111">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="0d18a-112">所有设备分配目标</span><span class="sxs-lookup"><span data-stu-id="0d18a-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="0d18a-113">所有许可的用户分配目标</span><span class="sxs-lookup"><span data-stu-id="0d18a-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="0d18a-114">符合性状态</span><span class="sxs-lookup"><span data-stu-id="0d18a-114">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="0d18a-115">设备和应用管理分配目标</span><span class="sxs-lookup"><span data-stu-id="0d18a-115">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="0d18a-116">设备应用管理</span><span class="sxs-lookup"><span data-stu-id="0d18a-116">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="0d18a-117">设备类别</span><span class="sxs-lookup"><span data-stu-id="0d18a-117">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="0d18a-118">设备注册类型</span><span class="sxs-lookup"><span data-stu-id="0d18a-118">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="0d18a-119">设备管理</span><span class="sxs-lookup"><span data-stu-id="0d18a-119">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="0d18a-120">设备平台类型</span><span class="sxs-lookup"><span data-stu-id="0d18a-120">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="0d18a-121">设备类型</span><span class="sxs-lookup"><span data-stu-id="0d18a-121">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="0d18a-122">支持</span><span class="sxs-lookup"><span data-stu-id="0d18a-122">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="0d18a-123">排除组分配目标</span><span class="sxs-lookup"><span data-stu-id="0d18a-123">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="0d18a-124">组分配目标</span><span class="sxs-lookup"><span data-stu-id="0d18a-124">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="0d18a-125">安装意图</span><span class="sxs-lookup"><span data-stu-id="0d18a-125">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="0d18a-126">IP 范围</span><span class="sxs-lookup"><span data-stu-id="0d18a-126">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="0d18a-127">IPv4 范围</span><span class="sxs-lookup"><span data-stu-id="0d18a-127">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="0d18a-128">IPv6 范围</span><span class="sxs-lookup"><span data-stu-id="0d18a-128">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="0d18a-129">键/值对</span><span class="sxs-lookup"><span data-stu-id="0d18a-129">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="0d18a-130">MIME 内容</span><span class="sxs-lookup"><span data-stu-id="0d18a-130">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="0d18a-131">移动应用疑难解答事件</span><span class="sxs-lookup"><span data-stu-id="0d18a-131">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="0d18a-132">代理域</span><span class="sxs-lookup"><span data-stu-id="0d18a-132">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="0d18a-133">Report</span><span class="sxs-lookup"><span data-stu-id="0d18a-133">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="0d18a-134">报表根目录</span><span class="sxs-lookup"><span data-stu-id="0d18a-134">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="0d18a-135">生成的应用状态</span><span class="sxs-lookup"><span data-stu-id="0d18a-135">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="0d18a-136">RGB 颜色</span><span class="sxs-lookup"><span data-stu-id="0d18a-136">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="0d18a-137">按帐户类型运行</span><span class="sxs-lookup"><span data-stu-id="0d18a-137">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="0d18a-138">运行状态</span><span class="sxs-lookup"><span data-stu-id="0d18a-138">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="0d18a-139">保存的 UI 状态生成选项</span><span class="sxs-lookup"><span data-stu-id="0d18a-139">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="0d18a-140">URI</span><span class="sxs-lookup"><span data-stu-id="0d18a-140">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="0d18a-141">用户</span><span class="sxs-lookup"><span data-stu-id="0d18a-141">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="0d18a-142">VPP 令牌帐户类型</span><span class="sxs-lookup"><span data-stu-id="0d18a-142">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="0d18a-143">VPP 令牌操作失败原因</span><span class="sxs-lookup"><span data-stu-id="0d18a-143">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="0d18a-144">Windows 域加入配置</span><span class="sxs-lookup"><span data-stu-id="0d18a-144">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
