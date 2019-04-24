---
title: Microsoft Intune 中的共享资源
description: 这些终结点在多个 Microsoft Graph API for Intune 工作流中使用。  使用给定资源所需的意向、目的和权限因特定工作流和基础调用的上下文而异。  此外, 特定工作流仅支持某些方法、属性和操作。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: cfb3acbb3b736fcb96d22773301ca6e2e3e4403f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32452181"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="99b3b-105">Microsoft Intune 中的共享资源</span><span class="sxs-lookup"><span data-stu-id="99b3b-105">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="99b3b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="99b3b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="99b3b-107">这些终结点在多个 Microsoft Graph API for Intune 工作流中使用。</span><span class="sxs-lookup"><span data-stu-id="99b3b-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="99b3b-108">使用给定资源所需的意向、目的和权限因特定工作流和基础调用的上下文而异。</span><span class="sxs-lookup"><span data-stu-id="99b3b-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="99b3b-109">此外, 特定工作流仅支持某些方法、属性和操作。</span><span class="sxs-lookup"><span data-stu-id="99b3b-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="99b3b-110">以下关系图资源在 Intune 工作流之间共享:</span><span class="sxs-lookup"><span data-stu-id="99b3b-110">The following Graph resources are shared between Intune workflows:</span></span>  

- [<span data-ttu-id="99b3b-111">所有设备分配目标</span><span class="sxs-lookup"><span data-stu-id="99b3b-111">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="99b3b-112">所有许可的用户分配目标</span><span class="sxs-lookup"><span data-stu-id="99b3b-112">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="99b3b-113">符合性状态</span><span class="sxs-lookup"><span data-stu-id="99b3b-113">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="99b3b-114">设备和应用管理分配目标</span><span class="sxs-lookup"><span data-stu-id="99b3b-114">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="99b3b-115">设备应用管理</span><span class="sxs-lookup"><span data-stu-id="99b3b-115">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="99b3b-116">设备类别</span><span class="sxs-lookup"><span data-stu-id="99b3b-116">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="99b3b-117">设备管理</span><span class="sxs-lookup"><span data-stu-id="99b3b-117">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="99b3b-118">排除组分配目标</span><span class="sxs-lookup"><span data-stu-id="99b3b-118">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="99b3b-119">组分配目标</span><span class="sxs-lookup"><span data-stu-id="99b3b-119">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="99b3b-120">安装意图</span><span class="sxs-lookup"><span data-stu-id="99b3b-120">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="99b3b-121">MIME 内容</span><span class="sxs-lookup"><span data-stu-id="99b3b-121">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="99b3b-122">Report</span><span class="sxs-lookup"><span data-stu-id="99b3b-122">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="99b3b-123">报表根目录</span><span class="sxs-lookup"><span data-stu-id="99b3b-123">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="99b3b-124">保存的 UI 状态生成选项</span><span class="sxs-lookup"><span data-stu-id="99b3b-124">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="99b3b-125">URI</span><span class="sxs-lookup"><span data-stu-id="99b3b-125">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="99b3b-126">用户</span><span class="sxs-lookup"><span data-stu-id="99b3b-126">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="99b3b-127">VPP 令牌帐户类型</span><span class="sxs-lookup"><span data-stu-id="99b3b-127">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
