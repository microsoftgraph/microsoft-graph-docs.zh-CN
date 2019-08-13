---
title: Microsoft Intune 中的共享资源-Microsoft Graph API
description: 列出支持租户组织的多个工作流的 Intune 终结点 (REST) 的 Microsoft Graph API。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: 0d2252093f222f5908756f312c2e82d591c29920
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372802"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="542b3-103">Microsoft Intune 中的共享资源</span><span class="sxs-lookup"><span data-stu-id="542b3-103">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="542b3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="542b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="542b3-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="542b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="542b3-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="542b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="542b3-107">这些终结点在多个 Microsoft Graph API for Intune 工作流中使用。</span><span class="sxs-lookup"><span data-stu-id="542b3-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="542b3-108">使用给定资源所需的意向、目的和权限因特定工作流和基础调用的上下文而异。</span><span class="sxs-lookup"><span data-stu-id="542b3-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="542b3-109">此外, 特定工作流仅支持某些方法、属性和操作。</span><span class="sxs-lookup"><span data-stu-id="542b3-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="542b3-110">以下关系图资源在 Intune 工作流之间共享:</span><span class="sxs-lookup"><span data-stu-id="542b3-110">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="542b3-111">操作状态</span><span class="sxs-lookup"><span data-stu-id="542b3-111">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="542b3-112">所有设备分配目标</span><span class="sxs-lookup"><span data-stu-id="542b3-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="542b3-113">所有许可的用户分配目标</span><span class="sxs-lookup"><span data-stu-id="542b3-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="542b3-114">符合性状态</span><span class="sxs-lookup"><span data-stu-id="542b3-114">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="542b3-115">设备和应用管理分配目标</span><span class="sxs-lookup"><span data-stu-id="542b3-115">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="542b3-116">设备应用管理</span><span class="sxs-lookup"><span data-stu-id="542b3-116">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="542b3-117">设备类别</span><span class="sxs-lookup"><span data-stu-id="542b3-117">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="542b3-118">设备注册类型</span><span class="sxs-lookup"><span data-stu-id="542b3-118">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="542b3-119">设备管理</span><span class="sxs-lookup"><span data-stu-id="542b3-119">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="542b3-120">设备平台类型</span><span class="sxs-lookup"><span data-stu-id="542b3-120">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="542b3-121">设备类型</span><span class="sxs-lookup"><span data-stu-id="542b3-121">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="542b3-122">支持</span><span class="sxs-lookup"><span data-stu-id="542b3-122">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="542b3-123">支持</span><span class="sxs-lookup"><span data-stu-id="542b3-123">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="542b3-124">排除组分配目标</span><span class="sxs-lookup"><span data-stu-id="542b3-124">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="542b3-125">组分配目标</span><span class="sxs-lookup"><span data-stu-id="542b3-125">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="542b3-126">安装意图</span><span class="sxs-lookup"><span data-stu-id="542b3-126">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="542b3-127">IP 范围</span><span class="sxs-lookup"><span data-stu-id="542b3-127">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="542b3-128">IPv4 范围</span><span class="sxs-lookup"><span data-stu-id="542b3-128">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="542b3-129">IPv6 范围</span><span class="sxs-lookup"><span data-stu-id="542b3-129">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="542b3-130">键/值对</span><span class="sxs-lookup"><span data-stu-id="542b3-130">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="542b3-131">MIME 内容</span><span class="sxs-lookup"><span data-stu-id="542b3-131">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="542b3-132">移动应用疑难解答事件</span><span class="sxs-lookup"><span data-stu-id="542b3-132">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="542b3-133">代理域</span><span class="sxs-lookup"><span data-stu-id="542b3-133">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="542b3-134">Report</span><span class="sxs-lookup"><span data-stu-id="542b3-134">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="542b3-135">报表根目录</span><span class="sxs-lookup"><span data-stu-id="542b3-135">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="542b3-136">生成的应用状态</span><span class="sxs-lookup"><span data-stu-id="542b3-136">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="542b3-137">RGB 颜色</span><span class="sxs-lookup"><span data-stu-id="542b3-137">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="542b3-138">运行状态</span><span class="sxs-lookup"><span data-stu-id="542b3-138">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="542b3-139">保存的 UI 状态生成选项</span><span class="sxs-lookup"><span data-stu-id="542b3-139">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="542b3-140">URI</span><span class="sxs-lookup"><span data-stu-id="542b3-140">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="542b3-141">用户</span><span class="sxs-lookup"><span data-stu-id="542b3-141">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="542b3-142">VPP 令牌帐户类型</span><span class="sxs-lookup"><span data-stu-id="542b3-142">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="542b3-143">VPP 令牌操作失败原因</span><span class="sxs-lookup"><span data-stu-id="542b3-143">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="542b3-144">Windows 域加入配置</span><span class="sxs-lookup"><span data-stu-id="542b3-144">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
