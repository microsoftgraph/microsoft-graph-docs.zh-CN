---
title: Microsoft Intune 中共享的资源
description: 这些终结点用于多个 Microsoft Graph API 中 Intune 工作流。  用途、 用途以及使用给定的资源所需的权限会有所不同，根据特定工作流和基础调用上下文。  此外，仅对特定的工作流支持某些方法、 属性和操作。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: cfb3acbb3b736fcb96d22773301ca6e2e3e4403f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966774"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="84c65-105">Microsoft Intune 中共享的资源</span><span class="sxs-lookup"><span data-stu-id="84c65-105">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="84c65-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="84c65-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="84c65-107">这些终结点用于多个 Microsoft Graph API 中 Intune 工作流。</span><span class="sxs-lookup"><span data-stu-id="84c65-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="84c65-108">用途、 用途以及使用给定的资源所需的权限会有所不同，根据特定工作流和基础调用上下文。</span><span class="sxs-lookup"><span data-stu-id="84c65-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="84c65-109">此外，仅对特定的工作流支持某些方法、 属性和操作。</span><span class="sxs-lookup"><span data-stu-id="84c65-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="84c65-110">下面的图资源 Intune 工作流之间共享：</span><span class="sxs-lookup"><span data-stu-id="84c65-110">The following Graph resources are shared between Intune workflows:</span></span>  

- [<span data-ttu-id="84c65-111">所有设备分配目标</span><span class="sxs-lookup"><span data-stu-id="84c65-111">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="84c65-112">所有许可的用户分配目标</span><span class="sxs-lookup"><span data-stu-id="84c65-112">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="84c65-113">合规性状态</span><span class="sxs-lookup"><span data-stu-id="84c65-113">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="84c65-114">设备和应用管理分配目标</span><span class="sxs-lookup"><span data-stu-id="84c65-114">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="84c65-115">设备应用管理</span><span class="sxs-lookup"><span data-stu-id="84c65-115">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="84c65-116">设备类别</span><span class="sxs-lookup"><span data-stu-id="84c65-116">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="84c65-117">设备管理</span><span class="sxs-lookup"><span data-stu-id="84c65-117">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="84c65-118">排除组分配目标</span><span class="sxs-lookup"><span data-stu-id="84c65-118">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="84c65-119">组分配目标</span><span class="sxs-lookup"><span data-stu-id="84c65-119">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="84c65-120">安装用途</span><span class="sxs-lookup"><span data-stu-id="84c65-120">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="84c65-121">MIME 内容</span><span class="sxs-lookup"><span data-stu-id="84c65-121">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="84c65-122">Report</span><span class="sxs-lookup"><span data-stu-id="84c65-122">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="84c65-123">报表根目录</span><span class="sxs-lookup"><span data-stu-id="84c65-123">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="84c65-124">保存 UI 状态生成选项</span><span class="sxs-lookup"><span data-stu-id="84c65-124">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="84c65-125">URI</span><span class="sxs-lookup"><span data-stu-id="84c65-125">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="84c65-126">用户</span><span class="sxs-lookup"><span data-stu-id="84c65-126">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="84c65-127">VPP 令牌帐户类型</span><span class="sxs-lookup"><span data-stu-id="84c65-127">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
