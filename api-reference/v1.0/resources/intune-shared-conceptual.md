---
title: Microsoft Intune 中的共享资源
description: 这些终结点在多个 Microsoft Graph API for Intune 工作流中使用。  使用给定资源所需的意向、目的和权限因特定工作流和基础调用的上下文而异。  此外，特定工作流仅支持某些方法、属性和操作。
localization_priority: Normal
author: davidmu1
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 8bd4eedcb9af1391ffeaa3aaf2c815a20981fc5c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447883"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="33934-105">Microsoft Intune 中的共享资源</span><span class="sxs-lookup"><span data-stu-id="33934-105">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="33934-106">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="33934-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33934-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="33934-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="33934-108">这些终结点在多个 Microsoft Graph API for Intune 工作流中使用。</span><span class="sxs-lookup"><span data-stu-id="33934-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="33934-109">使用给定资源所需的意向、目的和权限因特定工作流和基础调用的上下文而异。</span><span class="sxs-lookup"><span data-stu-id="33934-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="33934-110">此外，特定工作流仅支持某些方法、属性和操作。</span><span class="sxs-lookup"><span data-stu-id="33934-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="33934-111">以下关系图资源在 Intune 工作流之间共享：</span><span class="sxs-lookup"><span data-stu-id="33934-111">The following Graph resources are shared between Intune workflows:</span></span>  

- [<span data-ttu-id="33934-112">所有设备分配目标</span><span class="sxs-lookup"><span data-stu-id="33934-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="33934-113">所有许可的用户分配目标</span><span class="sxs-lookup"><span data-stu-id="33934-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="33934-114">符合性状态</span><span class="sxs-lookup"><span data-stu-id="33934-114">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="33934-115">设备和应用管理分配目标</span><span class="sxs-lookup"><span data-stu-id="33934-115">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="33934-116">设备应用管理</span><span class="sxs-lookup"><span data-stu-id="33934-116">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="33934-117">设备类别</span><span class="sxs-lookup"><span data-stu-id="33934-117">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="33934-118">设备管理</span><span class="sxs-lookup"><span data-stu-id="33934-118">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="33934-119">排除组分配目标</span><span class="sxs-lookup"><span data-stu-id="33934-119">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="33934-120">组分配目标</span><span class="sxs-lookup"><span data-stu-id="33934-120">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="33934-121">安装意图</span><span class="sxs-lookup"><span data-stu-id="33934-121">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="33934-122">MIME 内容</span><span class="sxs-lookup"><span data-stu-id="33934-122">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="33934-123">Report</span><span class="sxs-lookup"><span data-stu-id="33934-123">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="33934-124">报表根目录</span><span class="sxs-lookup"><span data-stu-id="33934-124">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="33934-125">保存的 UI 状态生成选项</span><span class="sxs-lookup"><span data-stu-id="33934-125">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="33934-126">URI</span><span class="sxs-lookup"><span data-stu-id="33934-126">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="33934-127">用户</span><span class="sxs-lookup"><span data-stu-id="33934-127">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="33934-128">VPP 令牌帐户类型</span><span class="sxs-lookup"><span data-stu-id="33934-128">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)

